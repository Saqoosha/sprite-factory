January 13th 2013 - v1.5.2
--------------------------
 * replaced `:csspath` option with `:cssurl` [issue #21](https://github.com/jakesgordon/sprite-factory/issues/21)
 * ordered css rules by pseudoclass importance [issue #20](https://github.com/jakesgordon/sprite-factory/pull/20)
 * added support for .ico files when using rmagick [issue #18](https://github.com/jakesgordon/sprite-factory/pull/18)

June 11th 2012 - v1.5.1
-----------------------
 * added a new `:return => :images` option for callers that want access to the detailed `images` hash instead of the generated css content

May 10th 2012 - v1.5.0
----------------------
 * @halida added a new `margin` option to (optionally) separate images in generated spritesheet to avoid 'bleeding' when browser scales the sprite (e.g. when user increases text size)
 * added `padding` support for `packed` layout
 * added `margin` support for `packed` layout
 * added support for using source image filename as automatic css selector [issue #12](https://github.com/jakesgordon/sprite-factory/issues/12)
 * added support for `:hover` (and other pseudo-class) selectors [issue #14](https://github.com/jakesgordon/sprite-factory/issues/14)

February 29th 2012 - v1.4.2
---------------------------
 * added support for `:nocomments => true` to suppress comments in generated output stylesheet
 * added support for images in subfolders - fixes [github issue #11](https://github.com/jakesgordon/sprite-factory/issues/11)

August 5th 2011 - v1.4.1
------------------------
 * added support for `:style => :scss` to generate .scss file (even though content will be almost exactly same as .css style)
 * deprecated `:output` option and replaced it with 2 new explicit `:output_image` and `:output_style` options
 * updated RELEASE NOTES to include setup for use with Rails 3.1 asset pipeline

Auguest 5th 2011 - v1.4.0
-------------------------
 * (not available)

July 9th 2011 - v1.3.0
----------------------

 * source image file extensions now treated in case INsensitive manner (e.g. we detect both .PNG, .png and .Png)
 * added `:nocss => true` option to suppress generation of output css file (caller should use `run!` return value instead - it contains the generated css content as a string)

May 8th 2011 - v1.2.0
---------------------

 * added new `:layout => :packed` option to use bin-packing algorithm for generating rectangular sprite sheet
 * added pngcrush support

April 29th 2011 - v1.0.0
------------------------

 * original version
