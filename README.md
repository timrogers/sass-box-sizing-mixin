Box Sizing Mixin / box-sizing.scss
===================================

By default, the web browsers we use on a daily basis use the __W3C box model__. Under this model, the width of a box does not include the padding and the border - instead, this is added on top of this value to the outside of the box's content.

However, modern browsers, and the CSS specification offer some useful CSS properties that allow you to change how this works. There are two other possible values which you can use to different effect:

- padding-box (not supported by CSS3 specification, but implemented in Firefox and WebKit)

`@import box-sizing; sass-box-sizing(padding);`

With this option, the width of the box includes the padding of the box, but the border is still tacked into the outside independently.

- border-box

`@import box-sizing; sass-box-sizing(border);`

With this option, the width of the box includes both the border and the padding, so the width you specify will actually be the width of everything related to the box, except the margins of course.

- content-box

`@import box-sizing; sass-box-sizing(content);`

This is the default W3C option, that is used in browsers if no other property is specified.

About
------

This is a mixin for the Sass CSS meta-language, created by [Tim Rogers](http://www.tim-rogers.co.uk). This work is completely in the public domain. Use it as you see fit!