# @gulp-plugin/collect ![npm (custom registry)](https://img.shields.io/npm/v/@gulp-plugin/collect?logo=npm) [![GitHub Package Registry version](https://img.shields.io/github/release/gulp-plugin/collect.svg?label=gpr&logo=github)](https://github.com/gulp-plugin/collect/packages/)

[![Build](https://github.com/gulp-plugin/collect/actions/workflows/node.js.yml/badge.svg)](https://github.com/gulp-plugin/collect/actions/workflows/node.js.yml)  [![Coverage Status](https://coveralls.io/repos/github/gulp-plugin/collect/badge.svg?branch=master)](https://coveralls.io/github/gulp-plugin/collect?branch=master) [![dependencies Status](https://david-dm.org/gulp-plugin/collect/status.svg)](https://david-dm.org/gulp-plugin/collect)

A JavaScript/TypeScript file gathering plugin for [gulp](https://github.com/gulpjs/gulp)

## Installation

```shell
npm install --save-dev @gulp-plugin/collect
```

## Usage

Then, add it to your `gulpfile.js`:

```typescript
const collect = require('@gulp-plugin/collect');

gulp.src('src/**/*.ts')
	.pipe(collect('typescript'))
	.pipe(gulp.dest('dist/'));

gulp.src('src/**/*.js')
  .pipe(collect('javascript'))
  .pipe(gulp.dest('dist/'));

const files = filenames.get('typescript') // ['a.ts','b.ts']
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
