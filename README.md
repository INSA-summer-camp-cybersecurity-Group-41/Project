# Lightweight SIEM
**A Cybersecurity Project Proposal for the Information Network Security Administration (INSA)**

- **Group:** 41
- **Focus Area:** Security Information and Event Management (SIEM)

---

## 1. Executive Summary

In the face of ever-growing digital infrastructure, national security agencies are inundated with vast streams of log data from a multitude of systems. The critical challenge lies in distinguishing genuine threats from benign background noise. This project details the development of a **Lightweight Security Information and Event Management (SIEM) system**. This system is designed to provide a powerful, focused solution for log aggregation, normalization, and automated threat detection. The core value of this SIEM lies in its ability to create a centralized analytical platform, dramatically enhancing threat visibility and accelerating incident response capabilities.

## 2. Project Objectives

This project will deliver a functional SIEM with the following core capabilities:

1.  **Centralized Log Collection:** To implement a robust ingestion pipeline capable of receiving and processing log data from diverse, real-time sources across a network.
2.  **Data Normalization:** To develop a parsing engine that transforms raw, inconsistent log entries into a standardized, structured format, making the data uniformly analyzable.
3.  **Threat Detection Engine:** To build a flexible, rule-based correlation engine that analyzes the normalized event stream to identify complex patterns indicative of security threats.
4.  **Actionable Alerting:** To generate clear, concise, and context-rich alerts upon the detection of a threat, providing security analysts with the immediate information needed to act.
5.  **Comprehensive Documentation:** To produce clear documentation detailing the system's architecture, operational procedures, and setup, ensuring its usability and extensibility.

## 3. Proposed Technical Approach

The system will be developed using a modern, efficient, and flexible technical stack to ensure project feasibility and promote rapid development.

- **Core Language:** Python 3 will serve as the primary development language, selected for its powerful data processing libraries and extensive support for network protocols.
- **Log Ingestion:** The system will feature a configurable network listener, such as a syslog-compatible server, designed to be the primary interface for log-generating devices and applications.
- **Dynamic Rule Engine:** To ensure adaptability, correlation rules will be externalized into a human-readable configuration file. This allows threat intelligence to be updated without modifying the application's source code.
- **Standardized Data Handling:** The project will leverage universal data formats like JSON for all normalized logs and alerts, guaranteeing interoperability and simplifying integration with other tools.

## 4. Proposed High-Level Architecture

The system's design is founded on a modular architecture, which separates core functions into distinct, interoperable components for improved maintainability and scalability.

1.  **Ingestion Pipeline:** This module is the system's front door, responsible for listening for, receiving, and queuing raw log data from all monitored sources.
2.  **Parsing & Normalization Engine:** This component acts as the universal translator, taking varied raw log formats from the pipeline and transforming them into the system's single, consistent event structure.
3.  **Correlation & Analysis Core:** This is the brain of the SIEM. It continuously analyzes the stream of normalized events, applying the defined rule set to detect suspicious patterns, multi-stage attacks, and policy violations.
4.  **Alerting & Reporting Framework:** When the correlation core identifies an incident, this module is triggered to format and dispatch detailed alerts to a predefined destination, such as a dedicated log file or the system console.

## 5. Development Methodology

The project will be developed using an iterative and modular approach, ensuring flexibility and consistent progress. This methodology prioritizes building a functional core and then expanding upon it with more advanced features.

-   **Modular Implementation:** Following the proposed architecture, each core component (Ingestion, Parsing, Correlation, Alerting) will be developed and unit-tested independently. This allows for a clear separation of concerns and facilitates parallel development efforts.

-   **Iterative Refinement:** Development will proceed in cycles. An initial iteration will focus on establishing a basic, end-to-end data pipeline. Subsequent cycles will add layers of complexity, such as support for new log formats, more sophisticated correlation rules, and enhanced alerting mechanisms.

-   **Continuous Integration:** As individual modules reach maturity, they will be continuously integrated and tested together. This ensures that the overall system remains stable and functional throughout the development lifecycle, preventing major integration challenges.

## 6. Key Deliverables

Upon project completion, Group 41 will provide the following:

1.  The complete and fully commented **source code** for the Lightweight SIEM.
2.  A configuration file containing a set of effective sample **detection rules**.
3.  This **`README.md`** file, serving as the official project and architectural documentation.
4.  A **final project summary and live presentation** demonstrating the system's features and capabilities.
