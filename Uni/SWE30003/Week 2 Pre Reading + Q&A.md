### Question in Practice
Characterise the difference between verification and validation and discuss where in the software development lifecycle (SDLC) verification and validation activities should be conducted, respectively.

### TL;DR Week 2 Pre-Reading

The _Tasks & Support_ method replaces traditional functional requirements with **task descriptions**, focusing on **what the user and system accomplish together**, not who does what. This delays design decisions (e.g., division of labor between user and system), avoids premature constraints, and improves alignment with business goals.

### Key Points:

- **Traditional requirement**: Focuses only on what the _system_ does. Can be inflexible and hard to verify or adapt.
    
- **Task-based requirement**: Describes user–system tasks together. More flexible, realistic, and user-oriented.
    

### Example:

- Traditional: “System shall record check-in and allocate rooms.”
    
- Task-based: “Support task 1.2: Check-in – give guest a room, mark it occupied, and start accounting.”
    

### Structure of a Task Description:

- **Purpose (Goal)**: The outcome (e.g., guest checked in).
    
- **Trigger**: What starts the task (e.g., guest arrival).
    
- **Subtasks**: High-level steps (e.g., find room, check credit, record guest).
    
- **Variants**: Special cases (e.g., no room, guest already booked).
    
- **Frequency/Criticality**: For performance expectations (e.g., group of 50 guests).
    
- **Problem & Support columns**: Identify existing issues and suggest solutions.
    

### Benefits:

- Easier to verify and validate with users.
    
- Supports business goals more clearly.
    
- Encourages innovative and adaptable design.
    
- Faster requirements gathering (e.g., 10 days vs 25 weeks in a hospital case).
    

### Drawbacks:

- Doesn’t include quality requirements (like usability or performance).
    
- Requires a separate data model.
    
- May need training for developers and suppliers to adapt to the format.
    

### Conclusion:

Task descriptions offer a more human-centered and context-aware approach to functional requirements. They support better design decisions, clearer communication, and faster development without locking in technical details too early.

### Question to Answer
The paper mentioned using the human-centered approach with task descriptions over functional requirements in a **hospital setting**. Characterise whether task descriptions would be beneficial in a **higher education setting** and justify why this is the case. Put an emphasis on the Software Development Lifecycle (SDLC) phases and where task descriptions fit with each stage.

### Answer to Question
When a software system is being built verification is concerned with the question, "Are we building the **product right**?". Validation is concerned with the question, "Are we building the **right product**?". In terms of the Software Development Lifecycle (SDLC), verification and validation are used in multiple parts of the SDLC each, not just one each. Verification is used mainly in the: *Requirements Analysis, Design, Implementation and Testing* stages of the SDLC. Whereas validation, is used in the *Requirements Elicitation, Requirements Analysis, Testing and Maintenance* phases of the SDLC.

The justification for this is that verification is concerned with the product that has already been selected in the previous phase (*Requirements Analysis*) and designing it according to the specifications so that in the *Design* phase, the solution can be designed, modeled and specified so that then the right product can be implemented properly in the *Implementation* phase and that it matches the design. Later on in the SDLC lifecycle, the *Testing* phase can also conform that the system meets the required specifications through rigorous testing.

The justification for validation is that it is concerned by what the product should look like in the first place and whether it is the **right product**. So, the *Requirements Elicitation* phase determines whether the stakeholder's needs are met for the desired product. *Requirement Analysis* is similar, but determining whether the requirements meet the desired expectations of the stakeholders. *Testing* is also important, by double checking that the right product has actually been built and meets the stakeholder requirements via QA testing, etc and for the *Maintenance* phase - making sure once the application is deployed and if needs change, that the solution can adopt and still meet expectations.



