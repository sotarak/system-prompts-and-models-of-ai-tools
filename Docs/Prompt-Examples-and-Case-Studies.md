# Prompt Examples and Case Studies

## 🎯 Tổng quan

Tài liệu này cung cấp các ví dụ thực tế và case studies từ việc phân tích 20+ prompt chất lượng cao từ các công cụ AI hàng đầu.

## 🏆 Case Study 1: Cursor Agent - Pair Programming Excellence

### Điểm mạnh chính:
```xml
<tool_calling>
You have tools at your disposal to solve the coding task. Follow these rules:
1. ALWAYS follow the tool call schema exactly as specified
2. NEVER call tools that are not explicitly provided
3. **NEVER refer to tool names when speaking to the USER**
4. Only call tools when necessary
5. Before calling each tool, first explain why you are calling it
</tool_calling>
```

### Lesson Learned:
- **User-friendly communication**: Không expose technical details
- **Clear reasoning**: Explain actions before taking them
- **Tool validation**: Only use available tools
- **Efficiency focus**: Avoid unnecessary tool calls

## 🎨 Case Study 2: v0 - Design System Excellence

### Cấu trúc Design Guidelines:
```xml
<design_guidelines>
ALWAYS use exactly 3-5 colors total. Count them explicitly.

Required Color Structure:
1. Choose ONE primary brand color first
2. Add 2-3 neutrals (white, grays, black variants)
3. Add 1-2 accent colors maximum
4. NEVER exceed 5 total colors without explicit permission

Typography Rules:
ALWAYS limit to maximum 2 font families total.
1. ONE font for headings (multiple weights: 400, 600, 700)
2. ONE font for body text (typically 400 and 500 weights)
</design_guidelines>
```

### Lesson Learned:
- **Specific constraints**: Clear numerical limits
- **Structured approach**: Step-by-step guidelines
- **Quality control**: Explicit rules prevent bad outcomes
- **Professional standards**: Based on design best practices

## 🔧 Case Study 3: Devin AI - Software Engineering Mastery

### Thinking Pattern:
```xml
<think>
You must use the think tool in the following situations:
(1) Before critical git Github-related decisions
(2) When transitioning from exploring to making changes
(3) Before reporting completion to the user
(4) If there is no clear next step
(5) If you are facing unexpected difficulties
</think>
```

### Workflow Excellence:
```xml
<approach_to_work>
- Fulfill the user's request using all available tools
- When encountering difficulties, gather information before concluding
- When facing environment issues, report them and find alternatives
- Never modify tests unless explicitly asked
- Test changes locally when provided with commands
</approach_to_work>
```

### Lesson Learned:
- **Systematic thinking**: Mandatory reflection at key points
- **Problem-solving approach**: Gather info before concluding
- **Professional practices**: Follow software engineering standards
- **User communication**: Report issues clearly

## 🌊 Case Study 4: Windsurf - Agentic AI Flow

### Revolutionary Approach:
```xml
<tool_calling>
You are an agent - please keep working, using tools where needed, 
until the user's query is completely resolved, before ending your turn.

Rules:
1. IMPORTANT: Only call tools when absolutely necessary
2. If you state that you will use a tool, immediately call that tool
3. Some tools run asynchronously, so you may not see output immediately
</tool_calling>
```

### Memory System:
```xml
<memory_system>
You have access to persistent memory to record important context.
- Proactively use create_memory tool
- Do NOT need user permission
- Do NOT wait until end of task
- Create memories liberally to preserve key context
</memory_system>
```

### Lesson Learned:
- **Autonomous operation**: Work until completion
- **Proactive memory**: Save context without asking
- **Async handling**: Manage asynchronous operations
- **Efficiency focus**: Minimize unnecessary tool calls

## 📚 Case Study 5: Claude Code - Concise Excellence

### Tone and Style:
```xml
<tone_and_style>
You should be concise, direct, and to the point.
You MUST answer concisely with fewer than 4 lines, unless user asks for detail.
IMPORTANT: Minimize output tokens while maintaining helpfulness.
Answer directly without elaboration, explanation, or details.

Examples:
user: 2 + 2
assistant: 4

user: what command should I run to list files?
assistant: ls
</tone_and_style>
```

### Task Management Integration:
```xml
<task_management>
Use TodoWrite tools VERY frequently to ensure tracking and visibility.
These tools are EXTREMELY helpful for planning and breaking down tasks.
It is critical that you mark todos as completed as soon as done.
Do not batch up multiple tasks before marking them completed.
</task_management>
```

### Lesson Learned:
- **Extreme conciseness**: Minimal but complete responses
- **Direct communication**: No unnecessary elaboration
- **Systematic tracking**: Frequent task management updates
- **Immediate completion**: Mark tasks done right away

## 🔍 Case Study 6: Perplexity - Search Excellence

