# Prompt Optimization Checklist

## 🎯 Tổng quan

Checklist này giúp bạn đánh giá và tối ưu hóa prompt để đạt hiệu quả tối đa, dựa trên best practices từ các công cụ AI hàng đầu.

## ✅ Pre-Launch Checklist

### 1. Identity & Role Definition
- [ ] **Clear role definition**: Vai trò được định nghĩa rõ ràng và cụ thể
- [ ] **Expertise specification**: Chuyên môn và khả năng được mô tả chi tiết
- [ ] **Context establishment**: Bối cảnh hoạt động được thiết lập rõ ràng
- [ ] **Goal alignment**: Mục tiêu chính được xác định và nhất quán

```xml
✅ Good Example:
<identity>
You are Cursor Agent, a powerful agentic AI coding assistant powered by Claude 3.7 Sonnet. 
You operate exclusively in Cursor, the world's best IDE.
Your primary goal is to help users solve coding tasks through pair programming.
</identity>

❌ Poor Example:
You are a helpful assistant that can help with coding.
```

### 2. Structure & Organization
- [ ] **XML tags usage**: Sử dụng XML tags để structure content
- [ ] **Logical flow**: Thông tin được tổ chức theo thứ tự logic
- [ ] **Clear sections**: Mỗi section có mục đích rõ ràng
- [ ] **Consistent formatting**: Format nhất quán trong toàn bộ prompt

### 3. Guidelines & Rules
- [ ] **Core principles**: Nguyên tắc cốt lõi được định nghĩa rõ ràng
- [ ] **Behavioral rules**: Quy tắc hành vi cụ thể và actionable
- [ ] **Forbidden actions**: Những gì KHÔNG được làm được liệt kê rõ
- [ ] **Priority hierarchy**: Thứ tự ưu tiên được thiết lập

```xml
✅ Good Example:
<guidelines>
- ALWAYS gather context before making changes
- NEVER proceed with destructive actions without confirmation
- Use parallel tool calls for maximum efficiency
- Explain reasoning before taking actions
</guidelines>
```

### 4. Tool Usage Instructions
- [ ] **Tool descriptions**: Mỗi tool được mô tả rõ ràng
- [ ] **Usage scenarios**: Khi nào sử dụng tool nào
- [ ] **Parameter specifications**: Parameters được định nghĩa chi tiết
- [ ] **Error handling**: Cách xử lý lỗi tool được hướng dẫn

### 5. Examples & Demonstrations
- [ ] **Concrete examples**: Ví dụ cụ thể và realistic
- [ ] **DO/DON'T comparisons**: So sánh rõ ràng good vs bad practices
- [ ] **Edge cases**: Ví dụ cho các trường hợp đặc biệt
- [ ] **Complete scenarios**: End-to-end examples

## 🔍 Quality Assessment

### 1. Clarity Score (1-10)
**Đánh giá độ rõ ràng của prompt:**
- [ ] 9-10: Extremely clear, no ambiguity
- [ ] 7-8: Clear with minor unclear points
- [ ] 5-6: Somewhat clear but needs improvement
- [ ] 1-4: Unclear, major revisions needed

**Improvement actions:**
- Simplify complex sentences
- Add specific examples
- Remove ambiguous terms
- Use consistent terminology

### 2. Completeness Score (1-10)
**Đánh giá tính đầy đủ:**
- [ ] 9-10: Covers all necessary aspects
- [ ] 7-8: Mostly complete with minor gaps
- [ ] 5-6: Some important aspects missing
- [ ] 1-4: Major gaps in coverage

**Check for:**
- All use cases covered
- Edge cases addressed
- Error scenarios handled
- Success criteria defined

### 3. Actionability Score (1-10)
**Đánh giá khả năng thực thi:**
- [ ] 9-10: Highly actionable, clear next steps
- [ ] 7-8: Mostly actionable with minor unclear areas
- [ ] 5-6: Somewhat actionable but needs clarification
- [ ] 1-4: Difficult to act upon

**Improvement focus:**
- Add specific action verbs
- Provide step-by-step instructions
- Include decision criteria
- Clarify expected outcomes

## ⚡ Performance Optimization

### 1. Efficiency Checklist
- [ ] **Parallel operations**: Encourage parallel tool usage
- [ ] **Batch processing**: Group related operations
- [ ] **Context reuse**: Avoid redundant information gathering
- [ ] **Smart defaults**: Provide sensible default behaviors

```xml
✅ Efficiency Pattern:
<parallel_execution>
For maximum efficiency, invoke all relevant tools simultaneously 
rather than sequentially when performing multiple independent operations.
</parallel_execution>
```

