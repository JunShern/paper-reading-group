# paper-reading-group

Theme based on [no style, please!](https://github.com/riggraz/no-style-please/tree/0a8ef94aac31a70d306d7463248386f0d9314a1a)

# Development

Serve locally:
```
bundle exec jekyll serve
```

Generate thumbnail images with `imagemagick`:
```
cp -r full/ thumb
mogrify -resize 75X75 thumb/*/*.png
```