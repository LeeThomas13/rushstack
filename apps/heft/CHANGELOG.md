# Change Log - @rushstack/heft

This log was last generated on Thu, 13 Aug 2020 09:26:39 GMT and should not be manually modified.

## 0.4.7
Thu, 13 Aug 2020 09:26:39 GMT

### Patches

- Fix a race condition where .js files were sometimes read by Jest before they were written by TypeScript
- Fix an issue where the TypeScript incremental build cache sometimes did not work correctly in "--watch" mode
- Add support for "additionalModuleKindsToEmit" in watch mode

## 0.4.6
Thu, 13 Aug 2020 04:57:38 GMT

### Patches

- Fix an issue with incorrect source maps for the Jest transform
- Fix a watch mode race condition where "--clean" ran in parallel with "heft test" (GitHub #2078)
- Fix an issue where "The transpiler output folder does not exist" was sometimes printed erroneously

## 0.4.5
Wed, 12 Aug 2020 00:10:05 GMT

*Version update only*

## 0.4.4
Tue, 11 Aug 2020 00:36:22 GMT

### Patches

- Fix an issue where emitted .js.map sourcemaps had an incorrect relative path (GitHub #2086)

## 0.4.3
Wed, 05 Aug 2020 18:27:33 GMT

*Version update only*

## 0.4.2
Tue, 04 Aug 2020 07:27:25 GMT

### Patches

- Update README.md logo

## 0.4.1
Mon, 03 Aug 2020 15:09:51 GMT

### Patches

- Add specific support for handling binary assets in Jest tests.

## 0.4.0
Mon, 03 Aug 2020 06:55:14 GMT

### Minor changes

- Add jest-identity-mock-transform for mocking .css imports in Webpack projects
- Add new "emitFolderPathForJest" setting in typescript.json, which simplifies how Webpack projects emit CommonJS for Jest

### Patches

- Fix an issue where jest-shared.config.json did not match .tsx file extensions
- Standardize how jest-shared.config.json references path-based imports
- Enable Jest "runInBand" when invoking Heft with "--debug"
- Fix an issue where "heft clean" did not clean Jest's unreliable cache

## 0.3.1
Thu, 30 Jul 2020 15:09:35 GMT

### Patches

- Emit errors and warnings from webpack.

## 0.3.0
Fri, 24 Jul 2020 20:40:38 GMT

### Minor changes

- Enable Heft to be used without the "@microsoft/rush-stack-compiler-n.n" system

## 0.2.2
Tue, 21 Jul 2020 00:54:55 GMT

### Patches

- Rename .heft/api-extractor.json to .heft/api-extractor-task.json to avoid confusion with API Extractor's config file

## 0.2.1
Tue, 21 Jul 2020 00:10:21 GMT

### Patches

- Update documentation

## 0.2.0
Mon, 20 Jul 2020 06:52:33 GMT

### Minor changes

- Make API Extractor's typescriptCompilerFolder option configurable.
- Include basic support for webpack-dev-server.

## 0.1.2
Thu, 16 Jul 2020 18:34:08 GMT

### Patches

- Republish to fix incorrect dependency specifier

## 0.1.1
Thu, 16 Jul 2020 17:53:35 GMT

### Patches

- Add support for TypeScript compilers older than version 3.6 (which do not support incremental compilation)

## 0.1.0
Wed, 15 Jul 2020 18:29:28 GMT

### Minor changes

- Initial release

