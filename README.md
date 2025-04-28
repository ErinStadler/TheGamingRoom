# Draw It or Lose It: Software Design Documentation

## Client Overview
**The Gaming Room** was the client for this project. They developed a popular Android-based game called **Draw It or Lose It** and wanted to expand it into a **web-based platform** accessible across multiple operating systems and devices. 

The Gaming Room required a scalable, secure, and highly available software solution that supported real-time interaction between players on different platforms.

## Project Summary
The Gaming Room tasked us with designing the software architecture for **Draw It or Lose It**. They requested a system that would support:
- Multiple teams and players
- Unique team and game names
- Single-instance memory management using a singleton pattern
- Scalability across web, mobile, and desktop environments
- Strong security measures to protect user data

Our design involved proposing a **microservices architecture** with **cloud-based deployment**, a **Linux server environment**, and technologies such as **PostgreSQL**, **MongoDB**, **OAuth 2.0**, and **WebSockets** to meet the requirements.

## Strengths in Documentation
One thing I did particularly well was **clearly aligning the system design to the client’s business goals**. Each recommendation (operating platform, memory management, storage solution) was backed with technical rationale tied directly to user needs, making the documentation focused, professional, and user-centric.

## Benefits of the Design Documentation Process
Working through the design document was helpful in clarifying the **core system architecture before starting to code**. It forced me to deeply consider factors like scalability, security, and distributed communication early on. Having a solid blueprint made the development phase smoother, as I already had solutions in mind for potential problems.

## Opportunities for Improvement
If I could revise one part of the documentation, I would **expand the diagrams and visuals**. A few UML diagrams and a visual system architecture map would have made the document even more readable and helped stakeholders better understand how the different components connect. In the future, I would invest more time in creating architectural diagrams alongside written explanations.

## Interpreting and Implementing User Needs
I interpreted the user’s needs by **mapping each requirement directly to a system design choice** (for example, ensuring single-instance gameplay via a singleton pattern, and enabling multi-platform accessibility through a web-based design).

It is critically important to prioritize user needs because they define the success or failure of the software; without addressing the core goals of scalability, usability, and security, the final product would not satisfy the client or the end users.

## Approach to Software Design
My approach to software design involved:
- **Analyzing** the client's goals and technical constraints
- **Selecting appropriate patterns** (e.g., Singleton, REST APIs, Microservices)
- **Proposing scalable, secure architectures** tailored to real-world deployment
- **Documenting every design choice** with clear justifications

In the future, I would use techniques such as:
- Building more **visual wireframes** early in the process
- Conducting **risk analysis** for scalability and security vulnerabilities
- Using **agile iteration** even in early design phases to incorporate client feedback more dynamically

---

# 🛠️ Known Issues (Initial Commit)

> The following bugs and issues are currently being addressed:

- Missing `package com.gameauth;` declaration in some Java classes.
- Minimal JavaDoc documentation for classes and methods.
- Use of hardcoded users in `GameAuthenticator`; needs secure user management.
- REST controllers (`GameUserRESTController`, `RESTClientController`) lack robust exception handling.
- No dependency injection is used for controller/service classes.
- Very limited test coverage (only application startup is tested).
- Basic hardcoded role checks in `GameAuthorizer`; needs dynamic RBAC support.
- Need to fully review and validate `config.yml` settings.

✅ These issues are known and will be fixed in future commits to improve security, maintainability, and scalability.
