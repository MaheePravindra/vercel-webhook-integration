# Contributing to Vercel Webhook Integration

Thank you for your interest in contributing to the Vercel Webhook Integration project! This document provides guidelines for contributing to this project.

## Getting Started

1. Fork the repository
2. Clone your fork locally
3. Create a new branch for your feature or bug fix
4. Make your changes
5. Test your changes thoroughly
6. Submit a pull request

## Development Setup

### Prerequisites
- Python 3.9 or higher
- Node.js (for Google Apps Script development)
- Git
- Vercel CLI (optional, for deployment testing)

### Local Development
```bash
# Clone the repository
git clone https://github.com/MaheePravindra/vercel-webhook-integration.git
cd vercel-webhook-integration

# Set up environment variables
cp .env.example .env
# Edit .env with your configuration

# Test the endpoints locally (if using Vercel CLI)
vercel dev
```

## Code Style Guidelines

### Python Code
- Follow PEP 8 style guidelines
- Use meaningful variable and function names
- Add docstrings to all functions
- Include type hints where appropriate
- Keep functions focused and single-purpose

### JavaScript Code
- Use consistent indentation (2 spaces)
- Use meaningful variable names
- Add comments for complex logic
- Follow Google Apps Script best practices

### Documentation
- Update README.md if adding new features
- Update API_REFERENCE.md for API changes
- Include examples in documentation
- Keep documentation up to date with code changes

## Testing

### Manual Testing
- Test all endpoints with sample payloads
- Verify Google Sheets integration
- Test error handling scenarios
- Validate external API integrations

### Test Payloads
Use the sample payloads provided in the documentation to test endpoints:
- Fire Safety: Test with different emergency types
- Plumbing/HVAC: Test with various service scenarios
- Error Cases: Test with malformed data

## Pull Request Process

1. **Create a descriptive title** that summarizes the change
2. **Provide a detailed description** including:
   - What changes were made
   - Why the changes were necessary
   - How to test the changes
   - Any breaking changes

3. **Update documentation** as needed
4. **Test thoroughly** before submitting
5. **Keep PRs focused** - one feature or fix per PR

## Issue Reporting

When reporting issues, please include:
- Clear description of the problem
- Steps to reproduce
- Expected vs actual behavior
- Environment details (Python version, etc.)
- Sample payloads (if applicable)
- Error messages or logs

## Feature Requests

For new features:
- Describe the use case
- Explain the expected behavior
- Consider backward compatibility
- Discuss implementation approach

## Code Review Guidelines

### For Reviewers
- Check for code quality and style
- Verify functionality works as described
- Test edge cases and error scenarios
- Ensure documentation is updated
- Consider security implications

### For Contributors
- Respond to feedback promptly
- Make requested changes
- Keep discussions focused and professional
- Test changes after addressing feedback

## Security

- Never commit sensitive data (API keys, passwords)
- Use environment variables for configuration
- Follow security best practices
- Report security issues privately

## Documentation Standards

### Code Comments
```python
def extract_variables_v2(call_data):
    """
    Extract dynamic variables for the second webhook
    
    Args:
        call_data (dict): Retell AI call data payload
        
    Returns:
        dict: Extracted variables with keys: fromNumber, customerName, etc.
    """
```

### API Documentation
- Include request/response examples
- Document all parameters
- Explain error codes
- Provide usage examples

## Release Process

1. Update version numbers
2. Update CHANGELOG.md
3. Create release notes
4. Tag the release
5. Deploy to production

## Community Guidelines

- Be respectful and inclusive
- Help others learn and grow
- Share knowledge and best practices
- Follow the code of conduct

## Getting Help

- Check existing documentation first
- Search existing issues
- Create a new issue with detailed information
- Join discussions in pull requests

## Recognition

Contributors will be recognized in:
- README.md contributors section
- Release notes
- Project documentation

Thank you for contributing to make this project better!