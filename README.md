# pdfmake [![Build Status][travis_img]][travis_url] [![GitHub][github_img]][github_url] [![npm][npm_img]][npm_url] [![Bower][bower_img]][bower_url] [![Packagist][packagist_img]][packagist_url] [![CDNJS][cdnjs_img]][cndjs_url]

[travis_img]: https://travis-ci.org/bpampuch/pdfmake.svg?branch=master
[travis_url]: https://travis-ci.org/bpampuch/pdfmake
[github_img]: https://img.shields.io/github/release/bpampuch/pdfmake.svg
[github_url]: https://github.com/bpampuch/pdfmake/releases/latest
[npm_img]: https://img.shields.io/npm/v/pdfmake.svg?colorB=0E7FBF
[npm_url]: https://www.npmjs.com/package/pdfmake
[bower_img]: https://img.shields.io/bower/v/pdfmake.svg?colorB=0E7FBF
[bower_url]: https://github.com/bpampuch/pdfmake
[packagist_img]: https://img.shields.io/packagist/v/bpampuch/pdfmake.svg?colorB=0E7FBF
[packagist_url]: https://packagist.org/packages/bpampuch/pdfmake
[cdnjs_img]: https://img.shields.io/cdnjs/v/pdfmake.svg?colorB=0E7FBF
[cndjs_url]: https://cdnjs.com/libraries/pdfmake

### 为什么有这个 fork？

- pdfmake 默认使用英文字体，该 fork 替换英文字体为开源的思源黑体
- 为减少字体文件大小，只使用了常规字体，因此设置字体为斜体和粗体时，字体依然显示常规字体

### Why this fork?

- pdfmake uses English fonts by default, and the fork replaces the English fonts with the open source Siyuan boldface
- In order to reduce the font file size, only regular fonts are used, so when the font is set to italics and bold, the font still displays regular fonts

```javascript
pdfMake.fonts = {
	SourceHanSC: {
		normal: "SourceHanSansCN-Regular.ttf",
		bold: "SourceHanSansCN-Regular.ttf",
		italics: "SourceHanSansCN-Regular.ttf",
		bolditalics: "SourceHanSansCN-Regular.ttf",
	},
};
```

PDF document generation library for server-side and client-side in pure JavaScript.

Check out [the playground](http://bpampuch.github.io/pdfmake/playground.html) and [examples](https://github.com/bpampuch/pdfmake/tree/master/examples).

#### This is unstable master branch for version 0.2.x, for stable version 0.1.x see [branch 0.1](https://github.com/bpampuch/pdfmake/tree/0.1).

### Features

- line-wrapping,
- text-alignments (left, right, centered, justified),
- numbered and bulleted lists,
- tables and columns
  - auto/fixed/star-sized widths,
  - col-spans and row-spans,
  - headers automatically repeated in case of a page-break,
- images and vector graphics,
- convenient styling and style inheritance,
- page headers and footers:
  - static or dynamic content,
  - access to current page number and page count,
- background-layer,
- page dimensions and orientations,
- margins,
- custom page breaks,
- font embedding,
- support for complex, multi-level (nested) structures,
- table of contents,
- helper methods for opening/printing/downloading the generated PDF,
- setting of PDF metadata (e.g. author, subject).

## Documentation

Documentation URL: https://pdfmake.github.io/docs/

## Building from sources

using npm:

```
git clone https://github.com/bpampuch/pdfmake.git
cd pdfmake
npm install
npm run build
```

using yarn:

```
git clone https://github.com/bpampuch/pdfmake.git
cd pdfmake
yarn
yarn run build
```

## License

MIT

## Authors

- [@bpampuch](https://github.com/bpampuch) (founder)
- [@liborm85](https://github.com/liborm85)

pdfmake is based on a truly amazing library [pdfkit](https://github.com/devongovett/pdfkit) (credits to [@devongovett](https://github.com/devongovett)).

Thanks to all contributors.
