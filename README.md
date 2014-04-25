# SCSS (Sass) Sugar for Espresso 2

## Features (Work in progress)

This Sugar is incomplete, but it's better than nothing. Here is what is currently supported:

* Use of .scss file extension or .css.scss extension to trigger the Sugar
* CSS (plain and simple) - this is inherited from the default CSS Sugar
* @include selector
* @mixin definition
* @warn directive
* @debug directive
* @if @else if @else @for @while statements
* $variable use, $variable definitions at root level
* !default suffix
* functions (the syntax is already a part of CSS)
* Nested selectors (only up to 5 levels deep, and only root level selectors show up in the navigator ATM)

### Changelog
- 2014-04-25: Forked from [github.com/sfcgeorge/Sass.sugar](https://github.com/sfcgeorge/Sass.sugar)

## Installation

1. Download the zip
2. Extract said zip
3. Rename folder to .sugar
4. Double click the .sugar file
5. Restart Espresso - voila!

## Who did this?

Credits go to [github.com/sfcgeorge/](https://github.com/sfcgeorge/) who did the original sugar.

### Future goals
I have no intention to create a fully 100% compatible sugar for SCSS syntax. That would be to much work. This is just a temporary fix until Espresso gets native support for SCSS. But feel free to send in pull requests to this repo with your fixes.

### Implementation

Basic CSS structure and functionality is already implemented by the Default CSS Sugar, so why reinvent the wheel? We include the default CSS Syntax, then build on it using SyntaxInjections. We shouldn't need to touch the Syntax file often, use SyntaxInjections where possible. Some of the original CSS Sugar are commented out purely for reference.
