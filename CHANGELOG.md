#### 2.0.0 (2022-06-15)

- Add support for NodeJs v18
- **(Breaking change)**: `ArcFile.extraction` is optional for `createExtractorFromData` now. If `ArcFile.fileHeader.flags.directory` is `true`, this field will be `undefined`.

#### 1.0.6 (2022-03-16)

- Add `createExtractorFromFile` support in Webpack

#### 1.0.5 (2022-02-28)

- Fix an issue on file extracting to current working directory ('./')

#### 1.0.4 (2022-02-15)

- Fix folder creation issue on Windows.

#### 1.0.3 (2021-05-10)

- Fix for Security Vulnerability on dependencies

#### 1.0.2 (2021-04-01)

- Fix for Security Vulnerability on dependencies

#### 1.0.1 (2021-02-18)

- Add new option `filenameTransform` for `ExtractorFromFileOptions`.

#### 1.0.0 (2020-12-29)

- Refactory by the latest EMScripten and UnRar DLL source. Since both of them changed a lot, there are many breaking changes in this update
- **(Breaking change)**: Use Javascript Exception instead of tuple `[state, result]` for error handling.
- **(Breaking change)**: The extractor object return by `createExtractorFromData` and `createExtractorFromFile` are now promise object. Since loading the wasm object in the latest EMScriten is asynchronized.
- **(Breaking change)**: The `fileHeaders` and `files` returned by the extractions api are changed from array to iterator, make the extraction lazy.

#### 0.8.0

- First release
