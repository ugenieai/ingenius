# Cursor Rules for Ingenius

## Project Context
Ingenius is the AI Agent Operations Command Centre for ugenie.ai - a mission-critical internal tool that integrates, automates, streamlines and handles manual startup operations tasks. This dashboard will dramatically improve operational efficiency and allow the founding team to focus on high-value strategic work.

## Technology Stack
- **Framework**: Next.js 14+ with App Router
- **Language**: TypeScript (strict mode)
- **Styling**: Tailwind CSS
- **Package Manager**: npm
- **Git**: Conventional commits preferred

## Coding Standards

### File Structure
- Use the `src/app` directory structure (App Router)
- Components go in `src/components/`
- Utilities in `src/lib/`
- Types in `src/types/`
- Constants in `src/constants/`

### Naming Conventions
- **Components**: PascalCase (e.g., `DashboardHeader.tsx`)
- **Files**: kebab-case for non-components (e.g., `api-client.ts`)
- **Variables**: camelCase
- **Constants**: UPPER_SNAKE_CASE
- **CSS Classes**: Follow Tailwind conventions

### TypeScript Guidelines
- Always use TypeScript
- Define proper interfaces and types
- Avoid `any` type
- Use strict type checking
- Export types from dedicated files when shared

### React Best Practices
- Use functional components with hooks
- Implement proper error boundaries
- Use React.memo for performance optimization when needed
- Follow React Hook rules
- Prefer composition over inheritance

## UI/UX Guidelines

### Design System
- **Colors**: Use a professional, modern palette suitable for enterprise dashboards
- **Typography**: Clean, readable fonts (Geist or similar)
- **Spacing**: Consistent spacing using Tailwind's spacing scale
- **Components**: Build reusable, accessible components
- **Responsive**: Mobile-first approach

### Dashboard Principles
- **Information Hierarchy**: Most critical operations data prominently displayed
- **Real-time Updates**: Show live system status and metrics
- **Quick Actions**: Common operations easily accessible
- **Visual Feedback**: Clear success/error states
- **Performance**: Fast loading and smooth interactions

## Development Workflow

### Code Quality
- Write clean, self-documenting code
- Add comments for complex business logic
- Use descriptive variable and function names
- Follow DRY (Don't Repeat Yourself) principles
- Implement proper error handling

### Testing
- Write unit tests for utilities and business logic
- Test components with React Testing Library
- Mock external API calls
- Test error scenarios

### Git Conventions
- Use conventional commits: `feat:`, `fix:`, `docs:`, `style:`, `refactor:`, `test:`
- Keep commits atomic and focused
- Write descriptive commit messages
- Use branches for features: `feature/dashboard-metrics`

## Operational Context

### Business Requirements
- **Efficiency**: Every feature should reduce manual work
- **Reliability**: System must be stable and dependable
- **Scalability**: Code should handle growing operational needs
- **Security**: Protect sensitive operational data
- **Usability**: Founders should easily understand and use features

### Integration Points
- Consider integration with existing ugenie.ai systems
- Plan for API connections to various operational tools
- Design for data aggregation from multiple sources
- Implement proper authentication and authorization

## AI Assistant Behavior

### When Making Changes
- Always understand the operational impact
- Prioritize user experience and efficiency  
- Consider error scenarios and edge cases
- Implement proper loading states
- Add appropriate logging for debugging

### Code Suggestions
- Favor proven patterns over experimental approaches
- Optimize for maintainability and readability
- Consider performance implications
- Suggest security best practices
- Recommend proper error handling

### Problem Solving
- Ask clarifying questions about business requirements
- Consider the end-user experience (founding team)
- Think about operational workflows
- Suggest improvements beyond the immediate request
- Document complex decisions and trade-offs

## Specific Dos and Don'ts

### ✅ DO
- Write self-documenting code
- Use TypeScript strictly
- Implement proper error boundaries
- Add loading states for async operations
- Use semantic HTML elements
- Follow accessibility guidelines
- Optimize for performance
- Test edge cases

### ❌ DON'T
- Use `any` types
- Ignore TypeScript errors
- Create overly complex abstractions
- Skip error handling
- Use inline styles instead of Tailwind
- Commit broken code
- Ignore console warnings
- Hardcode sensitive values

## Questions to Ask Yourself
1. Does this feature improve operational efficiency?
2. Is the code maintainable by the founding team?
3. Have I considered all error scenarios?
4. Is the user experience intuitive?
5. Will this scale as ugenie.ai grows?
6. Is the code properly typed and documented?
7. Have I tested the happy path and edge cases?
8. Does this align with the mission-critical nature of the tool?

---

Remember: Ingenius is not just another dashboard - it's a critical tool that will shape how ugenie.ai operates. Every decision should reflect this importance and contribute to the company's operational excellence. 