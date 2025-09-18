# Advanced Prompt Techniques

## 🧠 Chain of Thought Prompting

### 1. Thinking Tags Pattern
```xml
<thinking>
Let me analyze this step by step:
1. [PROBLEM ANALYSIS]
2. [APPROACH CONSIDERATION] 
3. [SOLUTION PLANNING]
4. [POTENTIAL CHALLENGES]
5. [FINAL DECISION]
</thinking>
```

**Ví dụ từ Devin AI:**
```xml
<think>
Before critical git Github-related decisions such as deciding what branch to branch off, 
what branch to check out, whether to make a new PR or update an existing one, 
I need to think through:
1. Current repository state
2. User's intended workflow
3. Best practices for the specific scenario
4. Potential conflicts or issues
</think>
```

### 2. Progressive Reasoning
```xml
<analysis>
Initial Assessment: [FIRST IMPRESSION]
Deeper Analysis: [DETAILED EXAMINATION]
Alternative Approaches: [OTHER OPTIONS]
Risk Assessment: [POTENTIAL ISSUES]
Recommendation: [FINAL CHOICE WITH REASONING]
</analysis>
```

## 🔧 Advanced Tool Usage Patterns

### 1. Parallel Tool Execution
```xml
<parallel_execution>
For maximum efficiency, whenever you perform multiple independent operations, 
invoke all relevant tools simultaneously rather than sequentially.

Example:
- Reading multiple files: Use 3 parallel read_file calls
- Running multiple commands: Batch them in a single execution
- Searching different directories: Execute searches in parallel
</parallel_execution>
```

**Implementation từ Augment Code:**
```xml
<use_parallel_tool_calls>
For maximum efficiency, whenever you perform multiple independent operations, 
invoke all relevant tools simultaneously rather than sequentially. 
Prioritize calling tools in parallel whenever possible.
</use_parallel_tool_calls>
```

### 2. Tool Selection Strategy
```xml
<tool_selection>
Before using any tool:
1. Assess what information you already have
2. Determine what additional information is needed
3. Choose the most appropriate tool for each task
4. Consider tool dependencies and execution order
5. Optimize for efficiency and accuracy
</tool_selection>
```

### 3. Error Recovery Patterns
```xml
<error_handling>
When tool execution fails:
1. Analyze the error message
2. Determine root cause
3. Try alternative approaches
4. If stuck after 3 attempts, ask user for help
5. Document lessons learned
</error_handling>
```

## 📋 Task Management Techniques

### 1. Hierarchical Task Breakdown
```xml
<task_management>
For complex projects:
1. Break into 3-7 milestone-level tasks
2. Each task should take ~20 minutes for a professional
3. Avoid micro-tasks or overly granular steps
4. Use clear, actionable task names
5. Track progress systematically

Task States:
- [ ] NOT_STARTED
- [/] IN_PROGRESS  
- [x] COMPLETE
- [-] CANCELLED
</task_management>
```

**Pattern từ v0:**
```xml
<TodoManager>
Core workflow:
1. set_tasks - Break project into 3-7 milestone tasks
2. move_to_task - Complete current work, focus on next task
3. generate_plan - Create detailed technical architecture plan

Guidelines:
• Milestone-level tasks - "Build Homepage", "Setup Auth"
• One page = one task
• UI before backend
• ≤10 tasks total
• NO vague tasks like "Polish", "Test", "Finalize"
</TodoManager>
```

### 2. Progress Tracking
```xml
<progress_tracking>
Update task states efficiently:
- Use batch updates when possible
- Mark previous task complete and next task in progress simultaneously
- If user feedback indicates issues, update task back to IN_PROGRESS
- Provide regular status updates to user
</progress_tracking>
```

## 🎯 Mode-Based Operation

### 1. Plan vs Act Modes
```xml
<mode_switching>
PLAN MODE:
- Focus on understanding and strategy
- Gather information and context
- Ask clarifying questions
- Create detailed implementation plans
- Use planning tools to organize thoughts

ACT MODE:
- Execute the established plan
- Use tools to implement solutions
- Make code changes and modifications
- Provide progress updates
- Verify results and completion
</mode_switching>
```

