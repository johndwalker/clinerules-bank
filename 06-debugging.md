# DEBUGGING
Below debugging routine is for persistent errors or incomplete fixes. So use this routine only when stuck.

## DIAGNOSE
- Gather all error messages, logs, and behavioral symptoms
- Add relevant context from files
- Retrieve relevant project architecture, plan and current working task as specified in @memory.mdc 

- Whenever you fail with any test result, always add more context using [DIAGNOSE](#diagnose) and debug the issue effectively first, then when you have complete information move towards a fix. 
- Explain your OBSERVATIONS and then give your REASONINGS to explain why this is EXACTLY the issue and not anything else. 
- If you aren't sure, first get more OBSERVATIONS by adding more [DIAGNOSE](#diagnose) context to the issue so you exactly and specifically know what's wrong. Additionally you can seek [CLARIFICATION](./05-coding-best-practices#clarification) if required.
- Understand architecture using [ANALYZE CODE](./05-coding-best-practices#step-1-analyze-code) relevant to the issue.
- Use the sequentialthinking mcp tool to think of all possible causes like architectural misalignment, design flaw rather than just a bug, etc.
- Look for similar patterns already solved elsewhere in the codebase in  @error-documentation.md and [WEB USE](./05-coding-best-practices#web-use) if needed.
- Present your fix using [REASONING PRESENTATION](./04-project-management#presentation) for validation.
- Start modifying code to update and fix things using [SYSTEMATIC CODE PROTOCOL](./05-coding-best-practices#systematic-code-protocol) and [TESTING](./05-coding-best-practices#testing).
