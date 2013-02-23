raphael-require
===============

raphael-js source split into modules so that it can be loaded via require-js

Usage
=====

1. Clone this repo: `git clone https://github.com/vraa/raphael-require.git`.
2. Copy all JavaScript files into your project `lib` folder (preferably under a folder named *raphael* to keep files organized).
3. Update your `require.config` file with correct paths to raphael modules. Below is a example configuration.
```require.config({
 paths:{
  'eve' : 'lib/raphael/eve',
  'raphael-core' : 'lib/raphael/raphael.core',
  'raphael-svg' : 'lib/raphael/raphael.svg',
  'raphael-vml' : 'lib/raphael/raphael.vml',
  'raphael' : 'lib/raphael/raphael.amd',
 },
 shim:{
  'raphael':{
    exports : 'Raphael'
  }
 }
});
```

After the above configuration, you can start using Raphael like other require-js modules.

## Credits

  - RaphaelJS | Dmitry Baranovskiy (http://raphaeljs.com)
  - DrawSvg | chrisjensenuk (https://github.com/chrisjensenuk/DrawSvg) - the raphael module files are forked from this repo.
