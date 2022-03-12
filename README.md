# superset-plugin-ant-funnel

This is the Superset Plugin Chart ant-funnel Superset Chart Plugin.

### Usage

To add the package to Superset, go to the `superset-frontend` subdirectory in your Superset source folder

```
npm i -S @ant-design/plots

npm i -S superset-plugin-ant-funnel
```

After this edit the `superset-frontend/src/visualizations/presets/MainPreset.js` and make the following changes:

```js
import { SupersetPluginAntFunnel } from "superset-plugin-ant-funnel";
```

to import the plugin and later add the following to the array that's passed to the `plugins` property:

```js
new SupersetPluginAntFunnel().configure({
    key: 'superset-plugin-ant-funnel',
     }),
```

After that the plugin should show up when you run Superset, e.g. the development server:

```
npm run dev-server
```
