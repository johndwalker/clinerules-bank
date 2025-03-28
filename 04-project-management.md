# Project Management

## Planning

When prompted to plan a new feature, follow these steps:
- Analyze all relevant code files thoroughly.
- Get any relevant context.
- Write .MD implementation plan. The plan should be written in the 'planning' directory. Structure the document to be easily parsed by yourself or another language model.
- Use the sequentialthinking mcp tool to break down the problem into key concepts and smaller sub-problems.
- Consider many ways to solve the problem.
- Set up the evaluation criterias and trade-offs to assess the merit of the solutions.
- Find the optimal solution based on the criterias and trade-offs involved.
- Feel free to [use the web](./05-coding-best-practices#web-use) as you weigh the options and perform research.
- Include a prompt near the beginning of the document that explains to yourself how to understand and execute the plan.
- Include a checklist (defined as '## Implementation Checklist') at the end with all necessary steps to complete the project in order of priority and dependency.
- As you define the checklist items, if you feel that a specific task should be split up into smaller tasks in order to follow coding best practices or simply due to the scope of the task, please act at your own discretion. These checklist items should be manageable, bite-sized chunks of work that can be accomplished in a single, short working session.
- Ensure that each task is well-defined, thouroughly detailed, and clear on how to execute it.
- As you plan, any written code must follow the Coding Best Practices.
- Follow the guidelines in [CLARIFICATION](./05-coding-best-practices#clarification).

## Presentation

When the planning is complete, provide a summary following these steps:
- Provide the PLAN with as much detail as possible. 
- Break down the solution step-by-step and think every step in through detail with clarity.
- Reason out its optimality w.r.t. other promising solutions.
- Explicitly tell all your assumptions, choices and decisions.
- Explain trade-offs in solutions.
- Restate my query in your own words if necessary after giving the solution.

## Execute the plan

When prompted to complete the next step of a specific plan, follow these steps:
- Read the plan and follow the prompt as instructed.
- However, limit your current focus to the first unfinished item in the '## Implementation Checklist', aka only accomplish that single task. If there are subtasks, only complete a single subtask. No exceptions! It is imperative that you only complete a single task.
- Please use the sequentialthinking mcp tool to plan any changes you make.
- When finished, please mark the item complete on the checklist. 
- If you determine that the next item on the checklist has already been completed, then mark it as complete and your work is finished!
- It is critical that you follow [all coding best practices](./05-coding-best-practices.md) as you execute the plan.
- Before implementing, validate the plan's solution.
