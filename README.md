# Study_Assistant
A Multi-Agent Study Assistant that uses coordinated agents to generate study plans, quizzes, and flashcards while tracking user progress and session history.
**Smart AI Study Assistant**

*Overview*

The Smart AI Study Assistant is a multi-agent system designed to help students efficiently plan their study schedules, generate quizzes, and review material using flashcards. By leveraging coordinated agents, the system automates key tasks in exam preparation and tracks learning progress over time, providing a structured and interactive study experience.

**Problem Statement **
Students often struggle to organize study plans, retain information, and prepare effectively for exams. Managing multiple subjects, deadlines, and revision sessions can be overwhelming, making it difficult to study efficiently. A smart assistant that automates planning, creates quizzes, and tracks progress can save time, improve learning outcomes, and reduce stress.

**Why Agents?**

The study workflow naturally splits into specialized tasks: understanding study goals, creating a schedule, generating practice content, and scheduling reviews. Agents allow each task to be handled independently while a Coordinator Agent orchestrates the workflow. This mirrors real-world enterprise systems and provides modular, scalable automation.


**The Smart AI Study Assistant consists of:

GoalAgent — analyzes study goals, topics, and deadlines from student input.

PlannerAgent — generates a structured daily study schedule.

QuizAgent — produces quizzes for practice.

ReviewAgent — schedules flashcards and spaced repetition reviews.

Coordinator Agent — orchestrate  the agents, manages sessions, stores progress, and returns a unified response.

The system uses SessionService and MemoryBank to maintain session history and track student progress over time.

**Demo**

When a student requests help, e.g., “I have a math final in 10 days, help me study derivatives,” the assistant:

GoalAgent identifies the topic and urgency.

PlannerAgent generates a study plan.

QuizAgent creates practice questions.

ReviewAgent schedules flashcards.

Coordinator combines all outputs into a single JSON response.

All external integrations are mocked, so the system runs safely offline.

**The Build**

Language: Python

Tools: MockLLM, SessionService, MemoryBank, ProgressStore, logging, metrics

Architecture: Modular multi-agent system with a Coordinator

Extensible: Agents can be replaced with real LLMs for advanced deployment


