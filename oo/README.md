# A day of an object in the memory
> *Author*: Enrique Urra - enrique.urra@gmail.com

>* Learning object-oriented programming is hard.
>* A key is to understand how objects are running and interacting in the memory of the computer.
>* I developed some useful concept infographic examples [here](OO-infographic-example.pdf) and material [here](OO-material-example.pdf) (check slides 25-41) that allows to explain how objects live and survive in the memory of the computer, step-by-step from their creation, through its modification and until their destruction.

To learn *object-oriented programming (OO)* is hard. Actually, to learn a procedural programming approach is actually hard, and over that, the object-oriented approach adds to it many concepts and abstractions that require a lot of flexibility in organizing and articulating code. *Polymorphism*? *Encapsulation*? These are not really OO-exclusive concepts, but OO forces you in some way to systematically apply them.

I never learned OO in University. Maybe the basics, but in a mechanical way. I really understood and learned OO concepts with this:

<img src="uo-screen.jpg" width="500"/>

For oldies, this is a screenshot of *Ultima Online* (UO), one of the most classic MMORPGs in history. Years ago I spent many hours on it, not only playing but also *coding*. That is because in older times 
(and in present), UO was played in official servers and in *alternative servers*, and the later were implemented and deployed with specific *emulators*. One of them was [RunUO](https://www.runuo.net/), an emulator completely coded in .NET (using C#). These emulators not only allowed to play the game close to the experience of official servers but also through *custom implementations* of the UO world that you can code in C#. I largely collaborated in the customization of local servers by implementing a lot of scripts for new NPCs, game systems and different mechanisms. Being this a pure-OO language, I effectively understood all those alien OO-concepts that I was taught in university. Imagine that you must implement a class that represent an NPC (a monster in the UO world, for example), and to develop its behavior and properties through the class methods and attributes. That was a straightforward approach of OO-learning!

From this experience, I learned one of the key element to effectively learn OO mechanisms: to understand *how objects are running and interacting in the memory of the computer*. In some way, you need to understand the objects that you are manipulating with code, the relationships between them (that are created at runtime) and the effects of their modification in the program behavior, i.e., the *program state*. This is hard because in OO, most of this complexity is direct implemented in classes, that are abstractions of objects. Because of that, you need to *visualize* objects within the first steps. With monsters, weapons and other UO-entities can be more easy to understand, but in common programming tasks, you need to deal with more abstract entities.

When teaching OO, specifically when teaching Java, [besides some useful concept infographic examples](OO-infographic-example.pdf), I produced some material that allowed me to explain to students how objects live and survive in the memory of the computer, step-by-step from their creation, through its modification and until their destruction. Something like the following image:

<img src="oo-memory-example.jpg" width="700"/>

It was fundamental to translate very-technical concepts into simpler ones. For example, computer memory is represented by a simple big-grey-box in which objects live. A single object is simply a rectangular-cuboid, in which some data is defined. This allows to effectively explain that you can have many objects of the same class, and each one has the same properties, but with different values. Live relationships between and/or to objects (i.e., references) are represented with dotted lines pointing to the related entities.

This gets more interesting when you include arrays in the memory:

<img src="oo-memory-example-2.jpg" width="700"/>

In this way, you can effectively explain what is really happening with the code at rightmost part of the diagram, step-by-step, and visualize how memory changes with each line of code at the leftmost part, which allows to transform pretty abstract concepts and behavior into very concrete examples. [You can see the complete material here](OO-material-example.pdf), in which these (slides 25-41) and other visual explanations (and code repositories) regarding OO-concepts are provided.