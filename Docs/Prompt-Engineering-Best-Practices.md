# Prompt Engineering Best Practices

## 🎯 Tổng quan

Prompt Engineering là nghệ thuật và khoa học thiết kế các instruction hiệu quả cho AI models. Dựa trên nghiên cứu từ 20+ prompt chất lượng cao, chúng ta đã xác định được các nguyên tắc cốt lõi để tạo ra prompt hiệu quả.

## 🏗️ Cấu trúc Prompt Hiệu quả

### 1. Identity & Role Definition
```xml
<identity>
You are [ROLE], [DESCRIPTION OF CAPABILITIES AND EXPERTISE].
Your primary goal is to [MAIN OBJECTIVE].
</identity>
```

**Ví dụ:**
```xml
<identity>
You are Cursor Agent, a powerful agentic AI coding assistant powered by Claude 3.7 Sonnet. 
You operate exclusively in Cursor, the world's best IDE.
Your primary goal is to help users solve coding tasks through pair programming.
</identity>
```

### 2. Core Guidelines
```xml
<guidelines>
- [FUNDAMENTAL PRINCIPLE 1]
- [FUNDAMENTAL PRINCIPLE 2] 
- [BEHAVIORAL RULE 1]
- [BEHAVIORAL RULE 2]
</guidelines>
```

### 3. Tool Usage Instructions
```xml
<tool_usage>
You have access to the following tools:
1. [TOOL_NAME]: [DESCRIPTION AND WHEN TO USE]
2. [TOOL_NAME]: [DESCRIPTION AND WHEN TO USE]

Rules:
- ALWAYS [CRITICAL RULE]
- NEVER [FORBIDDEN ACTION]
</tool_usage>
```

### 4. Workflow Definition
```xml
<workflow>
1. [STEP 1]: [DESCRIPTION]
2. [STEP 2]: [DESCRIPTION]
3. [STEP 3]: [DESCRIPTION]
</workflow>
```

## 🎨 Kỹ thuật viết Prompt

### 1. Sử dụng XML Tags để Structure
- **Tại sao**: Tạo ra cấu trúc rõ ràng, dễ parse và maintain
- **Cách dùng**: Wrap các sections khác nhau trong XML tags
- **Ví dụ**: `<identity>`, `<guidelines>`, `<examples>`

### 2. CAPS để Nhấn mạnh
- **ALWAYS**, **NEVER**, **CRITICAL**, **IMPORTANT**
- Sử dụng sparingly để tránh "shouting"
- Chỉ dùng cho những điểm thực sự quan trọng

### 3. DO/DON'T Examples
```markdown
**DO:**
- Use semantic search before making changes
- Wait for user confirmation after each action

**DON'T:**
- Make assumptions about user intent
- Proceed without gathering necessary context
```

### 4. Progressive Complexity
- Bắt đầu với basic concepts
- Gradually introduce advanced techniques
- Provide examples at each level

## 🛡️ Safety-First Approach

### 1. Data Protection
```xml
<security>
- NEVER expose sensitive information
- Always validate user permissions
- Implement proper error handling
</security>
```

### 2. Graceful Degradation
- Handle edge cases gracefully
- Provide fallback options
- Clear error messages

### 3. User Consent
- Ask for permission before destructive actions
- Explain potential consequences
- Provide undo mechanisms where possible

## 🔄 Workflow Patterns

### 1. Information Gathering First
```
1. Understand the request
2. Gather necessary context
3. Plan the approach
4. Execute with confirmation
5. Verify results
```

### 2. Parallel Processing
- Use parallel tool calls when possible
- Batch independent operations
- Optimize for efficiency

### 3. Iterative Refinement
- Start with basic implementation
- Gather feedback
- Iterate and improve
- Test thoroughly

## 📝 Communication Guidelines

### 1. Clear and Concise
- Use simple, direct language
- Avoid unnecessary jargon
- Be specific about actions

### 2. User-Centric
- Focus on user needs
- Provide helpful explanations
- Anticipate questions

### 3. Professional Tone
- Maintain consistency
- Be helpful but not overly casual
- Show expertise through actions

## 🎯 Specialized Patterns

### 1. Chain of Thought
```xml
<thinking>
Let me think through this step by step:
1. [ANALYSIS]
2. [REASONING]
3. [CONCLUSION]
</thinking>
```

### 2. Mode Switching
- **PLAN MODE**: For strategy and analysis
- **ACT MODE**: For execution and implementation
- Clear transitions between modes

### 3. Task Management
- Break complex tasks into subtasks
- Track progress systematically
- Update status regularly

## ⚡ Performance Optimization

### 1. Efficient Tool Usage
- Choose the right tool for each task
- Minimize redundant operations
- Use batch operations when possible

### 2. Context Management
- Keep relevant information accessible
- Remove outdated context
- Prioritize important information

### 3. Response Optimization
- Be concise but complete
- Structure responses clearly
- Use appropriate formatting

## 🔍 Quality Assurance

### 1. Testing Strategies
- Test with various inputs
- Verify edge cases
- Check error handling

### 2. Validation Methods
- Cross-reference with examples
- Verify against requirements
- Get user feedback

### 3. Continuous Improvement
- Monitor performance metrics
- Collect user feedback
- Iterate based on learnings

---

*Tiếp theo: [Prompt Structure Templates](./Prompt-Structure-Templates.md)*
