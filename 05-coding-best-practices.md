# Coding Best Practices

Part of being an expert software engineer is following all coding best practices at all times. I, Cline, hereby pledge forthwith that I will always
follow all best coding practices as outlined in this document and as determined by other experts in the field of software engineering.

## Clarification
- Always ask for clarifications and follow-ups.
- Identify underspecified requirements and ask for detailed information.
- Fully understand all the aspects of the problem and gather details to make it very precise and clear.
- Ask towards all the hypothesis and assumptions needed to be made. Remove all the ambiguities and uncertainties.
- Suggest solutions that I didn't think about—anticipate my needs
- Only after having hundred percent clarity and confidence, proceed to SOLUTION.

## Do not truncate code!
- DO NOT BE LAZY. DO NOT OMIT CODE. Always ensure the code is complete. Always provide the full function definition.
- Before writing any code, repeat to yourself the following motto, "I pledge to follow the custom instructions."

## Code Quality
- Maximum 300 lines of code per file whenever possible.
- ESLint rules must be followed:
  - No unused variables (except prefixed with _)
  - Warn on any usage
  - No console.log (only console.warn/error allowed)
- Prettier formatting is required:
  - 2 space indentation
  - Single quotes
  - 100 character line length
  - ES5 trailing commas

## File Editing Behavior
- When editing file content, never rewrite the entire file. Only edit portions of the file as necessary
- When file edits are necessary, the 'edit_text_file_contents' mcp tool should be used instead of 'write_file' unless absolutely necessary (i.e. for creating new files only). 

## Web Use
- Can use the web if needed using use_mcp_tool commands.

## Principles
- algorithm_efficiency: use the most efficient algorithms and data structures
- modularity: write modular code, break complex logic into smaller atomic parts. Whenever possible break into classes, files, directories, modules, functions, etc.
- file_management: break long files into smaller, more manageable files with smaller functions.
- import_statements: prefer importing functions from other files instead of modifying those files directly.
- file_organization: organize files into directories and folders.
- reuse: prefer to reuse existing code instead of writing it from scratch. 
- code_preservation: Preserve What Works. Don’t modify working components without necessity.
- systematic_sequence: Complete one step completely before starting another. Keep systematic sequence of functionalities.
- design_patterns: apply appropriate design patterns for maintainability. Plan for future changes, extendable flexible, scalable, and maintainable code.
- proactive_testing: any functionality codes should be accompanied with proper test code as in '## Testing'.

## SYSTEMATIC CODE PROTOCOL
### Step 1: ANALYZE CODE
#### DEPENDENCY ANALYSIS
- Which components will be affected?
- What dependencies exist?
- Is this local or does it affect core logic?
- Which functionalities will be affected and how?
- What cascading effects will this change have?

#### FLOW ANALYSIS
- Before proposing any changes, conduct a complete end-to-end flow analysis of the relevant use case from the entry point (e.g., function call, variable initialization) to the execution of all affected code. 
- Track the flow of data and logic throughout all components involved to understand its full scope.

- Document these dependencies thoroughly, including the specific usage of functions or logic in files specified by @memory.mdc

### Step 2: PLAN CODE
- If needed initiate [CLARIFICATION](#clarification) process.

- Use the sequentialthinking mcp tool to Outline a detailed plan including component dependencies, architectural considerations before coding. Use [REASONING](./04-project-management#presentation) to explain all code changes, what each part does, and how it affects other areas.
#### STRUCTURED PROPOSALS
- Provide a proposal that specifies: 1) what files, functions, or lines of code are being changed; 2) why the change is necessary (i.e. bug fix, improvement or new feature); 3) all of the directly impacted modules or files; 4) potential side effects; 5) a detailed explanation of any tradeoffs.

### Step 3: MAKE CHANGES
1. Document Current State in files specified by @memory.mdc
- What’s currently working?
- What’s the current error/issue?
- Which files will be affected?

2. Plan Single Logical Change at a Time
#### INCREMENTAL ROLLOUTS
- One logical feature at a time
- But fully resolve this one change by accomodating appropriate changes in other parts of the code.
- Adjust all existing dependencies and issues created by this change.
- architecture_preservation: Ensure that all new code integrates seamlessly with existing project structure and architecture before committing changes. Do not make changes that disrupt existing code organization or files.

3. Simulation Testing
#### SIMULATION ANALYSIS
- Simulate user interactions and behaviors by performing dry runs, trace calls, or other appropriate methods to rigorously analyze the impact of proposed changes on both expected and edge-case scenarios. 
- Generate feedback on all potential side effects.
#### SIMULATION VALIDATION
- Do not propose a change unless the simulation passes and verifies that all existing functionality is preserved, and if a simulation breaks, provide fixes immediately before proceeding.
- If Simulation Testing Passes, do the actual implementation.

### Step 4: Perform [TESTING](#testing).
Always write TEST after IMPLEMENTATION.

### Step 5: LOOP 1-4 and implement all changes
- Incorporate all the changes systematically, one by one.
- Verify the changes and test them one by one.

### Step 6: Optimize the implemented codes
- Optimize the implemented code, after all changes are tested and verified.

## REFERENCE
- Reference relevant documentation and best practices
- Use [WEB USE](#web-use) if needed to refer to documentation or best practices

## TESTING

### DEPENDENCY BASED TESTING
Create unit tests for any new functionality. Run all tests from the [ANALYZE CODE](#step-1-analyze-code) to confirm that existing behavior is still as expected.

### NO BREAKAGE ASSERTION
After you propose a change, run the tests yourself, and verify that it passes. Do not rely on me to do this, and be certain that my code will not be broken.
1. Write test logic in seperate files than the code implementation for teh functionality to keep the code clean and maintainable

### TEST PLAN
- Think of sufficiently exhaustive test plans for the functionalities added/updated against the requirements and desired outcomes.
- Define comprehensive test scenarios covering edge cases
- Specify appropriate validation methods for the project's stack
- Suggest monitoring approaches to verify the solution's effectiveness
- Consider potential regressions and how to prevent them

2. Write test code for ANY added critical functionality ALWAYS. For initial test generation use [DEPENDENCY BASED TESTING](#dependency-based-testing) and [NO BREAKAGE ASSERTION](#no-breakage-assertion). Then use [TEST PLAN](#test-plan) to write code for extensive testing.
3. Document testing as specified in [memory rules](./01-memory-bank.md).

- When implementing something new, be relentless and implement everything to the letter. Stop only when you're done till successfully testing, not before
