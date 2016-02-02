# showcar-icons

This module provides custom elements for simple inclusion of icons in your frontend project.

## Installation:

To install showcar-icons within your project use bower.

    bower install --save git@github.com:AutoScout24/showcar-icons.git


## How to include:
To make the custom elements available within you frontend, it is necessary to include some javascript (depending on your directory structure)

    require('showcar-icons/dist/showcar-icons.min.js');


## How to use:

use the following to include an icon in your frontend

    <as24-icon type="t-online"></as24-icon>
    <as24-icon type="flag/de"></as24-icon>

All the available icons are placed within the icons folder, using subfolder is possible too.  
If you want to use the icons without the showcar-ui library, you have to load a polyfill for custom elements first.  
See <https://cdnjs.com/libraries/document-register-element>

    <script src="//cdnjs.cloudflare.com/ajax/libs/document-register-element/0.5.4/document-register-element.js"></script>

## How to create different sizes

You can change the size of an svg by overriding css declarations.  
Example:

    as24-icon[type='navigation/car'] {
        svg {
            width: 42px;
            height: 34px;
        }
    }

## How to contribute:

If you need some additional icons within showcar-icons just add them to the icons folder or another subfolder. Afterwards it is necessary to create the showcar-icons.min.js again.

Rebuild showcar-icons.min.js with grunt:

    grunt

## License

MIT License
