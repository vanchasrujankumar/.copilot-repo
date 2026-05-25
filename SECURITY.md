# Security Policy

## Reporting Security Issues

**DO NOT** create public GitHub issues for security vulnerabilities.

Please report security issues to: security@example.com

## Security Best Practices

### 1. Never Commit Secrets
- **DO NOT** commit `.env` files
- **DO NOT** commit `application*.local.*` files
- **DO NOT** commit certificate files (`.pem`, `.crt`, `.key`)
- **DO NOT** commit database files (`.db`, `.sqlite`)
- **DO NOT** commit API keys, tokens, or passwords

### 2. Use Environment Variables
```bash
# Store secrets in environment variables
export API_KEY=your_secret_key
export DATABASE_URL=your_database_url
```

### 3. Use .gitignore
- All sensitive files are in `.gitignore`
- Verify before committing
- Use `git status` to check

### 4. Use git-crypt for Sensitive Files
```bash
# Install git-crypt
brew install git-crypt

# Initialize git-crypt
git-crypt init

# Add users
git-crypt add-gpg-user USER_ID
```

### 5. Regular Security Audits
- Review `.gitignore` regularly
- Check for accidental commits
- Rotate credentials periodically
- Update dependencies

## Protected Files

The following files are protected and should never be committed:

### Environment Files
- `.env`, `.env.*`
- `*.env`, `*.env.*`
- `secrets/`, `credentials/`, `keys/`

### Application Configs
- `application*.yml`, `application*.yaml`
- `application*.properties`
- `application*.json`, `application*.xml`
- `application*.uml`
- `config/local*`, `config/*.local.*`

### Certificate Files
- `*.pem`, `*.crt`, `*.key`
- `*.p12`, `*.pfx`

### Database Files
- `*.db`, `*.sqlite`, `*.sqlite3`

### Knowledge Base
- `.copilot-knowledge/`
- `*.knowledge.json`

## Pre-commit Hooks

Pre-commit hooks check for:
- Secrets in files
- Sensitive file patterns
- Large files
- Binary files

## Incident Response

If you accidentally commit secrets:
1. **IMMEDIATELY** rotate the exposed credentials
2. Remove from git history
3. Force push
4. Notify affected parties
5. Document the incident

## Dependencies

Regularly update dependencies:
```bash
npm audit
npm audit fix
npm outdated
npm update
```

## Contact

For security questions: security@example.com