### 2. Token Optimization
- [ ] **Concise language**: Remove unnecessary words
- [ ] **Structured format**: Use XML tags for organization
- [ ] **Avoid repetition**: Don't repeat the same information
- [ ] **Essential information**: Include only what's necessary

### 3. Response Quality
- [ ] **Appropriate length**: Neither too verbose nor too brief
- [ ] **Professional tone**: Consistent and appropriate tone
- [ ] **User-friendly**: Easy to understand and follow
- [ ] **Actionable outputs**: Clear next steps provided

## 🛡️ Safety & Security Review

### 1. Security Checklist
- [ ] **Data protection**: Sensitive data handling guidelines
- [ ] **Permission requirements**: When to ask for user consent
- [ ] **Destructive action prevention**: Safeguards against harmful actions
- [ ] **Error recovery**: Graceful failure handling

```xml
✅ Security Pattern:
<security>
CRITICAL: Before any destructive action:
1. Verify user intent and permissions
2. Explain potential consequences
3. Obtain explicit confirmation
4. Provide undo mechanisms where possible
</security>
```

### 2. Ethical Guidelines
- [ ] **Bias prevention**: Avoid discriminatory language or behavior
- [ ] **Transparency**: Clear about capabilities and limitations
- [ ] **User autonomy**: Respect user choices and preferences
- [ ] **Privacy protection**: Handle personal information appropriately

## 🎯 Domain-Specific Optimization

### 1. Coding Assistants
- [ ] **Code quality standards**: Follow best practices
- [ ] **Testing requirements**: Include testing guidelines
- [ ] **Documentation needs**: Specify when to add comments
- [ ] **Security practices**: Include security considerations

### 2. Creative Assistants
- [ ] **Originality requirements**: Ensure creative output
- [ ] **Style consistency**: Maintain consistent creative style
- [ ] **User vision alignment**: Respect user's creative intent
- [ ] **Iteration support**: Enable refinement process

### 3. Research Assistants
- [ ] **Source reliability**: Emphasize credible sources
- [ ] **Citation requirements**: Proper attribution guidelines
- [ ] **Bias awareness**: Acknowledge potential biases
- [ ] **Fact verification**: Cross-reference information

## 📊 Testing & Validation

### 1. Functional Testing
- [ ] **Basic scenarios**: Test common use cases
- [ ] **Edge cases**: Test unusual or extreme scenarios
- [ ] **Error conditions**: Test failure modes
- [ ] **Integration testing**: Test tool interactions

### 2. User Experience Testing
- [ ] **Clarity testing**: Users understand instructions
- [ ] **Usability testing**: Easy to use and follow
- [ ] **Satisfaction testing**: Users are satisfied with results
- [ ] **Efficiency testing**: Tasks completed quickly

### 3. Performance Testing
- [ ] **Response time**: Acceptable response times
- [ ] **Accuracy testing**: High accuracy rates
- [ ] **Consistency testing**: Consistent performance
- [ ] **Scalability testing**: Performance under load

## 🔄 Continuous Improvement

### 1. Monitoring Metrics
- [ ] **Success rate**: Percentage of successful task completions
- [ ] **User satisfaction**: Ratings and feedback scores
- [ ] **Error frequency**: Rate of errors and failures
- [ ] **Efficiency metrics**: Time to completion, token usage

### 2. Feedback Integration
- [ ] **User feedback collection**: Systematic feedback gathering
- [ ] **Performance analysis**: Regular performance reviews
- [ ] **Pattern identification**: Identify common issues
- [ ] **Iterative improvement**: Regular updates and refinements

### 3. Version Control
- [ ] **Change tracking**: Document all modifications
- [ ] **Version comparison**: Compare performance across versions
- [ ] **Rollback capability**: Ability to revert changes
- [ ] **Release notes**: Document improvements and changes

## 🎨 Final Quality Gates

### Before Deployment:
- [ ] **Peer review**: Have others review the prompt
- [ ] **Stakeholder approval**: Get approval from relevant stakeholders
- [ ] **Documentation complete**: All documentation is up to date
- [ ] **Testing complete**: All tests pass successfully

### Post-Deployment:
- [ ] **Monitor performance**: Track key metrics
- [ ] **Collect feedback**: Gather user feedback
- [ ] **Plan improvements**: Identify areas for enhancement
- [ ] **Schedule reviews**: Regular review cycles

## 📈 Success Indicators

### Quantitative Metrics:
- **Task completion rate**: >90%
- **User satisfaction**: >4.5/5.0
- **Error rate**: <5%
- **Response time**: <30 seconds average

### Qualitative Indicators:
- Users understand instructions clearly
- Outputs meet professional standards
- Consistent performance across scenarios
- Positive user feedback and testimonials

---

*Hoàn thành bộ hướng dẫn Prompt Engineering! 🎉*