**Implementation từ Cline:**
```xml
<plan_mode_respond>
In PLAN MODE, your job is to gather all information needed to fulfill the task.
- Search and understand the codebase
- Ask questions for clarification
- Architect a solution
- Brainstorm ideas with the user
- Create a detailed plan before switching to ACT MODE
</plan_mode_respond>
```

### 2. Context Switching
```xml
<context_management>
When switching between modes or tasks:
1. Save current context and progress
2. Load relevant context for new task
3. Maintain continuity of important information
4. Clear outdated or irrelevant context
5. Establish new working parameters
</context_management>
```

## 🔍 Information Gathering Strategies

### 1. Comprehensive Context Collection
```xml
<context_gathering>
Before making any changes:
1. Check existing context first
2. Use semantic search for understanding
3. Read relevant files completely
4. Understand dependencies and relationships
5. Gather all necessary information before acting

NEVER guess or make assumptions - always verify with tools.
</context_gathering>
```

### 2. Intelligent Search Patterns
```xml
<search_strategy>
Search Hierarchy:
1. Semantic search for high-level understanding
2. Grep search for specific patterns
3. File listing for structure exploration
4. Code definition search for relationships

Combine multiple search strategies for comprehensive coverage.
</search_strategy>
```

## 🛡️ Safety and Validation Techniques

### 1. Pre-Action Validation
```xml
<validation_framework>
Before any potentially destructive action:
1. Verify user intent and permissions
2. Check for potential side effects
3. Validate input parameters
4. Confirm with user if uncertain
5. Provide undo mechanisms where possible

NEVER proceed with destructive actions without explicit confirmation.
</validation_framework>
```

### 2. Graceful Degradation
```xml
<graceful_degradation>
When encountering limitations or errors:
1. Acknowledge the limitation clearly
2. Provide alternative approaches
3. Explain what can and cannot be done
4. Offer partial solutions if applicable
5. Guide user toward viable alternatives
</graceful_degradation>
```

## 🎨 Creative Problem Solving

### 1. Multi-Perspective Analysis
```xml
<perspective_analysis>
Approach problems from multiple angles:
1. Technical feasibility
2. User experience impact
3. Performance implications
4. Security considerations
5. Maintenance requirements
6. Future scalability

Consider trade-offs and optimize for the most important factors.
</perspective_analysis>
```

### 2. Iterative Refinement
```xml
<iterative_approach>
For complex solutions:
1. Start with minimal viable implementation
2. Test and gather feedback
3. Identify improvement opportunities
4. Implement enhancements incrementally
5. Validate each iteration
6. Document lessons learned
</iterative_approach>
```

## 📊 Performance Optimization

### 1. Efficiency Patterns
```xml
<efficiency_optimization>
Maximize performance by:
- Batching independent operations
- Reusing computed results
- Minimizing redundant tool calls
- Optimizing context usage
- Streamlining workflows
- Eliminating unnecessary steps
</efficiency_optimization>
```

### 2. Resource Management
```xml
<resource_management>
Manage computational resources:
- Monitor token usage
- Optimize prompt length
- Cache frequently used information
- Prioritize critical operations
- Balance speed vs accuracy
</resource_management>
```

## 🔄 Adaptive Behavior

### 1. Learning from Feedback
```xml
<adaptive_learning>
Continuously improve by:
- Analyzing user feedback
- Identifying common patterns
- Adjusting strategies based on outcomes
- Refining approaches over time
- Building knowledge base of solutions
</adaptive_learning>
```

### 2. Context-Aware Adaptation
```xml
<context_adaptation>
Adapt behavior based on:
- User expertise level
- Project complexity
- Time constraints
- Quality requirements
- Available resources
- Environmental factors
</context_adaptation>
```

---

*Tiếp theo: [Prompt Examples and Case Studies](./Prompt-Examples-and-Case-Studies.md)*
