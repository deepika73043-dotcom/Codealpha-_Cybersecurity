
# Secure Coding Review
## CodeAlpha Cyber Security Internship

### Objective
To identify common security weaknesses and recommend secure coding practices.

### Finding 1: Hardcoded Credentials
Passwords and secret keys should not be written directly in source code because they may be exposed when code is shared.

Recommendation: Use environment variables or a secrets manager.

### Finding 2: Plain-Text Password Storage
Storing passwords in plain text creates a serious security risk if the database is exposed.

Recommendation: Use a suitable password-hashing algorithm such as Argon2id or bcrypt.

### Finding 3: Input Validation
Unvalidated input can cause unexpected application behavior and security issues.

Recommendation: Validate input and handle errors safely.

### Security Best Practices
- Never commit passwords, API keys, or other secrets.
- Use secure authentication methods.
- Keep libraries and dependencies updated.
- Review code before deployment.
- Use security analysis tools where available.

### Conclusion
Secure coding practices help reduce vulnerabilities and protect sensitive information.

### Scope and Limitation
This is an educational review of common security weaknesses. It is not a complete audit of a production application.
