<h1 align="center">Activity Diagrams</h1>

We use Activity Diagrams to illustrate the 
<span style="font-size:2em;"> 
flow of control (system functionality) 
</span>
in a system. An activity diagram shows the flow of control for a system functionality; it 
<span style="font-size:2em;"> 
emphasizes the condition of flow and the sequence
</span>
in which it happens. We can also use an activity diagram to refer to the <span style="font-size:2em;"> 
steps involved in the execution of a use case.
</span>

Activity diagrams illustrate the dynamic nature of a system by modeling the flow of control from activity to activity. An activity <span style="font-size:2em;"> 
represents an operation 
</span>
on some class in the system that <span style="font-size:2em;"> 
results in a change in the state 
</span>
of the system. Typically, activity diagrams are used to model workflow or business processes and internal operations.

Following is an activity diagram for a user performing online shopping:

<p align="center">
    <img src="/media-files/activity-diagrams.svg" alt="Activity Diagram">
    <br />
    Sample activity diagram for online shopping
</p>

**What is the difference between Activity diagram and Sequence diagram?**

**Activity diagram** 
<span style="font-size:2em;"> Tracking functions: External Inputs -> Processes/Ops -> External Output</span>
captures the process flow. It is used for functional modeling. A functional model represents the flow of values from external inputs, through operations and internal data stores, to external outputs.

**Sequence diagram** 
<span style="font-size:2em;"> Tracking States/Transitions/Triggers which cause them</span>
tracks the interaction between the objects. It is used for dynamic modeling, which is represented by tracking states, transitions between states, and the events that trigger these transitions.

