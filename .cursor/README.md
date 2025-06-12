# Cursor Configuration

This directory contains MDC-formatted project rules that guide AI assistant behavior for the Ingenius project, following the latest [Cursor rules format](https://docs.cursor.com/context/rules).

## Rule Files (MDC Format)

### Core Rules (Always Applied)
- **`project-context.mdc`** 
  - Defines Ingenius mission and business context
  - Mission-critical operational requirements
  - Core principles for all development

- **`ugenie-style-guide.mdc`** 
  - Organization-wide coding standards from main ugenie project
  - UI component standards and layout guidelines
  - Performance, security, and accessibility requirements
  - Ensures consistency across all ugenie.ai projects

### Auto-Attached Rules (Context-Sensitive)
- **`typescript-standards.mdc`** - Applied when working with `.ts`/`.tsx` files
  - TypeScript strict mode requirements
  - Code quality standards
  - React TypeScript patterns

- **`dashboard-ui.mdc`** - Applied when working with components and app files
  - UI/UX standards for enterprise dashboards
  - Accessibility requirements
  - Design system guidelines

### On-Demand Rules
- **`git-workflow.mdc`** - Git and commit standards
- **`operational-efficiency.mdc`** - Operational workflow optimization focus

## Rule Types Used

- **Always**: Applied to all AI interactions (`alwaysApply: true`)
- **Auto Attached**: Triggered by file patterns (`globs: ["**/*.tsx"]`)
- **Agent Requested**: Available for AI to invoke when relevant
- **Manual**: Explicitly referenced with `@ruleName`

## Legacy Files

- **Root `.cursorrules`** - Legacy format, maintained for backward compatibility but deprecated per [Cursor documentation](https://docs.cursor.com/context/rules)

## Benefits

This structure provides:
- **Focused, composable rules** rather than monolithic configuration
- **Context-aware guidance** that activates based on file types
- **Consistent development patterns** across the team
- **Mission-critical operational focus** for ugenie.ai requirements
- **Modern MDC format** with proper metadata and descriptions
- **Organization-wide consistency** with main ugenie project standards

## Usage

Rules are automatically applied by Cursor based on their type and context. You can also:
- View active rules in Cursor Settings > Rules
- Manually reference rules with `@ruleName` syntax
- Generate new rules using `/Generate Cursor Rules` command

## Customization

Update individual `.mdc` files as the project evolves, keeping focus on operational efficiency and code maintainability. 