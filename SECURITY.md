# Security Policy

## Reporting a Vulnerability

If you discover a security vulnerability in this project, please follow the steps below:

1. **Do not open a public issue**: Please do not disclose security vulnerabilities publicly. We prefer to address issues privately first to prevent misuse.
2. **Contact us privately**: 
   - Send an email to [jermainealedare@gmail.com] You can also reach us through GitHub issues by tagging the repository maintainers directly.
3. **Provide details**: In your report, please include as much information as possible, including:
   - Description of the vulnerability
   - Steps to reproduce (if applicable)
   - Any other relevant information such as logs, screenshots, or proof-of-concept code.

We will investigate and respond as soon as possible.

## Security Best Practices

We encourage all contributors and users to follow security best practices to ensure that this project remains secure:

### 1. **Sensitive Information**:
   - **API Keys**: Ensure that sensitive information like API keys (e.g., Gemini API keys) are **never hardcoded** into the source code. Use environment variables or configuration files that are excluded from version control (e.g., `.env` files).
   - If you are contributing to this project, please ensure no sensitive data (e.g., passwords, API keys, tokens) is pushed to the repository.

### 2. **Dependencies**:
   - Ensure that all third-party libraries and dependencies are up to date. Regularly check for security patches for libraries and dependencies used in this project.
   - Use a tool like `pip-audit` to regularly check for vulnerabilities in dependencies.

### 3. **Data Storage**:
   - The flashcards data is saved in a local JSON file (`flashcards.json`). This file should not be used to store sensitive user information. Be cautious about the type of data stored and always sanitize user inputs.

### 4. **Code Review**:
   - All pull requests should be thoroughly reviewed for potential security flaws.
   - Avoid using unsafe functions or insecure coding patterns that could lead to vulnerabilities.

### 5. **Authentication & Authorization**:
   - This project does not include an authentication mechanism. If you plan to expand this project and add user authentication, ensure that best practices for handling passwords and sensitive data are followed (e.g., hashing passwords before storing them).

## Mitigation of Common Vulnerabilities

This section outlines common vulnerabilities to be mindful of and how they should be mitigated:

### 1. **Injection Attacks**:
   - Always sanitize and validate user inputs. Although this app does not directly interact with databases, you should still sanitize any user-generated content to avoid any potential for injection attacks.

### 2. **Cross-Site Scripting (XSS)**:
   - If expanding the app to use web technologies, ensure proper escaping of user inputs to avoid XSS vulnerabilities.

### 3. **Denial of Service (DoS)**:
   - Ensure that the app handles errors gracefully. Implement appropriate error handling to prevent the app from crashing due to invalid input or API failures.

### 4. **Access Control**:
   - Since this app does not have complex user roles or authentication, ensure that no unauthorized access to sensitive data can occur.

## Secure Deployment

If you are deploying this app to a server, ensure that the server is secured by following these steps:

- Always use HTTPS to encrypt communication between clients and the server.
- Regularly update the server and apply security patches.
- Ensure proper file permissions and access controls on the server.

## License

By submitting security-related patches or reporting vulnerabilities, you agree to allow the project maintainers to use, modify, or share your submission according to the project's [LICENSE](LICENSE) file.

