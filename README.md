Sprint Planning System (Java OOP)

Overview

This project implements a simplified sprint planning domain model in Java.

The goal of the exercise is to practice:
	•	Inheritance
	•	Encapsulation
	•	Business logic implementation
	•	Defensive copying
	•	Working without using Collections or Streams

The system models core SCRUM concepts such as Tickets, User Stories, Bugs, and Sprints.

⸻

Project Structure

The following classes are implemented:
	•	Ticket
	•	UserStory (extends Ticket)
	•	Bug (extends Ticket)
	•	Sprint

⸻

Class Responsibilities

Ticket

Base class representing a task.

Properties:
	•	id
	•	name
	•	estimate (hours)
	•	completed state

Features:
	•	Mark ticket as completed
	•	Check completion status
	•	Access ticket properties

⸻

UserStory

Represents a user story with dependencies.

Features:
	•	Cannot be completed until all dependencies are completed
	•	Returns defensive copy of dependencies
	•	Custom string representation
[US 1] User Registration Entity


⸻

Bug

Represents a bug linked to a completed UserStory.

Features:
	•	Created only if related UserStory exists and is completed
	•	Custom string representation

[Bug 2] Registration Form: Add password repeat

Sprint

Represents a sprint with:
	•	Time capacity
	•	Ticket limit

Rules:
	•	Cannot exceed total estimate capacity
	•	Cannot exceed ticket limit
	•	Cannot accept null tickets
	•	Cannot accept already completed tickets
	•	UserStory dependencies must be accepted first

Provides:
	•	Add methods for UserStory and Bug
	•	Defensive copy of tickets
	•	Total estimate calculation

⸻

Constraints

This implementation does NOT use:
	•	Collections
	•	Streams

Only arrays are used where required.

⸻

Purpose

This project demonstrates understanding of:
	•	Object-Oriented Programming principles
	•	Class inheritance
	•	Business rule validation
	•	Defensive programming
	•	Clean API implementation


