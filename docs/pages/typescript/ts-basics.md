### **Typescript Intro**

- As we know **JavaScript** is evolved from java.But unlike java, JS is loosely coupled.
  Means less rules...With this it become super easy to write and learn code...

- But eventually (over the time)... Dependency injection ( adding dependency or sending params to methods, passing values to function is called dependency injection) become much more complex... As the developer has to read all the code traversal to understand what type of parameters to send or to receive.

- In short unpredictable state issue...(To resolve this problem... Only to some extent, there evolved some packages like propTypes ( npm package) was created and widely used...).But that didn't solved the total problem.
- Hence Microsoft came up with **JS + TYPES = Typescript**. Which gives predictable state. Even before compilation. That is at the time of writing code itself. one can know what is input type and output type...

- Of course it demands extra code to be written For types but it helps With typescript developers.
- Especially who has to work with distributed teams or legacy projects. Observed significant boost in productivity as it reduced the mis-understanding / unpredictability among the code written by other/ old devs. And reduced the HOURS of KT.
- When it comes to compilation, Typescript compiler runs the type check system and converts the total code into pure JavaScript by removing all typings in build(which is native JS).
