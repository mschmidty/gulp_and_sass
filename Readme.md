This is a repository to help a friend get their head around [sass](https://sass-lang.com/) and [gulp](https://gulpjs.com/). It uses gulp to process sass and make a single line of css. It is well commented and simple so that it is easy to understand for someone just learning about sass or gulp.

# How to Install!
```bash
git clone https://github.com/mschmidty/gulp_and_sass.git
cd gulp_and_sass
npm install
```

And then to start watching files and processing them to css:

```bash
gulp
```

And you should see this with no errors:
```bash                       
[20:41:46] Using gulpfile ~/Dropbox/web_dev/test/gulp_and_sass/gulpfile.js
[20:41:46] Starting 'default'...
```
Every time you save a file it should detect the changes and overwrite the css files with the changes. You should see:

```bash
[20:53:15] Starting 'css'...
[20:53:15] Finished 'css' after 184 ms
```
There will be a warning if you have done something wrong.

# Whats happening
All of the .scss files are in the `src/scss/` folder.  Typically you have one file, which I've called `main.scss` here that you used as your parent scss file.  It will pull all of the other files into it using `@import "filename";`.  These can be in folders.  For the rest, check out the [Sass guide](https://sass-lang.com/guide) (you can toggle if you want scss or sass).  They do a better job of describing it then I could.

# A note on SCSS vs Sass
They are different although you hear them used like they are the same thing sometimes. This is an example of .scss.  I use scss in my day to day work. I have used sass too. To tell you the truth if it weren't for habit I might use sass.  

### Sass
```sass
.class-name
  border: 2px solid $black
  background: #BADA55
    .nested-class-name
      margin-top: 30px
```
### SCSS
```scss
.class-name{
  border: 2px solid $black;
  background: #BADA55;
    .nested-class-name{
      margin-top: 30px;
    }
}
```




