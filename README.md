webpack-output-action
=====================
### Notes
- DO NOT use release assets URL as CDN
- js file generated by this action cannot be used inside `<script type="module">`.  Use [jsdelivr](https://www.jsdelivr.com/) for ESM instead.
  - may change outputlibrarytype to 'module' if really needed
  - Can use [addaleax/gen-esm-wrapper](https://github.com/addaleax/gen-esm-wrapper) to generate ESM wrapper files for CommonJS modules

### Used by
- [dirkarnez/web-audio-playground](https://github.com/dirkarnez/web-audio-playground)

### TODO
- [x] `var exportModule`
  - https://www.webpackjs.com/configuration/output/#outputlibrarytype
- [ ] esm to umd support?
  - [Unable to import webpack-bundled UMD library as an ES6 import · Issue #9232 · webpack/webpack](https://github.com/webpack/webpack/issues/9232)