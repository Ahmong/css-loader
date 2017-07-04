# yan-css-loader

Fork from css-loader, with following additional feature:

1. ```:import()``` from .js file. This statement will import the classname-localized_name maps from js module. The js module being imported should export a 'locals' map object. You may use [csslocals-from-js-loader](https://github.com/Ahmong/csslocals-from-js-loader) to export the expected 'locals' object.
2. ```:import()``` from .vue file. This statement will import the classname-localized_name maps from vue components. The vue components should export a 'locals' map object, this may be done by using a webpack loader [csslocals-from-vue-loader](https://github.com/Ahmong/csslocals-from-vue-loader).
3. pseudo selector ```:reflocal(.classname)```. This selector will change the classname to the localized_name which imported from :import() statement.
