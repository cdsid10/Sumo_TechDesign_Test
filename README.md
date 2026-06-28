# Sumo Digital – Technical Designer Assessment

## Project Overview

This repository contains my submission for the **Sumo Digital Technical Designer Assessment**, developed in **Unreal Engine 5** using the Third Person Template.

The project focuses on demonstrating gameplay system architecture, multiplayer fundamentals, and technical design thinking through clean, well-documented Blueprint implementations. Throughout the project, Blueprint comments have been included to explain the reasoning behind key gameplay, networking, and architectural decisions rather than simply documenting node functionality.

---

# Technical Test

## Part One – Health System & Gameplay Object

### Health System

Implemented a modular, reusable health system featuring:

* Health implemented as a reusable Actor Component
* Current Health and Max Health
* Centralised damage processing
* Death handling
* Visual damage feedback
* Blueprint comments explaining design decisions and implementation reasoning

### Gameplay Object

Implemented a multiplayer-compatible spike trap that:

* Damages the player while active
* Retracts after activation
* Reactivates only once the trigger area becomes clear
* Separates gameplay state from visual presentation
* Includes Blueprint comments documenting gameplay and technical design decisions

---

## Part Two – Multiplayer

The gameplay object was adapted to function correctly within a multiplayer environment.

Implemented features include:

* Server-authoritative damage handling
* Replicated health values using RepNotify
* Multiplayer-compatible gameplay logic
* Replicated player death handling
* Blueprint comments explaining networking decisions and implementation choices

---

# Design Approach

The project was developed around the following technical design principles:

* **Modularity** – Gameplay systems are separated into reusable components where appropriate.
* **Maintainability** – Gameplay logic is centralised to reduce duplicated behaviour and simplify future expansion.
* **Server Authority** – Gameplay-critical logic is executed on the server, with clients reacting through replicated state.
* **Readability** – Blueprint comments focus on explaining design decisions and implementation reasoning to communicate the thought process behind the solution.

---

# Running the Project

## Requirements

* Unreal Engine 5

## Single Player

1. Open the project in Unreal Engine 5.
2. Load the default level if it is not already open.
3. Press **Play**.

## Multiplayer

1. Open the **Play** settings.
2. Set **Number of Players** to **2** (or more).
3. Launch using a **Listen Server**.
4. Interact with the spike trap to verify replicated health, damage, and death behaviour.

---

# Notes

The accompanying **Design Test** has been submitted separately via the Google Docs link provided in my submission email.

Thank you for taking the time to review my submission.
