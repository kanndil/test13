# Contributing to test13

Thank you for your interest in contributing to test13! This document provides guidelines and information for contributors.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [How to Contribute](#how-to-contribute)
- [Development Workflow](#development-workflow)
- [Coding Standards](#coding-standards)
- [Testing](#testing)
- [Documentation](#documentation)
- [Submitting Changes](#submitting-changes)
- [Issue Reporting](#issue-reporting)
- [Community](#community)

## Code of Conduct

By participating in this project, you agree to abide by our Code of Conduct. Please be respectful and constructive in all interactions.

### Our Standards

- Use welcoming and inclusive language
- Be respectful of differing viewpoints and experiences
- Gracefully accept constructive criticism
- Focus on what is best for the community
- Show empathy towards other community members

## Getting Started

### Prerequisites

Before contributing, ensure you have:

- Git installed and configured
- A GitHub account
- Basic understanding of the project structure
- Familiarity with the technologies used in this project

### Setting Up Your Development Environment

1. **Fork the repository** on GitHub
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/YOUR_USERNAME/test13.git
   cd test13
   ```
3. **Add the upstream remote**:
   ```bash
   git remote add upstream https://github.com/kanndil/test13.git
   ```
4. **Create a new branch** for your feature:
   ```bash
   git checkout -b feature/your-feature-name
   ```

## How to Contribute

### Types of Contributions

We welcome various types of contributions:

- **Bug fixes** - Help us identify and fix issues
- **Feature enhancements** - Add new functionality
- **Documentation improvements** - Help make our docs better
- **Code refactoring** - Improve code quality and maintainability
- **Testing** - Add or improve test coverage
- **Examples** - Provide usage examples and tutorials

### Before You Start

1. **Check existing issues** to see if your idea is already being discussed
2. **Open an issue** to discuss major changes before implementing them
3. **Search existing pull requests** to avoid duplicate work

## Development Workflow

### Branch Naming Convention

Use descriptive branch names with prefixes:

- `feature/` - New features (e.g., `feature/add-user-authentication`)
- `bugfix/` - Bug fixes (e.g., `bugfix/fix-login-error`)
- `docs/` - Documentation updates (e.g., `docs/update-api-guide`)
- `refactor/` - Code refactoring (e.g., `refactor/optimize-database-queries`)
- `test/` - Test additions/improvements (e.g., `test/add-unit-tests`)

### Keeping Your Fork Updated

Regularly sync your fork with the upstream repository:

```bash
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
```

## Coding Standards

### General Guidelines

- Write clear, readable, and maintainable code
- Follow existing code style and conventions
- Use meaningful variable and function names
- Add comments for complex logic
- Keep functions small and focused on a single responsibility

### Code Formatting

- Use consistent indentation (spaces or tabs, but be consistent)
- Follow language-specific style guides
- Remove trailing whitespace
- End files with a newline character

### Commit Messages

Write clear and descriptive commit messages:

```
type(scope): brief description

Longer description if necessary, explaining what changed and why.

- Use bullet points for multiple changes
- Reference issues with #issue-number
- Keep the first line under 50 characters
- Use present tense ("Add feature" not "Added feature")
```

**Types:**
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes (formatting, etc.)
- `refactor`: Code refactoring
- `test`: Adding or updating tests
- `chore`: Maintenance tasks

**Example:**
```
feat(auth): add user login functionality

Implement user authentication system with email/password login.
Includes input validation, password hashing, and session management.

- Add login form component
- Implement authentication middleware
- Add user session handling
- Update database schema

Fixes #123
```

## Testing

### Running Tests

Before submitting your changes, ensure all tests pass:

```bash
# Run all tests
npm test

# Run specific test suite
npm test -- --grep "feature-name"

# Run tests with coverage
npm run test:coverage
```

### Writing Tests

- Write tests for new features and bug fixes
- Ensure good test coverage for critical functionality
- Use descriptive test names that explain what is being tested
- Follow the existing test structure and patterns

### Test Guidelines

- **Unit tests** - Test individual functions/components in isolation
- **Integration tests** - Test how different parts work together
- **End-to-end tests** - Test complete user workflows

## Documentation

### Documentation Standards

- Keep documentation up-to-date with code changes
- Use clear and concise language
- Include code examples where appropriate
- Follow the existing documentation structure

### Types of Documentation

- **README.md** - Project overview and quick start guide
- **API documentation** - Detailed API reference
- **Tutorials** - Step-by-step guides for common tasks
- **Code comments** - Inline documentation for complex logic

## Submitting Changes

### Pull Request Process

1. **Ensure your branch is up-to-date** with the main branch
2. **Run all tests** and ensure they pass
3. **Update documentation** if necessary
4. **Create a pull request** with a clear title and description

### Pull Request Template

When creating a pull request, include:

```markdown
## Description
Brief description of the changes made.

## Type of Change
- [ ] Bug fix (non-breaking change which fixes an issue)
- [ ] New feature (non-breaking change which adds functionality)
- [ ] Breaking change (fix or feature that would cause existing functionality to not work as expected)
- [ ] Documentation update

## Testing
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] New and existing unit tests pass locally with my changes
- [ ] I have tested this change manually

## Checklist
- [ ] My code follows the style guidelines of this project
- [ ] I have performed a self-review of my own code
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] My changes generate no new warnings

## Related Issues
Fixes #(issue number)
```

### Review Process

- All pull requests require review before merging
- Address feedback promptly and professionally
- Be open to suggestions and improvements
- Update your PR based on review comments

## Issue Reporting

### Before Reporting an Issue

1. **Search existing issues** to avoid duplicates
2. **Check the documentation** for solutions
3. **Try the latest version** to see if the issue is already fixed

### Creating a Good Issue Report

Include the following information:

- **Clear title** that summarizes the issue
- **Detailed description** of the problem
- **Steps to reproduce** the issue
- **Expected behavior** vs actual behavior
- **Environment information** (OS, browser, version, etc.)
- **Screenshots or code samples** if applicable

### Issue Templates

#### Bug Report
```markdown
**Describe the bug**
A clear and concise description of what the bug is.

**To Reproduce**
Steps to reproduce the behavior:
1. Go to '...'
2. Click on '....'
3. Scroll down to '....'
4. See error

**Expected behavior**
A clear and concise description of what you expected to happen.

**Screenshots**
If applicable, add screenshots to help explain your problem.

**Environment:**
- OS: [e.g. iOS]
- Browser [e.g. chrome, safari]
- Version [e.g. 22]

**Additional context**
Add any other context about the problem here.
```

#### Feature Request
```markdown
**Is your feature request related to a problem? Please describe.**
A clear and concise description of what the problem is.

**Describe the solution you'd like**
A clear and concise description of what you want to happen.

**Describe alternatives you've considered**
A clear and concise description of any alternative solutions or features you've considered.

**Additional context**
Add any other context or screenshots about the feature request here.
```

## Community

### Communication Channels

- **GitHub Issues** - For bug reports and feature requests
- **GitHub Discussions** - For general questions and community discussions
- **Pull Requests** - For code review and collaboration

### Getting Help

If you need help:

1. Check the documentation and existing issues
2. Ask questions in GitHub Discussions
3. Reach out to maintainers through GitHub

### Recognition

We appreciate all contributions! Contributors will be:

- Listed in the project's contributors section
- Mentioned in release notes for significant contributions
- Invited to join the project as a maintainer for sustained contributions

## License

By contributing to test13, you agree that your contributions will be licensed under the same license as the project.

---

Thank you for contributing to test13! Your efforts help make this project better for everyone.

*Last updated: 2025-08-20*