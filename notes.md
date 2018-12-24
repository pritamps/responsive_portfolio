# Notes

## NPM 

* Install npm: from website
* Initialize `package.json` from this folder: `npm init`
* Install NPM sass `npm install node-sass`
* Change script in `package.json` to automatically run `node-sass` with watching option (`-w`) and recursive (`--recursive`):
```
node-sass -w scss/ -o dist/css --recursive
```
* How to deal with VS code (Windows) throwing error with the `-w` flag for `node-sass`: [link](https://stackoverflow.com/questions/50395998/vscode-wont-work-with-filewatchers)

## SASS

1. Global variables with `$`
2. Can do sub-properties using the `&` operator. For example:
```css
h1 {
    &.lg-heading {
        font-size: 6rem;
    }
```