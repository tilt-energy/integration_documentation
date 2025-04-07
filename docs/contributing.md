# Contributing to Tilt Integration Documentation

We welcome contributions to improve our integration documentation. This guide will help you get started with contributing.

## How to Contribute

1. **Fork the Repository**
   - Click the "Fork" button on the top right of this repository
   - Clone your forked repository to your local machine

2. **Create a Feature Branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make Your Changes**
   - Follow our documentation style guide
   - Ensure all links are working
   - Test your changes locally using MkDocs

4. **Commit Your Changes**
   Follow our conventional commit format:
   ```bash
   git commit -m "type(scope): description"
   ```
   
   Where:
   - `type` is one of:
     - `feat`: A new feature
     - `fix`: A bug fix
     - `docs`: Documentation changes
     - `style`: Changes that do not affect the meaning of the code (formatting, etc.)
     - `refactor`: A code change that neither fixes a bug nor adds a feature
     - `test`: Adding missing tests or correcting existing tests
     - `chore`: Changes to the build process or auxiliary tools
   - `scope` is optional and indicates the part of the codebase affected
   - `description` is a brief summary of the changes

   Examples:
   ```bash
   git commit -m "docs(api): add authentication section"
   git commit -m "feat(terminology): add new BMS terms"
   git commit -m "fix(links): correct broken documentation links"
   ```

5. **Push to Your Fork**
   ```bash
   git push origin feature/your-feature-name
   ```

6. **Create a Pull Request**
   - Go to the original repository
   - Click "New Pull Request"
   - Select your feature branch
   - Provide a clear description of your changes

## Documentation Style Guide

- Use clear, concise language
- Follow the existing structure and formatting
- Include examples where helpful
- Keep technical terms consistent with our terminology
- Use proper Markdown formatting

## Local Development

To test your changes locally:

1. Install MkDocs:
```bash
pip install mkdocs mkdocs-material mkdocs-redoc-tag
```

2. Run the development server:
```bash
mkdocs serve
```

3. View your changes at `http://127.0.0.1:8000`

## Questions?

If you have questions about contributing:

- Check the existing documentation
- Contact our integration support team: [integration-support@tilt-energy.com](mailto:integration-support@tilt-energy.com)