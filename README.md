     Vlasterx                                                   
     _|_|_|_|                      _|                  
     _|        _|_|    _|_|_|    _|_|_|_|              
     _|_|_|  _|    _|  _|    _|    _|                  
     _|      _|    _|  _|    _|    _|                  
     _|        _|_|    _|    _|      _|_| 

     _|_|_|    _|_|_|    _|_|    _|      _|    _|_|_|  
       _|    _|        _|    _|  _|_|    _|  _|        
       _|    _|        _|    _|  _|  _|  _|    _|_|    
       _|    _|        _|    _|  _|    _|_|        _|  
     _|_|_|    _|_|_|    _|_|    _|      _|  _|_|_|    
                                                   
                                                   
This collection of scripts enables end-user to create font-icons from SVG graphics.
It is build on top of **node.js** and multiple **gulp** processes. 

Download from: [vxFontIcons GitHub](https://github.com/Vlasterx/vxFontIcons)

## How to install?

### Install from scratch:
1. Clone this repo in a local folder
2. Install [Node.js](http://nodejs.org/download)

### From within local folder run these commands:
1. Install **gulp** globally by running command: `npm install gulp -g`
2. Install all required gulp plugins by running command: `npm install`

You are now all set to use this collection.


## How to use it?
In order to use this collection, you first need to do following steps:

1. Copy your SVG's to `icons16` folder
2. In your shell run `gulp` command

Gulp process will do the following
- It will create icon fonts and will copy them to `fonts/vxIcons` folder
- It will create SCSS styles within that folder
- It will create styleGuide for your icons by using KSS node and will place it in `styleGuide` folder


## File Revving
This font building pack usess font revving, which means that it will add different font version for each build. Apache will be able to read and refresh fonts every time they are rebuilt without user needing to reload a page or empty browser cache, so keep in mind that `.htaccess` file.


## Custom font name
If you want to change font name, you need to change few lines of code.

1. In `gulpfile.js` find `var fontName = 'vxIcons'` and change 'vxIcons' to your font name
2. In `scss/icons.scss` find and change `@import "fonts/vxIcons/vxIcons";`


## Author
Vladimir Jovanović
[Twitter](https://twitter.com/vlasterx) | [Facebook](https://www.facebook.com/dizajn.ninja) | [LinkedIn](http://vx.rs/linkedin) 