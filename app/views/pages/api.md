sphere
------

**Examples:**

   * `sphere(3);`
   * `sphere(r=5);`

**Arguments:**

   * `r`
     radius of the sphere

cube
----

**Examples:**

   * `cube(size = [2,3,4], center = true, r = 0.5);`
   * `cube(4);`

**Arguments:**

   * `size`
     cube size
   * `center = False`
     should center?
   * `r = 0.0`
     radius of rounding

square
------

**Examples:**

   * `square(size = [3,4], center = true, r = 0.5);`
   * `square(4);`

**Arguments:**

   * `size`
     square size
   * `center = False`
     should center?
   * `r = 0.0`
     radius of rounding

cylinder
--------

**Examples:**

   * `cylinder(r=10, h=30, center=true);`
   * `cylinder(r1=4, r2=6, h=10);`
   * `cylinder(r=5, h=10, $fn = 6);`

**Arguments:**

   * `r = 1.0`
     radius of cylinder
   * `h = 1.0`
     height of cylinder
   * `r1 = 1.0`
     bottom radius; overrides r
   * `r2 = 1.0`
     top radius; overrides r
   * `$fn = -1.0`
     number of sides, for making prisms
   * `center = False`
     center cylinder with respect to z?

circle
------

**Examples:**

   * `circle(r=10); // circle`
   * `circle(r=5, $fn=6); //hexagon`

**Arguments:**

   * `r`
     radius of the circle
   * `$fn = -1.0`
     if defined, makes a regular polygon with n sides instead of a circle

polygon
-------

**Examples:**

   * `polygon ([(0,0), (0,10), (10,0)]);`

**Arguments:**

   * `points`
     vertices of the polygon
   * `paths = []`
     order to go through vertices; ignored for now
   * `r = 0.0`
     rounding of the polygon corners; ignored for now

union
-----


**Arguments:**

   * `r = 0.0`
     Radius of rounding for the union interface

difference
----------


**Arguments:**

   * `r = 0.0`
     Radius of rounding for the difference interface

intersection
------------


**Arguments:**

   * `r = 0.0`
     Radius of rounding for the intersection interface

translate
---------

**Examples:**

   * `translate ([2,3]) circle (4);`
   * `translate ([5,6,7]) sphere(5);`

**Arguments:**

   * `v`
     vector to translate by

scale
-----

**Examples:**

   * `scale(2) square(5);`
   * `scale([2,3]) square(5);`
   * `scale([2,3,4]) cube(5);`

**Arguments:**

   * `v`
     vector or scalar to scale by

rotate
------


**Arguments:**

   * `a`
     value to rotate by; angle or list of angles

linear_extrude
--------------

**Examples:**

   * `linear_extrude(10) square(5);`

**Arguments:**

   * `height = 1.0`
     height to extrude to...
   * `center = False`
     center? (the z component)
   * `twist = Undefined`
     twist as we extrude, either a total amount to twist or a function...
   * `scale = Undefined`
     scale according to this funciton as we extrud...
   * `translate = Undefined`
     translate according to this funciton as we extrude...
   * `r = 0.0`
     round the top?

pack
----

**Examples:**

   * `pack ([45,45], sep=2) { circle(10); circle(10); circle(10); circle(10); }`

**Arguments:**

   * `size`
     size of 2D box to pack objects within
   * `sep`
     mandetory space between objects

shell
-----


**Arguments:**

   * `w`
     width of the shell...

rotate_extrude
--------------

**Examples:**

   * `rotate_extrude() translate(20) circle(10);`

**Arguments:**

   * `a = 360.0`
     angle to sweep
   * `r = 0.0`
   * `translate = [0.0,0.0]`

