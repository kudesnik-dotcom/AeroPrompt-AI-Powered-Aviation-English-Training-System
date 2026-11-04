# AeroPrompt: AI-Powered Aviation English Training System

An LLM-based training framework designed to help aviation professionals improve their English language skills through structured exercises, technical communication scenarios, and personalized assessment.

## Overview

AeroPrompt transforms general-purpose Large Language Models (LLMs) into specialized Aviation English tutors for pilots, aircraft maintenance engineers, and technical personnel.

The system combines structured prompt engineering with aviation-specific reference materials to create a guided learning environment. It focuses on practical language skills required in aviation operations and maintenance communication.

The project was developed during my internship at **Aeroflot Technics (2026)**.

## Key Features

- **Source-Grounded Learning:** Prompts instruct the LLM to rely on uploaded reference documents rather than introduce unsupported grammar rules or technical terminology.
- **Adaptive Training:** Exercise difficulty can be adjusted according to the learner's performance.
- **Diagnostic Assessment:** A 30-question assessment identifies vocabulary, grammar, and language production weaknesses.
- **Realistic Simulations:** Interactive scenarios reproduce technical fault reporting and professional communication situations.
- **Structured Feedback:** Learners receive explanations, corrections, progress summaries, and targeted exercises.
- **Progress Tracking:** A diagnostic assessment can be repeated after four weeks to evaluate progress.

## System Architecture

The training framework consists of three interconnected components:

### 1. Grammar Training

A structured grammar course covering six major areas:

- Nouns
- Articles
- Prepositions
- Adjectives
- Adverbs
- Verbs, including tenses, modal verbs, and passive voice

Grammar exercises use aviation-related examples and scenarios.

### 2. Aviation Terminology Glossary

A reference glossary containing approximately 550 terms across 15 aircraft systems, along with technical communication expressions and maintenance-related terminology.

It covers areas such as:

- Aircraft structure
- Hydraulic and pneumatic systems
- Landing gear
- Electrical systems
- Flight instruments
- Navigation and communication
- Power plant and APU
- Fuel systems
- Aircraft maintenance
- Technical anomalies

### 3. AI Prompt System

The core of the project is a collection of nine structured prompts: one master prompt and eight specialized training modes.

| Prompt | Training Mode | Purpose |
|---|---|---|
| 0 | Master Prompt | Configures the AI tutor and establishes training rules |
| 1 | Vocabulary Flashcards | Reinforces aviation terminology |
| 2 | Grammar Training | Practices grammar through aviation-related exercises |
| 3 | Fault Reporting Simulation | Simulates reporting technical failures |
| 4 | Crew Communication Simulation | Practices professional aviation dialogues |
| 5 | Diagnostic Assessment | Evaluates the learner's current level and identifies weaknesses |
| 6 | Maintenance Task Orders | Practices understanding and communicating maintenance instructions |
| 7 | Technical Parameters | Trains learners to describe values, compare parameters, and interpret technical information |
| 8 | Error Review | Identifies recurring mistakes and generates targeted exercises |

## How It Works

The recommended learning workflow follows a structured sequence:

1. Upload the required grammar and glossary reference documents to an LLM workspace.
2. Initialize the training environment using the Master Prompt.
3. Complete the diagnostic assessment to identify knowledge gaps.
4. Practice vocabulary and grammar using specialized training modes.
5. Participate in interactive technical communication simulations.
6. Review recurring mistakes and complete targeted exercises.
7. Repeat the diagnostic assessment after four weeks to evaluate progress.

## Prompt Engineering Approach

The system incorporates several instruction-design principles:

- **Document Grounding:** Restricting generated exercises and explanations to uploaded reference materials.
- **Instruction Constraints:** Preventing the model from providing answers before the learner attempts an exercise.
- **Contextual Learning:** Using realistic aviation maintenance and operational scenarios.
- **Adaptive Difficulty:** Adjusting exercise complexity based on learner performance.
- **Evaluation Framework:** Providing structured feedback and rubric-based assessment.

These constraints are designed to reduce unsupported information and keep training aligned with the supplied materials. They do not guarantee that an LLM will never generate inaccurate information.

## Supported LLM Platforms

The prompts are designed for use with general-purpose LLM platforms, including:

- ChatGPT
- Claude
- Grok

Platform functionality and output quality may vary.

## Project Documentation

The accompanying training manual provides:

- The recommended learning workflow
- Grammar course structure
- Aviation terminology reference overview
- Complete prompt collection
- Instructions for configuring an LLM workspace

## Author

**Pavel Apikov**

Developed during an internship at Aeroflot Technics, 2026.

Areas of interest: Data Analytics, LLM Prompt Engineering, AI Systems, and Aviation.

[LinkedIn](https://linkedin.com/in/apikov-paul) | [GitHub](https://github.com/kudesnik-dotcom)

## Disclaimer

This project is an educational training framework. It is not an official ICAO examination preparation or certification system and does not replace approved aviation training, official technical documentation, or professional instruction.

The system relies on user-provided reference materials. AI-generated content should be independently verified before being used in any operational aviation context.

## Repository Structure

AeroPrompt/
│
├── README.md
├── THIRD_PARTY_MATERIALS.md
│
├── prompts/
│   ├── 00_master_prompt.md
│   ├── 01_vocabulary_flashcards.md
│   ├── 02_grammar_training.md
│   ├── 03_fault_reporting_simulation.md
│   ├── 04_crew_communication.md
│   ├── 05_diagnostic_assessment.md
│   ├── 06_maintenance_task_orders.md
│   ├── 07_technical_parameters.md
│   └── 08_error_review.md
│
└── docs/
    └── system_overview.md
