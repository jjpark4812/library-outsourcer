---
name: library-outsourcer
description: Evaluates whether open-source libraries or tools can improve coding outputs (quality, efficiency, and performance) compared to building or maintaining from scratch. Use when planning new features, optimizing existing ones, evaluating library options, or looking for tools to offload work.
---

**Execute phase-by-phase.** 

## PHASE 1: QUESTION THE USER

- Relentlessly inquire about every aspect of the user's desired outcome. 
  - If a question can be answered by exploring the codebase, do so instead.
- Ask one question at a time, providing answer options for each.
  - Each option should walk down a different design branch towards the desired outcome.
  - Recommend the answer most effective at achieving that goal.
    - Concisely present reasoning behind every recommendation.
- Address any question or concern that the user may express BEFORE proceeding to the next question.
  - Fully resolve the current question before proceeding to the next.
- Only proceed to the next phase once you have a clear understanding of the user's desired outcome and a shared vision with the user.

## PHASE 2: SCOPE THE TASK

- Based on the user's desired outcome, explore the relevant codebase to understand the scope of the task. 
  - Identify the specific components, functionalities, and dependencies relevant to the task. 
- Only proceed to the next phase once you have a clear understanding of the scope of the task.

## PHASE 3: ASSESS THE VIABILITY OF LIBRARY OUTSOURCING

- Critically identify risks and tradeoffs of building from scratch instead of using a library.
- Determine whether or not leveraging an existing open-source library will:
  1. produce a cleaner, higher-quality outcome. 
  2. better serve the project's central purpose and design.
  3. introduce avoidable risks and complications.

### CREATIVE INTEGRATION PRINCIPLES:
  - **Consider CREATIVE ways to leverage libraries.**
  - **DO NOT only think about the implementation in isolation, but also how it can interact with other project libraries and components to unlock hidden value.**
  - **Consider hybrid approaches where the task can be completed partly from scratch (E.g. middlewares, intermediary components, etc.) and partly with library implementation to create unexpected synergy.**

- Only proceed to the next phase upon determining that library outsourcing is viable. If it is not, end this skill and proceed with the task without leveraging a library.

## PHASE 4: IDENTIFY RELEVANT AND RELIABLE LIBRARIES

- Identify RELEVANT and RELIABLE open-source libraries that will enhance the outcome of the task.
  - If necessary, use web search to find candidates.
- **Prioritize adherence to the project's central purpose and design when selecting libraries.**
- ONLY select libraries that:
  1. will provide substantial value to the project.
  2. WILL NOT introduce security vulnerabilities, technical debt, or maintenance issues.

## PHASE 5: PRESENT THE SELECTION

- Present each selected library in order of most impactful to the user's desired outcome, to least.
- For each selected library: 
  - CLEARLY outline why it better serves the project than building from scratch. 
  - Transparently present risks of implementation compared to building from scratch.
- Identify (where applicable) whether libraries should: 
  1. DEFINITELY be implemented.
  2. PROBABLY be implemented.
  3. POSSIBLY be implemented.
- Identify where libraries and components will conflict or synergize with each other.
- Provide reasoning for each judgment, and address any question or concern that the user may express.
- Await user approval on which libraries to implement or not before proceeding to the next phase.
- If the user rejects all library options, end this skill and proceed with the task without leveraging a library.

## PHASE 6: CREATE AN IMPLEMENTATION PLAN

- Based on the "### CREATIVE INTEGRATION PRINCIPLES", create a detailed implementation plan for the user-approved selection, outlining how they will be integrated into the project to achieve the user's desired outcome.
  - Plan so that synergistic libraries and components are implemented together if that will maximize value, output quality, and efficiency. 
- Review the implementation plan to ensure that it will not introduce avoidable security vulnerabilities, technical debt, or maintenance issues.

---