A jekyll repo for my first attempt at web development using gulp deployment and browser sync. 
Pug -> html 
sass -> css 

```javascript
var deploy = require("gulp-gh-pages");

gulp.task("deploy", ["jekyll-build"], function () {
    return gulp.src("./_site/**/*")
        .pipe(deploy());
});
```
