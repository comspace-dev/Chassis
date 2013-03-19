# Chassis

Chassis is a mixin for Sass giving you a solid grid ready for use on your website.

## Requirements

- Of course you need a way to compile [Sass](http://sass-lang.com)
- You should import Pilot before all other Sass files

## Constants

	$gutter-width-px: 20 !default;
	$use-clearfix: false !default;

The default value for the width of the gutter is set to 20px. If you like to change that, do that in your custom stylesheet. Do not edit this value in the Chassis file.

Change the value of <code>$use-clearfix</code> to <code>true</code> if you like to clear the floats with the clearfix placeholder class instead of <code>overflow: hidden;</code>.

## The mixin

## Placeholder classes

### %grid

This class is the container for our grids. It does clear the floats of the grids.

### %grid__item

This is the base class for our grids. You should <code>@extend</code> it wherever you need a grid.

### %clearfix

If you choose to clear the floats with the clearfix this class is used. We provide this class because we can not know if you already have a clearfix class in your stylesheet. Safety first.