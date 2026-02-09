# 🎯 Vibe Coding with Cursor: A Complete Guide

A systematic approach to building projects with AI-assisted development using Cursor IDE. This methodology breaks down project development into clear, manageable phases with optimized prompts for each stage.

## 📋 Table of Contents

- [What is Vibe Coding?](#what-is-vibe-coding)
- [Development Phases](#development-phases)
- [Phase-Specific Prompts](#phase-specific-prompts)
- [Best Practices](#best-practices)
- [Examples](#examples)
- [Tips & Tricks](#tips--tricks)

---

## 🌟 What is Vibe Coding?

Vibe Coding is a structured approach to AI-assisted development that emphasizes:

- **Clear Communication**: Using precise, context-rich prompts
- **Iterative Development**: Building in phases with validation
- **AI Collaboration**: Leveraging Cursor's AI to handle boilerplate and implementation details
- **Quality Assurance**: Validating at each step before moving forward

This methodology works for any project type: web apps, APIs, mobile apps, CLIs, data pipelines, and more.

---

## 🔄 Development Phases

### Phase 1: Discovery & Planning
**Goal**: Define what you're building and create a solid foundation

### Phase 2: Architecture Design
**Goal**: Design the technical structure and components

### Phase 3: Validation & Review
**Goal**: Verify the plan before implementation

### Phase 4: Implementation
**Goal**: Build the actual project

### Phase 5: Testing & Refinement
**Goal**: Ensure quality and fix issues

### Phase 6: Documentation
**Goal**: Create comprehensive documentation

---

## 💬 Phase-Specific Prompts

### 🎯 Phase 1: Discovery & Planning Prompt

```
I want to build [PROJECT DESCRIPTION]. 

Context:
- Purpose: [What problem does this solve?]
- Target Users: [Who will use this?]
- Key Features: [List 3-5 main features]
- Constraints: [Any technical/business constraints?]
- Success Criteria: [What makes this successful?]

Please help me:
1. Refine the project scope and identify any unclear requirements
2. Suggest the most suitable tech stack and tools
3. Identify potential challenges or risks
4. Create a high-level project roadmap with milestones
5. Recommend best practices for this type of project

Format the response as a structured project brief that I can reference throughout development.
```

**Example Output**: Project brief with scope, tech stack, risks, and roadmap

---

### 🏗️ Phase 2: Architecture Design Prompt

```
Based on our project brief, design the technical architecture for [PROJECT NAME].

Requirements:
- Tech Stack: [List from Phase 1]
- Scale: [Expected users/load]
- Integration Needs: [APIs, services, databases]

Please provide:
1. Directory structure with explanation for each folder
2. Data models and schemas
3. API endpoints or key interfaces
4. Component hierarchy (for frontend projects)
5. External dependencies and services
6. Environment variables and configuration needed
7. Architecture diagram in ASCII or description

Focus on:
- Scalability and maintainability
- Clear separation of concerns
- Best practices for [tech stack]
```

**Example Output**: Complete architecture blueprint ready for implementation

---

### ✅ Phase 3: Validation & Review Prompt

```
Review the following project plan and architecture for potential issues:

[Paste your project brief and architecture]

Please analyze:
1. Completeness: Are there any missing components or considerations?
2. Feasibility: Are there any unrealistic or overly complex parts?
3. Best Practices: Does it follow industry standards for [tech stack]?
4. Potential Issues: What could go wrong and how to mitigate?
5. Optimization: Any suggestions for improvement?
6. Security: Are there security considerations we should address?

Provide specific, actionable feedback.
```

**Example Output**: Comprehensive review with improvement suggestions

---

### 🔨 Phase 4: Implementation Prompts

#### 4.1 Initial Setup
```
Set up the initial project structure for [PROJECT NAME] using [TECH STACK].

Include:
1. Initialize the project with proper configuration
2. Create the directory structure we designed
3. Set up development dependencies and tools
4. Create configuration files (.env.example, config files, etc.)
5. Add initial README with setup instructions
6. Set up linting, formatting, and pre-commit hooks (if applicable)

Use best practices and latest stable versions.
```

#### 4.2 Feature Implementation
```
Implement [FEATURE NAME] for [PROJECT NAME].

Context:
- Purpose: [What this feature does]
- User Story: As a [user type], I want to [action] so that [benefit]
- Acceptance Criteria:
  * [Criterion 1]
  * [Criterion 2]
  * [Criterion 3]

Technical Requirements:
- [List specific technical requirements]
- [Integration points]
- [Data handling needs]

Please:
1. Write clean, well-documented code
2. Follow our established architecture
3. Include error handling and edge cases
4. Add inline comments for complex logic
5. Ensure code is modular and reusable

Style: Follow [coding style guide] conventions
```

#### 4.3 Database/Data Layer
```
Create the data layer for [PROJECT NAME].

Requirements:
- Database: [Type - PostgreSQL, MongoDB, etc.]
- Models: [List entities]
- Relationships: [Describe relationships]

Please create:
1. Database schema/models with proper types
2. Migration files (if applicable)
3. Seed data for development
4. Database access layer/repositories
5. Indexes for performance
6. Validation rules

Include comments explaining design decisions.
```

#### 4.4 API Development
```
Create the API endpoints for [FEATURE/MODULE].

Endpoints needed:
- [HTTP METHOD] /path - [Description]
- [HTTP METHOD] /path - [Description]

For each endpoint, include:
1. Request validation and sanitization
2. Proper HTTP status codes
3. Error handling with meaningful messages
4. Authentication/authorization (if needed)
5. Input validation
6. Response formatting
7. Rate limiting considerations (if applicable)

Follow REST/GraphQL best practices.
```

#### 4.5 Frontend Components
```
Create the [COMPONENT NAME] component for [PROJECT NAME].

Requirements:
- Framework: [React/Vue/Angular/etc.]
- Functionality: [What it does]
- Props/Inputs: [List required props]
- State Management: [How it manages state]

Please create:
1. Component structure with proper TypeScript types
2. Styling using [CSS framework/approach]
3. Event handlers and business logic
4. Loading and error states
5. Accessibility features (ARIA labels, keyboard navigation)
6. Responsive design considerations
7. Unit test structure

Follow [style guide] and component library patterns.
```

---

### 🧪 Phase 5: Testing & Refinement Prompts

#### 5.1 Test Creation
```
Create comprehensive tests for [MODULE/FEATURE].

Test Coverage Needed:
- Unit tests for [specific functions/components]
- Integration tests for [workflows]
- Edge cases and error conditions

Please create:
1. Test files following our project structure
2. Test cases covering happy path and edge cases
3. Mock data and fixtures
4. Setup and teardown procedures
5. Meaningful test descriptions
6. Aim for >80% code coverage

Use [testing framework] and follow [testing patterns].
```

#### 5.2 Bug Fix Prompt
```
There's an issue with [FEATURE/COMPONENT]:

Problem:
[Describe the bug]

Steps to Reproduce:
1. [Step 1]
2. [Step 2]
3. [Step 3]

Expected Behavior:
[What should happen]

Actual Behavior:
[What actually happens]

Context:
- Environment: [dev/staging/production]
- Browser/Platform: [if relevant]
- Error Messages: [any errors]

Please:
1. Identify the root cause
2. Provide a fix with explanation
3. Add tests to prevent regression
4. Suggest any related improvements
```

#### 5.3 Code Review & Refactoring
```
Review and refactor [FILE/MODULE] to improve:

Focus Areas:
- Code readability and maintainability
- Performance optimization
- DRY principle adherence
- Error handling
- Security best practices
- Type safety

Current Code:
[Paste code or reference file]

Please provide:
1. Specific issues identified
2. Refactored code with improvements
3. Explanation of changes made
4. Performance implications (if any)
```

---

### 📚 Phase 6: Documentation Prompts

#### 6.1 README Creation
```
Create a comprehensive README.md for [PROJECT NAME].

Include:
1. Project title and description
2. Key features
3. Tech stack
4. Prerequisites
5. Installation instructions
6. Configuration (environment variables)
7. Usage examples
8. API documentation (if applicable)
9. Project structure
10. Contributing guidelines
11. License
12. Contact/Support information

Make it beginner-friendly and well-formatted with proper sections.
```

#### 6.2 API Documentation
```
Generate API documentation for [PROJECT NAME].

For each endpoint, include:
1. Endpoint URL and HTTP method
2. Description of functionality
3. Authentication requirements
4. Request parameters (path, query, body)
5. Request example
6. Response format
7. Response examples (success and error)
8. Possible error codes
9. Rate limiting info

Format: [Markdown/OpenAPI/Swagger]
```

#### 6.3 Code Documentation
```
Add comprehensive documentation to [FILE/MODULE].

Please add:
1. File-level documentation explaining purpose
2. Function/method documentation with:
   - Purpose
   - Parameters with types
   - Return value
   - Examples
   - Exceptions/errors
3. Complex logic explanations
4. Type definitions documentation
5. Usage examples for public APIs

Follow [JSDoc/PyDoc/etc.] standards.
```

---

## ✨ Best Practices

### 1. **Context is King**
Always provide relevant context in your prompts:
- What you're building
- Tech stack being used
- Coding standards to follow
- Constraints or requirements

### 2. **Iterate, Don't Generate Everything**
Build incrementally:
- Start with structure, then add features
- Validate each component before moving on
- Refactor as you go

### 3. **Be Specific About Requirements**
Instead of: "Create a login form"
Use: "Create a React login form component with email/password fields, client-side validation, loading states, error handling, and remember me checkbox. Use Tailwind CSS and follow our design system."

### 4. **Use Cursor Features Effectively**
- **Cmd/Ctrl + K**: For inline edits and quick changes
- **Cmd/Ctrl + L**: For chat-based development and planning
- **@-mentions**: Reference specific files in your prompts
- **Composer**: For multi-file changes

### 5. **Maintain Prompt History**
Keep a log of successful prompts for similar future tasks

### 6. **Review Before Accepting**
Always review AI-generated code:
- Check for security issues
- Verify error handling
- Ensure it follows your patterns
- Test thoroughly

### 7. **Provide Feedback**
If the output isn't right:
- Be specific about what needs changing
- Provide examples of desired output
- Reference existing code patterns

---

## 📖 Examples

### Example 1: Building a Todo App

**Phase 1 - Planning**
```
I want to build a modern todo application.

Context:
- Purpose: Help users manage daily tasks with a clean, intuitive interface
- Target Users: Individuals looking for a simple task manager
- Key Features: 
  * Add/edit/delete tasks
  * Mark tasks complete
  * Filter by status
  * Persist data locally
- Constraints: Must work offline, no backend required
- Success Criteria: Fast, responsive, works on mobile and desktop

[Use Planning Prompt template above]
```

**Phase 4 - Implementation**
```
Create the Task component for our todo app.

Requirements:
- Framework: React with TypeScript
- Functionality: Display task with checkbox, edit/delete buttons
- Props: task object, onToggle, onDelete, onEdit functions
- State: Edit mode toggle

[Follow Frontend Component prompt template]
```

---

### Example 2: Building a REST API

**Phase 2 - Architecture**
```
Design the architecture for a blog API.

Requirements:
- Tech Stack: Node.js, Express, PostgreSQL, JWT auth
- Scale: Small to medium (1000s of users)
- Integration: Need to integrate with cloud storage for images

[Follow Architecture Design prompt]
```

**Phase 4 - API Implementation**
```
Create the blog posts API endpoints.

Endpoints needed:
- GET /api/posts - List all posts with pagination
- GET /api/posts/:id - Get single post
- POST /api/posts - Create new post (auth required)
- PUT /api/posts/:id - Update post (auth required)
- DELETE /api/posts/:id - Delete post (auth required)

[Follow API Development prompt]
```

---

## 💡 Tips & Tricks

### 🎯 Prompt Engineering Tips

1. **Start Broad, Then Narrow**
   - First: Get the big picture and architecture
   - Then: Dive into specific implementations

2. **Use Examples**
   - Show examples of similar code you like
   - Reference existing patterns in your codebase

3. **Specify Output Format**
   - "Return as JSON"
   - "Use TypeScript interfaces"
   - "Follow our coding style guide"

4. **Chain Prompts**
   - Use output from one prompt as input for the next
   - Build complexity gradually

### 🔧 Cursor-Specific Tips

1. **Use @ Commands**
   ```
   @filename.ts - Reference specific files
   @docs - Search documentation
   @folder - Reference entire directories
   @web - Search the web for solutions
   ```

2. **Composer Mode**
   - Use for changes spanning multiple files
   - Great for refactoring
   - Can implement entire features

3. **Inline Editing**
   - Select code + Cmd/Ctrl+K for quick edits
   - Great for small tweaks and fixes

4. **Context Management**
   - Keep relevant files open
   - Use .cursorignore to exclude unnecessary files
   - Pin important conversations

### 🚀 Workflow Optimization

1. **Morning Planning Session**
   - Start day with planning prompts
   - Get architecture decisions done early
   - Set clear goals for the day

2. **Batch Similar Tasks**
   - Create all models at once
   - Write all API endpoints together
   - Generate tests in batches

3. **Regular Refactoring**
   - Don't let tech debt accumulate
   - Refactor weekly with AI assistance
   - Keep code quality high

4. **Document as You Go**
   - Use documentation prompts immediately after implementation
   - Don't leave docs for the end
   - Update README with each major feature

---

## 🎓 Learning Resources

### Deepen Your Vibe Coding Skills

- **Cursor Documentation**: https://cursor.sh/docs
- **Prompt Engineering Guide**: https://www.promptingguide.ai/
- **Clean Code Principles**: Review before each project
- **Your Tech Stack Docs**: Always reference official documentation

---

## 🤝 Contributing

Found a better prompt pattern? Have suggestions?
- Open an issue
- Submit a pull request
- Share your successful prompts

---

## 📄 License

This guide is open source. Use it, modify it, share it.

---

## 🙏 Credits

Created by developers who believe AI is a tool for enhancing, not replacing, software craftsmanship.

---

**Happy Vibe Coding! 🚀**

Remember: AI is your pair programmer, not a magic wand. Good prompts + your expertise = amazing results.
