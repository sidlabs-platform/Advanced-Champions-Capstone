# Advanced Champions Programme – Hands-on Lab

## Project: Agentic Engineering Learning Hub

### Business Scenario

Your organisation wants to create an internal **Learning Management Portal for software engineers**.

The platform will help developers discover and learn modern engineering practices, with an initial focus on:

- GitHub
- GitHub Copilot
- Agentic Engineering
- Agentic SDLC
- AI-assisted software development
- CI/CD and DevSecOps

The organisation expects the platform to grow over time. Your goal in this session is therefore not only to build a working application, but also to create a foundation that can be extended with additional capabilities in future sessions.

---

# 1. User Personas

The initial application should support two primary personas.

### Learner

A learner should be able to:

- Discover available courses
- Search and filter courses
- View course details
- Enrol in courses
- Navigate through course modules and lessons
- Mark lessons as completed
- Track learning progress
- Resume courses already started
- View completed courses
- View their overall learning dashboard

### Administrator

An administrator should eventually be able to manage the learning catalogue.

For the initial version, focus primarily on the learner experience. Your architecture should, however, allow administrative capabilities to be introduced later.

---

# 2. Course Catalogue

Create a catalogue containing courses across at least two learning categories.

### Agentic Engineering

Example courses:

- Introduction to Agentic Engineering
- Agentic SDLC Fundamentals
- Designing AI Agents
- MCP Fundamentals
- Building Agentic Workflows
- Agent Evaluation and Observability

### GitHub

Example courses:

- GitHub Fundamentals
- GitHub Copilot Fundamentals
- Advanced GitHub Copilot
- GitHub Actions and CI/CD
- GitHub Advanced Security
- GitHub Enterprise Fundamentals

You may create additional courses if required.

Each course should contain appropriate metadata, including:

- Course name
- Description
- Category
- Difficulty level
- Estimated learning duration
- Instructor
- Modules
- Lessons
- Course status

Use realistic sample data for the catalogue.

---

# 3. Learning Portal Home Page

Create a modern landing page for the Learning Hub.

The page should help users quickly understand:

- What the platform provides
- Available learning areas
- Featured courses
- Popular or recommended courses
- Courses they are currently learning

The application should provide clear navigation to the course catalogue and the learner's dashboard.

---

# 4. Course Discovery

Users should be able to browse the complete course catalogue.

Provide capabilities to:

- Search courses
- Filter courses by category
- Filter courses by difficulty
- Sort courses
- View relevant course information before opening a course

Course cards should provide enough information for learners to decide whether they want to explore the course.

---

# 5. Course Details

Selecting a course should open a detailed course page.

The page should display:

- Course title
- Description
- Category
- Difficulty
- Estimated duration
- Instructor
- Modules and lessons
- Learner's current progress, where applicable

Users who are not enrolled should be able to enrol in the course.

Users who are already enrolled should be able to continue learning.

---

# 6. Course Enrolment

A learner should be able to enrol in any available course.

Consider appropriate application behaviour for scenarios such as:

- A learner trying to enrol twice
- A course that is unavailable
- Enrolment failing unexpectedly
- A learner returning to an existing enrolment

The learner's enrolled courses should appear on their dashboard.

---

# 7. Course Modules and Lessons

A course consists of multiple modules.

Each module can contain multiple lessons.

For example:

**Agentic SDLC Fundamentals**

1. Introduction to Agentic Engineering
2. Understanding AI Agents
3. Agentic SDLC
4. Tools and Context
5. Human-in-the-Loop Systems
6. Agent Evaluation
7. Final Assessment

Learners should be able to navigate through the learning material and mark lessons as completed.

The system should remember their progress.

---

# 8. Learning Progress

The platform should track learning progress at multiple levels.

For example:

- Lesson completed
- Module progress
- Course progress
- Overall learner progress

Course progress should be visible as a percentage or equivalent visual representation.

Consider edge cases such as:

- Courses containing no lessons
- Newly enrolled courses
- Previously completed courses
- Changes to course content after a learner has started

---

# 9. Learner Dashboard

Create a personalised dashboard that provides a consolidated view of the learner's activity.

The dashboard should include information such as:

### Continue Learning
Courses currently in progress.

### My Courses
Courses in which the learner is enrolled.

### Completed Learning
Courses already completed.

### Learning Progress
Useful indicators showing the learner's overall learning journey.

### Recommended Learning
Courses that may be relevant to the learner.

For this version, recommendations do **not** need to use AI. A simple rules-based approach is sufficient.

---

# 10. Assessments

Courses should support basic assessments or quizzes.

