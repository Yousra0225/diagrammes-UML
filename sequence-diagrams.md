# Sequence Diagrams
*The sequence diagram is a type of UML diagram that shows the order of interactions between objects/actors, over time to execute a specific scenario*.  
The main concepts found in a UML sequence diagram are: 
* **The participants** : the actors or objects that are involved in the scenario.
* **The time line** : the order of the interactions between the participants.
* **The messages** : the interactions between the participants.
* **Creation and destruction** : the creation and destruction of the participants.

## Elements of a Sequence Diagram 
### 1. Participants (Lifelines)
- Represent objects, actors, or systems involved.
- Drawn at the top as boxes with names.
- Below each, a dashed vertical line called a **lifeline** shows their activity over time.

### 2. Messages
- Horizontal arrows between participants.
- Represent method calls or signals.
- Each arrow is labeled with the **operation name** (e.g. `sendEmail()`).

### 3. Activation Bars
- Thin vertical rectangles on a lifeline.
- Show that an object is actively executing a method.
- Begin when a message is received and end when the task is done.

### 4. Object Creation
- Shown with a **dashed arrow** labeled with `new` or `<<create>>`.
- A new participant (lifeline) appears when the object is created.

### 5. Object Destruction (optional)
- Marked with an **X** at the end of a lifeline.
- Shows when the object is removed from memory.
