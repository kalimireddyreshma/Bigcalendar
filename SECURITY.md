# Security Policy

## Reporting a Vulnerability

If you discover a security vulnerability in this project, please email us at **kalimireddyreshma@gmail.com** instead of using the issue tracker.

### What to Include

When reporting a vulnerability, please include:

1. **Description**: Clear description of the vulnerability
2. **Location**: Where in the code the vulnerability exists
3. **Impact**: What could happen if exploited
4. **Steps to Reproduce**: How to trigger the vulnerability
5. **Suggested Fix**: If you have one

### Response Timeline

- **Initial Response**: Within 48 hours
- **Fix Development**: 7-30 days depending on severity
- **Release**: Patched version released as soon as possible
- **Disclosure**: We'll work with you on timing and credit

## Supported Versions

| Version | Status | Support Until |
|---------|--------|---|
| 1.0.x | Active | Current |
| < 1.0 | Unsupported | N/A |

## Security Best Practices

### For Users

1. **Keep Dependencies Updated**
   ```bash
   npm update
   npm audit
   ```

2. **Use Environment Variables**
   - Never commit `.env` files
   - Use `.env.local` for sensitive data

3. **Regular Security Audits**
   ```bash
   npm audit
   npm audit fix
   ```

### For Contributors

1. **Code Review**: All code is reviewed before merging
2. **Dependency Management**: Regular updates and audits
3. **Testing**: Security tests included in CI/CD
4. **Documentation**: Security guidelines documented

## Security Measures

- ✅ Automated dependency scanning
- ✅ Code quality checks with ESLint
- ✅ GitHub Actions CI/CD pipeline
- ✅ Branch protection rules
- ✅ Regular security audits

## Vulnerability Disclosure

We follow responsible disclosure practices:

1. We acknowledge receipt of vulnerability reports
2. We work on fixing the issue promptly
3. We release patches before public disclosure
4. We credit the reporter (if desired)

## Security Updates

Security updates are released as patch versions (e.g., 1.0.1) and are important to apply.

---

Thank you for helping keep this project secure! 🔒
