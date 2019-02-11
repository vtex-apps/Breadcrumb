# VTEX Breadcrumb

## Description
The VTEX Breadcrumb app is a secondary navigation scheme that reveals the user location on the site.
This is a VTEX app that is used by Dreamstore product.

:loudspeaker: **Disclaimer:** Don't fork this project. Use, contribute, or open issue with your feature request.

## Release schedule
| Release  | Status              | Initial Release | Maintenance LTS Start | End-of-life | Dreamstore Compatibility
| :--:     | :---:               |  :---:          | :---:                 | :---:       | :---: 
| [0.x]    | **Maintenance LTS** |  2018-05-29     | 2018-11-20            | March 2019  | 1.x
| [1.x]    | **Current Release** |  2018-11-20     |                       |             | 2.x
See our [LTS policy](https://github.com/vtex-apps/awesome-io#lts-policy) for more information.

## Table of Contents
- [Usage](#usage)
- [API](#api)
  - [Blocks API](#blocks-api)
    - [Configuration](#configuration)
  - [Styles API](#styles-api)
- [Troubleshooting](#troubleshooting)
- [Tests](#tests)

## Usage

This app uses our store builder with the blocks architecture. To know more about Store Builder [click here.](https://help.vtex.com/en/tutorial/understanding-storebuilder-and-stylesbuilder#structuring-and-configuring-our-store-with-object-object)

To use this app you need to add it in your dependencies in the `manifest.json` file.

```json
"dependencies": {
    "vtex.breadcrumb": "1.x",
}
```

Then, add `breadcrumb` block into your app theme, like we do in our [Dreamstore app](https://github.com/vtex-apps/dreamstore/blob/master/store/blocks.json). 

### Blocks API
:construction: :construction: :construction:

This app has an interface that describes what rules must be implemented by a block when you want to use the `breadcrumb` block.

```json
  "breadcrumb": {
    "component": "Breadcrumb"
  }
```

#### Configuration 
Through the Storefront you can change the behavior and interface of `breadcrumb`. But, you can also make adjusts in your theme app, like Dreamstore does.

| Prop name          | Type           | Description                                                                 |
| ------------------ | -------------- | --------------------------------------------------------------------------- |
| `term`             | `String`       | Term used to get to that specific page on the website                       |
| `categories`       | `Array(String)`| List of categories which the product belongs to  							|

### Styles API
:construction: :construction: :construction:

## Troubleshooting
You can check if others are passing through similar issues [here](https://github.com/vtex-apps/breadcrumb/issues). Also feel free to [open issues](https://github.com/vtex-apps/breadcrumb/issues/new) or contribute with pull requests.

## Tests

To execute our tests go to react/ folder and run yarn test