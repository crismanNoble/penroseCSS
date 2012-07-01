Penrose Triangle in CSS
=======
![Penrose Triangle](http://www4c.wolframalpha.com/Calculate/MSP/MSP2641a24h29e827h40h400000f3hd56b33d8f782?MSPStoreType=image/gif&s=26&w=397&h=200 Penrose via Wolfram Alpha)  

[From Wikipedia:](http://en.wikipedia.org/wiki/Penrose_triangle)
>The Penrose triangle, also known as the Penrose tribar, is an impossible object. It was first created by the Swedish artist Oscar Reutersvärd in 1934. The mathematician Roger Penrose independently devised and popularised it in the 1950s, describing it as "impossibility in its purest form". It is featured prominently in the works of artist M. C. Escher, whose earlier depictions of impossible objects partly inspired it.

*TLDR: [I made a penrose triangle in css](http://crismanNoble.github.com/penroseCSS) because geometry is neat.*

I used to attempt to draw penrose triangles during class, and would always sketch out a contorted mess. Then I learned geometry. If you think of a penrose triangle as a series of smaller triangles you begin to see that it is nothing more than craftily shaded [equilateral triangles](http://www.wolframalpha.com/input/?i=triangle+graph&lk=1&a=ClashPrefs_*Graph.TriangleGraph-) next to each other. 

Now that we know the secret to the penrose triangle we need to translate these learnings into CSS.

We can make a CSS triangle of pretty much any shape using [this old trick](http://davidwalsh.name/css-triangles).

A perfectly equilateral triangle would have the following properties: 2 units wide, sqrt(3) units high.

That can be approximated with this css:  
    `.triangle {
      width: 0px; 
      height: 0px; 
      border-left: 10px solid transparent;
      border-right: 10px solid transparent;
      border-bottom: 17.25px solid red;
    }`

Put triangles next to each other with the following rules
    `margin-left: -10px;
    float: left;`

Keep stacking your triagles left, your going to need 11 per row, and six rows in total. Put everything in a wrapper that is 120px wide and bam, your done.  

[See it in action](http://crismanNoble.github.com/penroseCSS).
