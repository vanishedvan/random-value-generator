# Changelog

## 0.2.0

* Generated `browser.js` for use in websites
* Generated `emoji-code-points.json` used by `randomEmoji()` as a list of emojis to pick from
* Updated the list of emojis, which now contains 3907 emojis (2263 more than in previous version)
* Added stricter type checking for function `randomNumber(max)`, `randomInteger(max)`, `randomString(len)`, and `randomHash(len)`
* Added default `max` for `randomNumber(max)` to be `1`
* Added default `max` for `randomInteger(max)` to be `2`
* Fixed an issue where `randomInteger(max)` always returns `NaN`
* Changed `randomInteger(max)` behavior; if `max` is negative, the returned integer will now always be greater than and not equal to `max`
* Optimized `randomBoolean()`
* Added default `len` for `randomHash(len)` to be `1`
* Fixed an issue where `randomHash(len)` always returns a zero-length string, now it returns a string containing `A-Z`, `a-z`, and `0-9` as long as `len` is not `0`
* Made function `randomNumber(max)`, `randomInteger(max)`, `randomString(len)`, and `randomHash(len)` accept boxed/wrapper type parameters
* Generated `index.js`
* Generated `index.mjs` for use in projects using ES Modules
* Removed dependency `randomatic` and `uuid`

Other changes:
* Added `.gitignore`
* Added `.npmignore`
* Updated `travis.yml` to set Node.js versions for test runs
* Added `API_DOCS.md` for API documentations
* Added `BUILD_INSTRUCTIONS.md` to detail the build process
* Added `CHANGELOG.md` to list all changes for each version
* Updated `README.md`
* Moved the main portion of code into `base.js` as source for building
* Added `build.js`, `Command.js`, `CommandList.js`, and `utilities.js` for build process
* Added `EmojiScraper.js` to properly scrape emoji code points from files obtainable from [Unicode Consortium](https://unicode.org/)
* Removed `package-lock.json` and excluded the file from git tracking
* Updated description, author, and repository field in `package.json`
* Added homepage, bugs, contributors, browser, directories, and engines field in `package.json`
* Added scripts for building in `package.json`
* Added tests

## 0.1.3

* Added function [`randomEmoji()`](/API_DOCS.md#randomemoji)
* Changed `randomHash(len)` behavior to always return a zero-length string

Other changes:
* Started utilizing Travis CI in development phase
* Prepared for code testing
* Updated `README.md`

## 0.1.2

Updated `README.md`

## 0.1.1

No changes.

## 0.1.0

No changes.

## 0.0.2

* Removed accidental debug logging in `index.js`

Other changes:
* Added keywords field in `package.json`
* Updated description, author, license, and repository field in `package.json`
* Added more content to `README.md`
* Committed `package-lock.json`

## 0.0.1

Initial release.