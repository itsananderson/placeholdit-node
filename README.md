placeholdit
===========

Simple CLI node utility that downloads images from [placehold.it](http://placehold.it).

Installation
------------

Installing is quite simple

```
npm install -g placeholdit 
```

If you want to reuse the file fetching logic, you can also install placeholdit as a dependency of your own module

```
npm install --save placeholdit 
```

Usage
-----

Placeholdit is pretty easy to use.

```
placeholdit [-d path/to/download/folder] width[xheight] [...]
```

Here are some concrete usage examples

```bash
placeholdit 200x100 # Download a 200x100 image
placeholdit 100x300 200 # Download a 100x300 image and a 200x200 image
placeholdit -d placeholders 800x600 # Download a 800x600 image into the placeholders folder
```

In order for the -d (a.k.a. --directory) flag to work, the folder must already exist.
Otherwise placeholdit will just return an error.
