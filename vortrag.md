# Design & Implementation of a Fraud Detection System for Autonomous Teams

## Motivation
- Fraud activity is an unlawful action, where someone intentionally deceives other person or system for their own profit
- Fraud prevention is a serious matter, FTC reported 70% increase in fraud activities in 2021, compared to 2020 (#cite)
- Large businesses usually are built upon multiple teams that have their own responsibility and expertise
- The independent teams have their own preferences and practices. They even might have a different idea on how a fraudulent customer might be
- The goal of this research is to establish collaboration between multiple autonomous teams in a single fraud detection process as efficiently as possible

## Analysis
- Fraud (#cite) detection techniques can be categorized to 2 parts, supervised and unsupervised
- Lots of researches on how to detect fraud better, more accurate
- Project don't want to compete with them, won't come up with a better algorithm to predict fraud
- Project only explores the possibility of collaboration between teams in a fraud detection process
- Used unsupervised method, rule based detection
- Rule based is not the perfect method, difficult to manage, and the rules have to be adapted
- Rule based can be useful when there's not much prior knowledge on how a fraudulent entity might be
- Chosen rule based because it's the simplest form to implement, and it is the most suitable method to collaborate on

## Use Cases
- Use case diagram created to visualize the flow of a fraud detection process and the possible use cases of the system
- User stories are defined by reexamining the use case diagram. The user stories will be the single source of truth for the requirements of the system

## Architecture
- Show system and SW architecture
- The UI and FDS is part of the Layered Architecture. Presentation Layer (UI), Business Layer (FDS), Database Layer (MongoDB)
- The message broker is NOT a part of the layer. Message broker is rather a part of event driven architecture. But I won't necessarily state that the software is built upon event driven architecture, because only a part of it 
- Mention node, for UI it's de facto and for backend because of its non-blocking I/O operation

## Business Layer
- Show sequences, do not go into detail on ALL of it, keep it short and simple, as said by the Prof.

## Result
- Docker compose, all components can be run as Docker containers in one command
- Most configurations can be configured via environment variables (no need to touch code)
- Additional necessary features that are discovered during the implementation process is implemented
- Testing (SW built with TDD), try to test as much as possible

## Evaluation
- Go to user story table and its implementation

## Demonstration
- Demo time!

## Outlook
- Hoped that this system can establish a common ground for autonomous teams to collaborate on a fraud detection process
- Not ready to be used in a real world scenario out of the box, more improvement such as data security and GDPR needed