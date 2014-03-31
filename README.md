Pharo ideas
===========
This is a collection of my ideas about cool features in Pharo. Feel free to contact me or to implement them.

Test-method runtime binding
---------------------------
We can gather an information about what methods are executed when test is being run. This way test can register to the methods and run itself each time a method is modified. A true **auto-testing**.

Projects
--------
Right now there is no notion of a **project** in Pharo. Project should be based around the concept of a _package_ that is present now. Then it should have optional modules such as tests, benchmarks, code critics, ext… Each module should be able to store additional data e.g.: tests should store data about method binding (see: _Test-method runtime binding_), code critics should store false-positives. Additional data of the modules should clutter the source code. Having project structure should enable a concept of **resources** – a non-code data.
