# SASS and SCSS

## Introduction
SASS (Syntactically Awesome Style Sheets) is a preprocessor scripting language that is interpreted or compiled into CSS. SCSS (Sassy CSS) is a syntax of SASS which is more like CSS and easier to use for those who are familiar with CSS.

## Features
- **Nesting**: Allows you to nest your CSS selectors in a way that follows the same visual hierarchy of your HTML.
- **Variables**: Enables you to use variables to store values you want to reuse throughout your stylesheet.
- **Partials and Import**: Lets you break your CSS into smaller, reusable pieces.
- **Mixins**: Allows you to create reusable chunks of code.
- **Inheritance**: Helps you share a set of CSS properties from one selector to another.
- **Operators**: Perform calculations to determine CSS property values.

## Installation
To install SASS, you can use npm:
```bash
npm install -g sass
```

## Usage
To compile SCSS to CSS, use the following command:
```bash
sass input.scss output.css
```

## Example
Here is an example of SCSS code:
```scss
$primary-color: #333;

body {
    font: 100% $primary-color;
}

nav {
    ul {
        margin: 0;
        padding: 0;
        list-style: none;
    }

    li { 
        display: inline-block; 
    }

    a {
        font-weight: bold;
        text-decoration: none;
        color: $primary-color;

        &:hover {
            color: lighten($primary-color, 10%);
        }
    }
}
```

### SASS Example
Here is an example of SASS code:

```sass
$primary-color: #333

body
    font: 100% $primary-color

nav
    ul
        margin: 0
        padding: 0
        list-style: none

    li 
        display: inline-block

    a
        font-weight: bold
        text-decoration: none
        color: $primary-color

        &:hover
            color: lighten($primary-color, 10%)
```

## Resources
- [SASS Official Website](https://sass-lang.com/)
- [SASS Documentation](https://sass-lang.com/documentation)

## License
This project is licensed under the MIT License.