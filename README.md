# SoftProject
Design challenge partial for ClickUp.

In the nature of a pull request
I have decided to submit a query before moving on to the next section of the layout & learn what remains unfinished in the navbar for revision.
If you would please speak on what level's I've given too much or too little consideration.

# Table of Contents
0. [Deci-rem](#Deci-rem)
1. [Navbar](#Navbar)
2. [The Logo](#The-Logo)
3. [Menu Items](#Menu-Items)
4. [The Arrow](#The-Arrow)
5. [Considerations](#Considerations)


## Deci-rem

I applied a default font size of 62.5% to the root to convert rem to 10px for rounding, so no need for the crazy 16px conversions and division problems.
This way 1.6 rem now = 16px.

You can explictly set the font-size on a parent to 1.6rem when you want to use em,
otherwise you simply add a decimal place to any px value and the conversion is easy.


## Navbar

The highest point across elements at the top is the 'Request Demo button' 210px(13.125rem) x 60px(3.75rem)
There is 47px above this, which is where I have set the navbar.

The top content / navbar is 47 px from the top
1 px shy of 3rem(48px).

While this project is made with design software, the use of a border placeholder in design
can throw things off by the borders thinkness
whereas outlines don’t affect the elements content positioning.

The left most element is 240px(15rem) from the edge.

1248 width(47.175rem), 112(7rem) right margin.


## The Logo

Made with before and after pseudo elements, I reduced the height of the entire element by the size of margin from the top of the navbar 
to eliminate bottom overflow.


## Menu Items

To deal with the text jitter which comes from the shifting of surrounding elements by the font weight of the on focus change
I used a text shadow for the focus effect.

There are slight variations in the widths of the words by less than 1px.
the height is also 25px instead of 26px.

## The Arrow
The arrow height is 0 px, with a 2 px border border radius 2px
and the chevron cluster is a total of 14 x 6 px.

In the design software there is a 90% rotation on the element which suggests that it is the corner of a box, 
and design software allows for rounded terminals, via border radius.
But applying a border radius to a border used to make the chevron in CSS will not result in this.
So I made the arrow out of divs, much like a burger menu with before and after pseudo elements
to which rounded terminals can be applied via border radius.

Not knowing where these rotated borders were clipped, as what’s showing makes a rectangle/diamond instead of a square if mirrored,
I calculated the actual dimensions of the chevron by taking the 14 x 6 space and dividing it 
into 2 right triangles which result in 7 x 6 x ‘9.22’px - the actual length of each chevron half
each at a 49.4° angle from the tip.

However when changing my screen size to 80%, 33% and 25% in chrome and 90% and 80% in firefox the arrow renders off proportion.
I assume that this is an area where you would just use an icon or design an svg instead.

## Considerations

I can move on to responsive options via media query.
Flex was only used to Row the elements and align items vertically. I was not so sure that justify content would ensure the horizontal pixel specs of the figma design.
Or maybe I was taking pixel perfect too literally.

Using live sass watch in vs code for compliation.

I greatly appreciate as much exposure as I can get to a professional workflow and expectations.
Hopefully I can work with you all in the future or receive communications in order to prepare for the next hiring cycle or opening.

