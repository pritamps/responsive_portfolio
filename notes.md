# Notes

## JavaScript

* Can select individual DOM elements with `document.querySelector('.className')`. 
* Can select all elements inside a `div` with `document.querySelectorAll('.className')`.
* Can add and remove classes to an element by using `element.classList.add('newClass')`.

## SASS and CSS

1. Global variables with `$`
2. Can do sub-properties and sub-classes and sub-states using the `&` operator. For example:
```css
h1 {
    &.lg-heading {
        font-size: 6rem;
    }
main {
    h1 {
        font-size: 6rem;
    }
a {
    &:hover {
        color: blue;
    }
.menu {
    &-branding {  // This will apply to class menu-branding.
        color: yellow;
    }
}
```
4. `lighten($primary-color, 2)` can be used to lighten colors.
5. `@mixin` allows for functions
6. `@if` works for if-then-else
7. Pseudo-elements like `&:after`: One use is to avoid standard `overlay` divs
8. Partial files start with `_`
9. `&:after` adds a div with content specified by content property after the div. Example: 
```css
    &:after {
        content: '';
        position: absolute;
        top: 0;
        right: 0;
        width: 100%;
        height: 100%;
        z-index: -1;
        background: rgba($primary-color, $background-opacity);
    }
```
10. `translate3D` adds translation.

## NPM 

* Install npm: from website
* Initialize `package.json` from this folder: `npm init`
* Install NPM sass `npm install node-sass`
* Change script in `package.json` to automatically run `node-sass` with watching option (`-w`) and recursive (`--recursive`):
```
node-sass -w scss/ -o dist/css --recursive
```
* How to deal with VS code (Windows) throwing error with the `-w` flag for `node-sass`: [link](https://stackoverflow.com/questions/50395998/vscode-wont-work-with-filewatchers)

