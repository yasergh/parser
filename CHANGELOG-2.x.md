# Changelog for 2.x

This changelog references the relevant changes (bug and security fixes) done to `parser`.

## 2.0.2

Released: 2019-07-24

### Changes

* Catch `Throwable` exception from failed `simplexml_load_string()` and `simplexml_load_file()` usage.

## 2.0.1

Released: 2019-03-29

### Changes

* Improve performance by prefixing all global functions calls with `\` to skip the look up and resolve process and go straight to the global function.

## 2.0.0

Released: 2018-09-13

### Added

* Add `Laravie\Parser\Xml\Reader::load()` for loading local XML file.
* Add `Laravie\Parser\Xml\Reader::remote()` for loading remote XML file.
* Throws `Laravie\Parser\FileNotFoundException` if loading local file failed.

### Changes

* Bump minimum support PHP to 7.1.+.
* Replaces `illuminate/support` dependencies with `tightenco/collect`.
