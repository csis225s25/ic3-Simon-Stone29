# In Class Problem Set 3

I used ComboBoxDemo.java a few years ago.  It used to compile cleanly.  Even though the code has not changed, it now  will not compile without throwing warnings.

Doing everything from a command prompt or Git Bash (no IDEs allowed), your mission is to debug the code and find out why it stopped compiling cleanly.  When you have figured it out,  note what you changed and why it stopped working in the README.md file.


**Changes to code**
We added < String > to the line where we created an instance of JComboBox called cBox1


**What caused it to stop working?** 
It was trying to create a new generic type JComboBox object without specifying the type as String.
Java warns you because it won't be able to catch an error at compile time if you pass in different typed arguments later in the code.
The compiler doesn't know what type it is supposed to be and won't be able to give an accurate error at compile time.
