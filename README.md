# Chassis

Chassis is a mixin for Sass giving you a solid grid ready for use on your website.

## Requirements

* Of course you need a way to compile [Sass](http://sass-lang.com)
* You should import Chassis before all other Sass files

## Defaults

	$gutter-width-px: 20 !default;
	$use-clearfix: false !default;
	$breakpoints: baby-bear 400, mama-bear 650, papa-bear 940 !default;

The default value for the width of the gutter is set to 20px. If you like to change that, do that in your custom stylesheet. Do not edit this value in the Chassis file.

Change the value of <code>$use-clearfix</code> to <code>true</code> if you like to clear the floats with the clearfix instead of <code>overflow: hidden;</code>.

The list of breakpoint consists of names and pixel values, although the pixel values are currently not used in Chassis.

## Placeholder classes

### %grid

This class is the container for our grids. It does clear the floats of the grids.

### %grid__item

This is the base class for our grids. You should <code>@extend</code> it wherever you need a grid.

### %grid__item--one-third

These <code>@extends</code> define the width of the grid. You can choose from one whole down to twelfths.
