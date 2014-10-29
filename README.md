material-sass
=============

## Using this library

1. Clone the repository (or download it as zip and extract it)
2. Remember the path to the `_material.scss` file (`<path>/_material.scss`)
3. Include the library:
  - Using SASS from command line: `sass --compass -I <path> [your-other-args]`
  - Within a compass project: Add the following line to your `config.rb`: `add_import_path "<path>"`
4. Import the files to your scss/sass: `@import "material/design;"` (or only `@import "material";` if you just want to use the helpers (variables and mixins) without importing any declared css-rules)
