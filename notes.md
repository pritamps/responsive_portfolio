# Notes

## NPM 

* Install npm: from website
* Initialize `package.json` from this folder: `npm init`
* Install NPM sass `npm install node-sass`
* Change script in `package.json` to automatically run `node-sass` with watching option (`-w`) and recursive (`--recursive`):
```
node-sass -w scss/ -o dist/css --recursive
```