
gulp-phpjade-mod
=============


This module is a modification of [gulp-jade-php](https://travis-ci.org/oroce/gulp-jade-php) which itself
is based on the well written [gulp-jade](https://github.com/phated/gulp-jade).

It is used to compile [phpjade-mod](https://github.com/kimkwanka/phpjade-mod) templates using gulp.

### Usage

    var jade = require('gulp-phpjade-mod');

    gulp.task('templates', function() {
      gulp.src('./views/**/*.jade')
        .pipe(jade({
            locals: {
              title: 'Dat website title'
            }
         }))
         .pipe(gulp.dest('./dist'));
    });

### Options

Like gulp-jade-php this module is based on gulp-jade,so it supports everything mentioned in gulp-jade's [README](https://github.com/phated/gulp-jade#options).

The default extension is `.php`, but like with gulp-jade-php you can pass `extension: '.phtml'` to generate phtml files.

### Licence

The MIT License (MIT)

Copyright (c) 2015 Kim Kwanka

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.