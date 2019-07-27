Introduction to the concept of Autotiling
-----------------------------------------

The purpose of this presentation is to familiarize you with the concept of autotiling, and to allow you to determine your needs in the field, it is not a tutorial on the application of this system in Godot.

For that, I advise you the tutorial of michagamedev (https://michagamedev.wordpress.com/2018/02/24/181/) until a complete documentation is written.

In some tileset, tiles are made to assemble. In this way for example.

.. image:: https://i.imgur.com/fAdeoyv.png

Here it's quite simple, but it can quickly become complex.

.. image:: https://i.imgur.com/cr2YfVA.png

Creating a map with this kind of tilesets can quickly become infernal because you have to choose from a large number of tiles, the tile A that connects correctly to tile B.

To simplify map creation with tilesets of this type, there is the autotiling system.
Who will choose the right tile for you ?

You do that : You get that :

.. image:: https://i.imgur.com/NKpbGVf.png

There are three modes of autotiling in Godot.
 - 2X2
 - 3X3 (minimal)
 - 3X3

Understanding the difference between these three modes is not obvious.

Autotile mode 2X2
-----------------

This mode requires only 16 tiles unique, and allows to make areas with a width of 2 minimum, otherwise it does not work.

It can be used to make surfaces, paths, gravel, lakes, but also rooms.

Here are two examples made with the 2X2 mode.

- In this example we can see a gravel path in the grass.
.. image:: https://i.imgur.com/tsD8b88.png
(Daniel Cook - http://www.lostgarden.com/2006/07/more-free-game-graphics.html)

- And here we can see an example with rooms.
.. image:: https://i.imgur.com/kVUTIsv.png
(pixel_poem - https://twitter.com/pixel_poem)

With this mode, there may be visual bugs, there are impossible combinations. Here is an impossible example, in this case, Godot, do not answer any more.

.. image:: https://i.imgur.com/GcnqtAv.png

Autotile mode 3X3 minimal
-------------------------

If you have the courage to draw 48 unique tiles, this is definitely the mode you need.
With this mode, you will be able to make grounds such as walls, lakes, rivers, but also platforms.

.. image:: https://i.imgur.com/tzY7G04.png
.. image:: https://i.imgur.com/RnYMGpN.png

If you do not make mistakes in the tileset, there will never be a visual bug. There are still impossible configurations.
Because yes, it's the 3X3 MINIMAL!

But why minimal?
Well, because there is an even more complete mode, with more tiles, very more tiles.

Autotile mode 3X3
-----------------

More ? Oh yes, 256 tiles is a lot.

.. image:: https://i.imgur.com/9F59zj0.png

The interest may not be obvious. With this single image.

.. image:: https://i.imgur.com/rk0za0x.png

In this image we can see that the tile takes into account the presence of corners and changes shape, which is not the case in 3x3 minimal version.

This mode detects diagonal connections, so you can use this information. Or not !

.. image:: https://i.imgur.com/MLxOy6Z.png

Conclusion
----------

It remains for you to determine your needs during your preparatory drawing.
I wish you a good level design :wink:
