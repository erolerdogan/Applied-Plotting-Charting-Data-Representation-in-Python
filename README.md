# Applied-Plotting-Charting-Data-Representation-in-Python
Data Visualization, Data Virtualization in Python 

#Some Great Informations;
**Matplotlib**  (http://www.aosabook.org/en/matplotlib.html)
Matplotlib's origin dates to an attempt by one of us (John Hunter) to free himself and his fellow epilepsy researchers from a proprietary software package for doing electrocorticography (ECoG) analysis. 

Matplotlib encapsulates not just the drawing interfaces to allow rendering to multiple devices, but also the basic event handling and windowing of most popular user interface toolkits. Because of this, users can create fairly rich interactive graphics and toolkits

The architecture to accomplish this is logically separated into three layers, which can be viewed as a stack. Each layer that sits above another layer knows how to talk to the layer below it, but the lower layer is not aware of the layers above it. The three layers from bottom to top are: **backend, artist, and scripting**.

**Backend Layer** 
-FigureCanvas encapsulates the concept of a surface to draw onto (e.g. "the paper").
-Renderer does the drawing (e.g. "the paintbrush").
-Event handles user inputs such as keyboard and mouse events.

**Artist Layer**
This hierarchy is the middle layer of the matplotlib stack, and is the place where much of the heavy lifting happens.  It is the object that knows how to take the Renderer (the paintbrush) and put ink on the canvas. Everything you see in a matplotlib Figure is an Artist instance; the title, the lines, the tick labels, the images, and so on all correspond to individual Artist instances. There are two types of Artists in the hierarchy. Primitive artists represent the kinds of objects you see in a plot: Line2D, Rectangle, Circle, and Text. Composite artists are collections of Artists such as the Axis, Tick, Axes, and Figure. Each composite artist may contain other composite artists as well as primitive artists. For example, the Figure contains one or more composite Axes and the background of the Figure is a primitive Rectangle.

**Scripting Layer (pyplot)**
Most special-purpose languages for data analysis and visualization provide a lighter scripting interface to simplify common tasks, and matplotlib does so as well in its matplotlib.pyplot interface.
