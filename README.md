# Object-Oriented Guest Manager

Key Features

The Object-Oriented Guest Manager is a sophisticated event administration platform designed to facilitate the comprehensive management of guest registries with precision and ease. The system allows for seamless guest registration, capturing critical data such as names, ages, and detailed geographic information through an integrated address management system and a structured country enumeration. While the project’s heritage is rooted in fundamental 2D-array management for data persistence, it has evolved into a robust object-oriented solution where each attendee is handled as a distinct, encapsulated entity. Furthermore, the application provides real-time statistics, automatically generating analytical reports that distinguish between adult and child demographics while identifying the oldest and youngest attendees to offer organizers immediate oversight. Advanced functionalities, such as the ability to modify existing entries and dynamic seat swapping via index manipulation, ensure that the registry remains flexible and responsive throughout the lifecycle of an event.

Technical Implementation

This application is engineered in Java and adheres to a modular Model-View-Controller (MVC) architecture, ensuring a clean separation between data logic, user interface components, and event handling. Moving away from the elementary use of `java.util.Scanner` and primitive 2D String arrays found in earlier procedural versions, this implementation utilizes the `javax.swing` library and `JOptionPane` to provide a professional Graphical User Interface (GUI). The system’s architecture is defined by specialized classes—including `Guest`, `Address`, and `GuestManager`—which leverage private attributes and public accessor methods to maintain high levels of data integrity. This transition to a modular framework allows for efficient UI management, where a centralized controller utilizes a switch-case structure to bridge the gap between user interactions and the underlying data model.

Challenges & Reflection

Transitioning to an object-oriented paradigm proved to be an intensive pedagogical challenge, requiring a shift in perspective from simple scripting to complex system architecture. A significant portion of the development was dedicated to robust input validation, specifically implementing checks such as `hasNextInt` and regex matching to ensure that non-numeric or empty strings do not compromise the system’s stability. The project also required rigorous error handling for domain-specific constraints, such as preventing negative ages or unassigned address fields within the class constructors. Reflecting on the implementation, the report highlights that while the logic was initially centralized within the main method in previous procedural assignments, the decision to move logic into discrete, method-driven classes significantly enhanced the software's maintainability and long-term scalability.

Getting Started

To initialize the Object-Oriented Guest Manager on your local system, ensure you have the JDK installed and execute the following commands in your terminal:

```bash
# Navigate to the source root directory
cd da339a_U2_src_Alper_Eken

# Compile the modular package structure
javac partyController/*.java partyModel/*.java partyView/*.java

# Run the application via the MainProgram entry point
java partyController.MainProgram
