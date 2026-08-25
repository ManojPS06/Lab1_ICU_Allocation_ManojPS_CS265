# Lab 1: Requirements Engineering & UML Use-Case Modelling

**Problem Statement #20 — Healthcare & Telemedicine**
**Hospital Bed & ICU Allocation Dashboard**

## Problem Context

An emergency room bed management dashboard displaying real-time ward occupancy, prioritizing ICU transfers based on triage score, and orchestrating inter-facility ambulance transfer workflows.

**Actors:** Triage Nurse, Hospital Administrator, Ambulance Dispatcher

## Deliverables

| File | Description |
|---|---|
| [`Requirements_Table.docx`](./Requirements_Table.docx) | 5 Functional Requirements (FR-001–FR-005) and 2 Non-Functional Requirements (NFR-001–NFR-002), each with ID, Type, Description, Priority, Acceptance Criteria, and Rationale. |
| [`UseCase_Diagram.pdf`](./UseCase_Diagram.pdf) | UML Use-Case Diagram with all actors, 7 use cases, one `<<include>>` relationship (Request ICU Bed Transfer → Verify Bed Availability), and one `<<extend>>` relationship (Coordinate Inter-Facility Ambulance Transfer → Request ICU Bed Transfer). |
| [`UseCase_Flow.docx`](./UseCase_Flow.docx) | Use-Case Flow Specification for "Request ICU Bed Transfer" (UC-03) — Preconditions, Postconditions, Main Success Scenario, and one Alternate Flow. |

## Summary

- **Core FR-001:** Computes triage severity scores from intake vitals and dynamically orders the ER bed allocation waitlist.
- **Core NFR-001:** Bed status transitions must propagate to all connected ER dashboard clients in under 1 second via WebSockets.
- **Use-Case Diagram actors:** Triage Nurse, Hospital Administrator, Ambulance Dispatcher.
- **Use cases:** Compute Triage Score & Prioritize Waitlist, Monitor Real-Time Ward Occupancy, Request ICU Bed Transfer, Verify Bed Availability, Coordinate Inter-Facility Ambulance Transfer, Update Bed Status, Generate Occupancy Report.

## Author

Manoj — PES1UG24CS265, Section E.
