material-sass
=============

## Using this library

1. Clone the repository (or download it as zip and extract it)
2. Remember the path to the `_material.scss` file (`<path>/_material.scss`)
3. Include the library:
  - Using SASS from command line: `sass --compass -I <path> [your-other-args]`
  - Within a compass project: Add the following line to your `config.rb`: `add_import_path "<path>"`
4. Import the files to your scss/sass: `@import "material/design;"` (or only `@import "material";` if you just want to use the helpers (variables and mixins) without importing any declared css-rules)

## Available Helpers

### Variables

#### `@import "material/colors";`
* Every color with every hue like `$<colorName>-<hue>` (e.g. `$red-500` or `$deepPurple-A400`)
* Every color as map with the hues as keys and the colors as values (e.g. `map-get($red, 500)` or `map-get($deepPurple, A400)`)
* The `$colors`-map with the color names as keys and the color-maps as values (useful in `@each` statements)
* [More information here](http://www.google.com/design/spec/style/color.html#color-ui-color-palette)

#### `@import "material/defaults`;
* `$primary-<hue>` and `$accent-<hue>` (defaults are indigo(primary) and pink(accent))

### Mixins

#### `@import "material/mixins";`
* `z-depth(n)` sets the box-shadow to emulate the given z-depth. Valid values are 1 to 5 or 0 for no shadow (e.g. `@include z-depth(2);`) [More information here](http://www.google.com/design/spec/layout/layout-principles.html#layout-principles-dimensionality)
