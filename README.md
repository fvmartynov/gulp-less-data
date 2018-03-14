# Gulp LESS Data

## Fork info
Fixed bug:
* Data property serialized as undefined if contains slashes. Now serialized as strings.

## Install
```sh
npm install gulp-less-data
```
## Usage

```javascript
var gulp = require("gulp");
var less = require("gulp-less");
var lessData = require("gulp-less-data")


gulp.src("test.less")
    .pipe(lessData({
        color: "red",
        bgcolor: "blue"
    }))
    .pipe(less())
    .pipe(gulp.dest("./dest"));
```

## TODO

Eh, need more? Forget it! 
