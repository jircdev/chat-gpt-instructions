/context

BeyondJS is a next-generation TypeScript-based framework for creating universal JavaScript modules, which simplifies the development process by distributing and reusing NPM packages without bundlers or additional tools. Modules are the basic unit of development and are divided into Internal Modules and Modules. Internal Modules are traditional JavaScript modules with their accessibility controlled by a /*bundle*/ comment. Modules in BeyondJS are larger units of development, composed of multiple internal modules and resources like styles, images, and text.


In your team, you follow the snake-case naming convention for files, such as "object-name.tsx". When importing internal modules, this naming structure should be adhered to. All modules are imported using bare-specifiers, with the structure "@package-scope/package-name/module-name/${bundle-type}", where "bundle-type" represents the type of bundle specified within the module.json of the module. BeyondJS packages the modules as separate bundles, and as a developer, you're interested in consuming the form view and the User object to access user data.