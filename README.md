Penrose Triangle in CSS
=======
![Penrose Triangle](http://upload.wikimedia.org/wikipedia/commons/thumb/c/c1/Penrose-dreieck.svg/192px-Penrose-dreieck.svg.png "Penrose via Wikipedia")  

[From Wikipedia:](http://en.wikipedia.org/wiki/Penrose_triangle)
>The Penrose triangle, also known as the Penrose tribar, is an impossible object. It was first created by the Swedish artist Oscar Reutersvärd in 1934. The mathematician Roger Penrose independently devised and popularised it in the 1950s, describing it as "impossibility in its purest form". It is featured prominently in the works of artist M. C. Escher, whose earlier depictions of impossible objects partly inspired it.

The follwoing is the boring story of recreating the famous penrose triangle using CSS.

I used to attempt to draw penrose triangles during class, and would always sketch out a contorted mess. Then I learned geometry. If you think of a penrose triangle as a series of smaller triangles you begin to see that it is nothing more than craftily shaded [equilateral triangles](http://www.wolframalpha.com/input/?i=triangle+graph&lk=1&a=ClashPrefs_*Graph.TriangleGraph-) next to each other. 

Now that we know the secret to the penrose triangle we need to translate these learnings into CSS.

We can make a CSS triangle of pretty much any shape using [this old trick](http://davidwalsh.name/css-triangles).

An isometric triangle has the following properties:

That can be approximated with this css:
    .triangle {
      width: 0px; 
      height: 0px; 
      border-left: 10px solid transparent;
      border-right: 10px solid transparent;
      border-bottom: 17.25px solid red;
    }

Put two next to each other with the following rules
    margin-left: -10px;
    float: left;

Make a new line of triangles:

start shading them properly

have a bit of fun with skrollr

Make some shit.
