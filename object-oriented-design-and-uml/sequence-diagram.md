<h1 align="center">Sequence Diagram</h1>

Sequence diagrams describe <span style="font-size:2em;">
 interactions among classes</span> in terms of an exchange of messages over time and are used to explore the logic of complex operations, functions or procedures. In this diagram, the <span style="font-size:2em;">sequence of interactions</span> between the objects is represented in a <span style="font-size:2em;">step-by-step manner</span>.

Sequence diagrams show a detailed flow for a specific use case or even just part of a particular use case. They are almost self-explanatory; they show the calls between the different objects in their sequence and can explain, at a detailed level, different calls to various objects.

A sequence diagram has two dimensions: The vertical dimension shows the sequence of messages (top to bottom) in the chronological order that they occur; the horizontal dimension shows the object instances to which the messages are sent (between the class' instances).

<p align="center">
    <img src="/media-files/sequence-diagram.svg" alt="Sequence Diagram">
    <br />
    Sample sequence diagram for ATM balance inquiry
</p>
A sequence diagram is straightforward to draw. Across the 
<span style="font-size:2em;"> 
top
</span>
of your diagram, 
<span style="font-size:2em;"> 
identify
</span>
the class instances (objects) by putting each class instance inside a box (see above figure). If a class instance 
<span style="font-size:2em;"> 
sends a message 
</span>
to another class instance, <span style="font-size:2em;"> 
draw a line 
</span>
with an open arrowhead pointing to the receiving class instance and place the name of the message above the line. Optionally, for important messages, you can draw a <span style="font-size:2em;"> 
dotted line
</span>
with an arrowhead pointing back to the originating class instance; label the returned value above the dotted line.