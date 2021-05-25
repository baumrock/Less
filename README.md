# Less parser for ProcessWire 

This is a ProcessWire module front-end for the [Wikimedia LESS parser](https://github.com/wikimedia/less.php).
Originally developed by Bernhard Baumrock with additions by Ryan Cramer. Requires ProcessWire 3.0.164+. 

## Install

1. Copy all files included in this module into new directory `/site/modules/Less/`.
2. In the ProcessWire admin, go to Modules > Refresh. 
3. Click install for the Less module. 

## API usage

### Compile two .less files to a css file
~~~~~
$less = $modules->get('Less');
$less->setOption('compress', true);
$less->addFile('/path/to/file1.less');
$less->addFile('/path/to/file2.less'); 
$less->saveCss('/path/to/file.min.css'); 
~~~~~

### Access Wikimedia less parser directly
~~~~~
$parser = $less->parser();
$parser->parseFile('/path/to/file.less');
$css = $parser->getCss();
~~~~~
For details about API methods you can access from `$parser` see: <https://github.com/wikimedia/less.php>

## Usage with ProcessWire’s AdminThemeUikit module

Install this module to add the ability to customize the ProcessWire core AdminThemeUikit admin theme module CSS.
For this usage, you must have ProcessWire 3.0.179 or newer. This section will be completed once the feature is
available in ProcessWire.

## License

This module uses the Apache license for consistency with the Wikimedia LESS parser license.