At minimum, consider:

- Multiple-choice questions
- Answers
- Correct answer
- Learner submission
- Score
- Pass/fail status

A learner should be able to complete an assessment and see the result.

Design this capability so that more intelligent assessment experiences could be added later.

---

# 11. Badges and Course Completion

A learner completing a course should receive appropriate recognition.

Design a basic mechanism for:

- Course completion
- Completion status
- Achievement/badge
- Completion date

A learner should be able to see their achievements from the dashboard.

---

# 12. Backend Services

The application should expose appropriate APIs to support the user experience.

Consider APIs covering areas such as:

- Courses
- Course details
- Users
- Enrolments
- Modules
- Lessons
- Progress
- Assessments
- Dashboard information

Do not create APIs simply because they are listed above.

**Design the APIs based on your application's architecture and requirements.**

---

# 13. Data Persistence

Application information should persist between sessions.

Consider appropriate data models for:

- Users
- Courses
- Modules
- Lessons
- Enrolments
- Progress
- Assessments
- Achievements

Choose an appropriate persistence technology for your solution.

---

# 14. Application Quality

The application should not only work on the happy path.

Consider:

- Input validation
- Error handling
- Logging
- Loading states
- Empty states
- Invalid requests
- Duplicate operations
- Boundary conditions
- Maintainability
- Accessibility
- Responsive user experience

---

# 15. Testing

Create automated tests for important application behaviour.

Testing should cover appropriate areas such as:

- Business logic
- API behaviour
- Validation
- Progress calculations
- Duplicate enrolment
- Course completion
- Assessment scoring
- Error scenarios
- Edge cases

Do not optimise for the number of tests.

Optimise for meaningful coverage of important behaviour.

---

# 16. Documentation

The repository should contain sufficient documentation for another developer to understand and work with the application.

At minimum, document:

- Application purpose
- Architecture
- Technology choices
- Project structure
- Setup instructions
- Running the application
- Running tests
- Major design decisions
- Known limitations

---

# 17. Engineering Expectations

Treat this as an application intended to evolve beyond today's lab.

Your solution should therefore demonstrate:

- Clear separation of concerns
- Maintainable code
- Reusable components
- Appropriate error handling
- Secure coding practices
- Automated testing
- Consistent coding standards
- Good documentation

Avoid unnecessarily complex architecture.

---

# Important: Future Requirements

This application will continue to evolve during subsequent Advanced Champions sessions.

Future requirements may include capabilities such as:

- AI-powered course recommendations
- Conversational learning assistant
- Personalised learning paths
- Automatic quiz generation
- Agentic workflows
- Specialised AI agents
- External tools and services
- Enterprise authentication and authorisation
- Security controls
- Automated code review
- CI/CD
- Additional observability
- Production deployment

**You do not need to implement these capabilities in this session.**

However, avoid architectural decisions that make future enhancement unnecessarily difficult.

---

# Your Challenge

You have deliberately **not** been given:

- A programming language
- A frontend framework
- A backend framework
- A database technology
- A detailed architecture
- API definitions
- Complete UI designs
- Database schemas
- Complete acceptance criteria

These are engineering decisions your team needs to make.

Use **GitHub Copilot as your AI engineering partner** throughout the exercise.

Do not immediately ask Copilot to:

> "Build the entire application."

Instead, think like an engineering team.

### Recommended working approach

**Understand → Clarify → Plan → Design → Implement → Test → Review → Improve**

Use Copilot to help you:

1. Analyse the requirements
2. Identify ambiguity and missing requirements
3. Make reasonable assumptions
4. Design the solution
5. Break the work into manageable tasks
6. Implement incrementally
7. Test continuously
8. Review generated code
9. Refactor where necessary
10. Document your engineering decisions

You remain responsible for the architecture, implementation decisions and quality of the final solution.

---

# Session 1 Definition of Done

By the end of the exercise, demonstrate a working **Learning Hub MVP** providing the core learner journey:

**Discover Course → View Course → Enrol → Learn → Complete Lessons → Track Progress → Complete Course**

The solution should include:

- Working user interface
- Course catalogue
- Course search/filtering
- Course details
- Course enrolment
- Modules and lessons
- Progress tracking
- Learner dashboard
- Basic assessment capability
- Persistent data
- Backend/API layer
- Automated tests
- Error handling and validation
- Repository documentation

Most importantly:

**Keep your repository.**

This application will evolve throughout the Advanced Champions Programme.

Today's objective is not to create the final application.

Today's objective is to create a **strong engineering foundation that future sessions can progressively make more intelligent, agentic, secure and production-ready.**
