# Fractals
An interactive visualization of the Mandelbrot set written with HTML and JavaScript - this project uses JavaScript and the HTML canvas element to draw the Mandelbrot set and allow the user to zoom in and out. The crux of this program is a function that determines whether or not a number is in the set. This is done with a for loop to estimate whether a complex number diverges and returns how many iterations through the loop it takes for the number to diverge. This value is used to color the pixel that represents that number on the canvas.

## The Mandelbrot Set
The Mandelbrot set is  defined as the set of complex numbers *c* for which the function f(*z*) = *z<sup>2</sup>* + *c* does not diverge when iterated from *z* = 0.

Let's try and break that down in English...

One way of defining the Mandelbrot set is by looking at how complex functions behave under repeated iteration. A complex function is on that is defined on complex numbers - numbers with the form a + bi (i is an 'imaginary number' that represents the square root of -1). The function in question is f(*z*) = *z<sup>2</sup>* + *c*, where c is a complex number. For each *c* we start with *z* = 0 and evaluate the function. The result is then plugged back in as the value for *z* and we repeat the process. As we continue to iterate the function, the iterates either get larger or are bounded and remain close to 0. The values for *c* that stay close to 0 make up the Mandelbrot set.

If you're interested in a much better explanation, I recommend [this article](https://blogs.scientificamerican.com/roots-of-unity/a-few-of-my-favorite-spaces-the-mandelbrot-set/).