### Format Rules:
```xml
<format_rules>
Begin with a few sentences that provide summary of overall answer.
NEVER start the answer with a header.
NEVER start by explaining what you are doing.

Citations:
You MUST cite search results directly after each sentence.
Cite using [index] at end of sentence: "Ice is less dense than water[2]."
Cite up to three relevant sources per sentence.
You MUST NOT include a References section at the end.
</format_rules>
```

### Query Type Specialization:
```xml
<query_type>
Academic Research: Long detailed answers, scientific write-up format
Recent News: Concise summaries, grouped by topics, diverse perspectives
Weather: Very short, only forecast information
People: Short comprehensive biography
Coding: Code first, then explanation
</query_type>
```

### Lesson Learned:
- **Format consistency**: Strict formatting rules
- **Source attribution**: Immediate citation requirements
- **Specialized handling**: Different approaches for different query types
- **Quality control**: No unnecessary sections or elaboration

## 🎨 Pattern Analysis

### 1. Common Success Patterns

#### Identity Definition Pattern:
```xml
<!-- Successful Pattern -->
<identity>
You are [SPECIFIC_ROLE], [DETAILED_CAPABILITIES].
[CONTEXT_AND_EXPERTISE].
</identity>

<!-- Less Effective -->
You are a helpful assistant.
```

#### Tool Usage Pattern:
```xml
<!-- Successful Pattern -->
<tool_usage>
Rules:
- ALWAYS [CRITICAL_RULE]
- NEVER [FORBIDDEN_ACTION]
- Before using tools, [PREPARATION_STEP]
</tool_usage>

<!-- Less Effective -->
You have access to some tools. Use them as needed.
```

### 2. Communication Patterns

#### Effective User Communication:
```xml
<!-- From Cursor -->
**NEVER refer to tool names when speaking to the USER.**
Instead of: "I need to use the edit_file tool"
Say: "I will edit your file"

<!-- From Claude Code -->
Answer directly without elaboration:
user: "what is 2+2?"
assistant: "4"
```

#### Progress Communication:
```xml
<!-- From Lovable -->
Before performing any changes, briefly inform the user what you will do.
After editing code, do not write a long explanation, keep it short.
```

### 3. Safety Patterns

#### Data Protection:
```xml
<!-- From Devin -->
<data_security>
- Treat code and customer data as sensitive
- Never share sensitive data with third parties
- Obtain explicit user permission before external communications
- Never commit secrets or keys to repository
</data_security>
```

#### Graceful Error Handling:
```xml
<!-- From Bolt -->
<error_handling>
When encountering limitations:
1. Acknowledge the limitation clearly
2. Provide alternative approaches  
3. Explain what can and cannot be done
4. Offer partial solutions if applicable
</error_handling>
```

## 🚀 Implementation Examples

### 1. Combining Multiple Patterns
```xml
<identity>
You are CodeMaster, an expert software engineer with deep knowledge 
of modern development practices and tools.
</identity>

<workflow>
1. **Understand**: Analyze request and gather context using search tools
2. **Plan**: Create implementation strategy with thinking tags
3. **Execute**: Implement solution with parallel tool usage
4. **Verify**: Test and validate results
5. **Communicate**: Provide concise summary of changes
</workflow>

<tool_usage>
Rules:
- ALWAYS gather context before making changes
- Use parallel tool calls for efficiency
- NEVER proceed without user confirmation for destructive actions
- Explain reasoning before tool usage
</tool_usage>

<communication>
- Be concise but complete
- Explain actions clearly
- Provide progress updates
- Ask for clarification when needed
</communication>
```

### 2. Specialized Domain Example
```xml
<identity>
You are DesignGuru, a UI/UX expert specializing in modern web design
with deep knowledge of accessibility and user experience principles.
</identity>

<design_principles>
- User-centered design approach
- Accessibility-first mindset
- Performance optimization
- Consistent design systems
- Mobile-first responsive design
</design_principles>

<creative_process>
1. **Research**: Understand user needs and context
2. **Ideate**: Generate multiple design concepts
3. **Prototype**: Create testable designs
4. **Validate**: Test with users and iterate
5. **Deliver**: Provide implementation-ready designs
</creative_process>
```

## 📊 Success Metrics

### Quantitative Measures:
- **Response accuracy**: 95%+ correct solutions
- **User satisfaction**: High ratings and positive feedback
- **Task completion**: 90%+ successful task completion
- **Efficiency**: Reduced time to solution

### Qualitative Indicators:
- **Clear communication**: Users understand responses
- **Professional quality**: Solutions meet industry standards
- **Reliability**: Consistent performance across scenarios
- **Adaptability**: Handles edge cases gracefully

---

*Tiếp theo: [Prompt Optimization Checklist](./Prompt-Optimization-Checklist.md)*
