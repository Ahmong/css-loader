# yan-css-loader

Fork from css-loader, with following additional feature:

1. ```:import()``` from .js file. This statement will import the classname-localized_name maps from js module.
2. ```:import()``` from .vue file. This statement will import the classname-localized_name maps from vue components.
3. pseudo statment ```:reflocal(.classname)```. This statement will change the classname to the localized_name which imported from :import() statement.

