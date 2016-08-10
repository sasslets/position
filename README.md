Sasslets - position
=====================

Installation
------------
``` sh
bower install sasslets-position --save-dev
```
``` sh
npm install sasslets-position --save-dev
```

Usage
-----

> signature

``` sass
@include position(fixed|absolute|relative|etc, $top, $right, $bottom, $left )
```

> shortcuts

``` sass
@include absolute( $top, $right, $bottom, $left )
@include fixed( $top, $right, $bottom, $left )
@include relative( $top, $right, $bottom, $left )
```

> example 1

``` sass
@include position( fixed, 0, 0, null, 0 )
```
> returns:

``` css
position: fixed;
top: 0;
right: 0;
left: 0;
```

> example 2

``` sass
@include position( absolute, 0, 0 )
```
> returns:

``` css
position: absolute;
top: 0;
right: 0;
```

> example 3

``` sass
@include fixed( 1rem, 1rem )
```
> returns:

``` css
position: fixed;
top: 1rem;
right: 1rem;
```


> example words 1

``` sass
@include fixed( top )
```
> returns:

``` css
position: fixed;
top: 0;
right: 0;
left: 0;
```

> example words 2

``` sass
@include fixed( left )
```
> returns:

``` css
position: fixed;
top: 0;
left: 0;
bottom: 0;
```

> example words 3

``` sass
@include fixed( top, left )
```
> returns:

``` css
position: fixed;
top: 0;
left: 0;
```

> example words 4

``` sass
@include fixed( bottom )
```
> returns:

``` css
position: fixed;
bottom: 0;
left: 0;
right: 0;
```
