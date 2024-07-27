<h1 align="center">Class Diagram</h1>

Class diagram is the backbone of object-oriented modeling - it shows how different entities (people, things, and data) relate to each other. In other words, it shows the static structures of the system.

A class diagram describes the attributes and operations of a class and also the constraints imposed on the system. Class diagrams are widely used in the modeling of object-oriented systems because they are the only UML diagrams that can be mapped directly to object-oriented languages.

The purpose of the class diagram can be summarized as:

1. <span style="font-size:2em;"> Analysis and design of the static view of an application. </span>
2. To describe the <span style="font-size:2em;">responsibilities</span> of a system.
3. To provide <span style="font-size:2em;">a base</span> for component and deployment diagrams.
4. Forward and reverse engineering.

A class is depicted in the class diagram as a rectangle with three horizontal sections, as shown in the figure below. The upper section shows the class’s name (Flight), the middle section contains the properties of the class, and the lower section contains the class’s operations (or “methods”).

<p align="center">
    <img src="/media-files/class-relationship.svg" alt="Class Relationships">
</p>

These are the different types of relationships between classes:

**Association:** If two classes in a model need to communicate with each other, there must be <span style="font-size:2em;"> a link </span> between them. This link can be represented by an association. Associations can be represented in a class diagram by a line between these classes with an arrow indicating the navigation direction.

* By default, associations are always assumed to be <span style="font-size:2em;">bi-directional</span> this means that both classes are aware of each other and their relationship. In the diagram below, the association between Pilot and FlightInstance is bi-directional, as both classes know each other.

By contrast, in a <span style="font-size:2em;">uni-directional </span> association, two classes are related - but <span style="font-size:2em;"> only one class knows that the relationship exists </span>. 
  
* In the below example, only Flight class knows about Aircraft; hence it is a uni-directional association

**Multiplicity:** Multiplicity indicates <span style="font-size:2em;">how many </span> instances of a class participate in the relationship. It is a constraint that specifies the <span style="font-size:2em;"> range of permitted cardinalities between two classes </span>. 

For example, in the diagram below, one FlightInstance will have two Pilots, while a Pilot can have many FlightInstances. A ranged multiplicity can be expressed as “0…*” which means “zero to many" or as “2…4” which means “two to four”.

We can indicate the multiplicity of an association by adding multiplicity adornments to the line denoting the association. The below diagram, demonstrates that a FlightInstance has exactly two Pilots but a Pilot can have many FlightInstances.

<span style="font-size:2em;">
FlightInstance will have 2 Pilots, a (each) Pilot will have multiple FlightInstances
</span>

<p align="center">
    <img src="/media-files/class-diagram.png" alt="Class Diagram">
    <br />
    Sample class diagram for flight reservation system
</p>

**Aggregation:** 

<p align="center">
    <img src="/media-files/Aggregation.png" alt="Class Diagram">
</p>

Aggregation is a special type of association used to model a “whole to its parts” relationship. In a basic aggregation relati`onship, the lifecycle of a <span style="font-size:2em;">PART class is independent of the WHOLE class’s lifecycle </span>. In other words, aggregation implies a relationship where the child <span style="font-size:2em;">can exist independently of the parent </span>. In the above diagram, Aircraft can exist without Airline.

**Composition:** 

<p align="center">
    <img src="/media-files/Composition.png" alt="Class Diagram">
</p>

The composition aggregation relationship is just another form of the aggregation relationship, but the child class’s instance lifecycle is dependent on the parent class’s instance lifecycle. In other words, Composition implies a relationship where the child <span style="font-size:2em;">cannot exist independent </span>  of the parent. In the above example, WeeklySchedule is composed in Flight which means when Flight lifecycle ends, WeeklySchedule automatically gets destroyed.

**Generalization:** 

<p align="center">
    <img src="/media-files/Generalization.png" alt="Class Diagram">
</p>

Generalization is the mechanism for <span style="font-size:2em;"> combining similar classes of objects into a single, more general class </span>. Generalization <span style="font-size:2em;">identifies commonalities </span> among a set of entities. In the above diagram, Crew, Pilot, and Admin, all are Person.

**Dependency:** 

<p align="center">
    <img src="/media-files/Association.png" alt="Class Diagram">
</p>

A dependency relationship is a relationship in which one class, the client, <span style="font-size:2em;"> uses or depends on another class </span>, the supplier. In the above diagram, FlightReservation depends on Payment.

**Abstract Class:** 


An abstract class is identified by specifying its name in <span style="font-size:2em;">_italics_</span>. In the above diagram, both Person and Account classes are abstract classes.

<p align="center">
    <img src="/media-files/uml-conversion.svg" alt="UML Conversion">
</p>