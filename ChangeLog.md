### 0.3.1 / 2015-04-17

* Drop support for hunspell-1.2

### 0.3.0 / 2013-05-01

* Detect Ubuntu's hunspell directory (`/usr/share/hunspell`).
* {FFI::Hunspell::Dictionary#encoding} now returns an `Encoding` object.
* Encode Strings returned from {FFI::Hunspell::Dictionary#stem} and
  {FFI::Hunspell::Dictionary#suggestions} to match the dictionary's native
  encoding.

### 0.2.6 / 2013-02-05

* Removed the env dependency.
* Check the returned count from `Hunsepll_stem` in
  {FFI::Hunspell::Dictionary#stem}.
* Check the returned count from `Hunspell_suggest` in
  {FFI::Hunspell::Dictionary#suggest}.

### 0.2.5 / 2012-05-11

* Load `libhunspell-1.2.so.0` if `libhunspell-1.2.so` cannot be found.
* Load `libhunspell-1.3.so.0` if `libhunspell-1.3.so` cannot be found.

### 0.2.4 / 2012-04-27

* Require ffi ~> 1.0.
* Attempt loading `libhunspell-1.2` and `libhunspell-1.3`.

### 0.2.3 / 2011-02-02

* Require ffi >= 0.6.0 and <= 1.1.0:
  * JRuby requires ffi >= 1.0.0.
  * A lot of projects still require ffi ~> 0.6.0.

### 0.2.2 / 2011-01-25

* Added {FFI::Hunspell::USER_DIR}.
* Added {FFI::Hunspell::KNOWN_DIRECTORIES}, containing known dictionary
  directories used by Debian, Fedora and Mac Ports.
* Have {FFI::Hunspell.directories} return the dictionary directories found
  on the system.

### 0.2.1 / 2011-01-23

* Require env ~> 0.1.2.
  * Use `Env.lang` to get the default language.
* Updated the Copyright years.

### 0.2.0 / 2011-01-22

* Added {FFI::Hunspell.lang}.
* Added {FFI::Hunspell.lang=}.
* Added {FFI::Hunspell.directories}.
* Have {FFI::Hunspell::Dictionary.open} accept a language name, and search
  {FFI::Hunspell.directories} for the dictionary files.

### 0.1.0 / 2010-10-05

* Initial release.

