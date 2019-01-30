# custom-d3-bundle
D3 is pretty amazing, but as a dependency its also pretty heavy. In most cases you only need a small subset of what d3 has to offer. So creating a small custom bundle can improve load time.

This repo is based upon Mike Bostock's instructions for custom bundles:
https://bl.ocks.org/mbostock/bb09af4c39c79cffcde4

## How to

In order to create your own bundle, simply run

```
npm install
```

Open the index.js file and add/remove required modules from the d3 universe

```
export {
  event,
  select,
  selectAll
} from "d3-selection";
```

Make sure you have all required d3 packages installed:

```
npm install d3-selection --save-dev
```

Then run 

```
npm run prepublish
```

Voila.
