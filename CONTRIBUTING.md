# Contributing to OrcaSlicer

Thank you for your interest in contributing to OrcaSlicer! This document provides guidelines for contributing to this project, incorporating governance frameworks from TengerTechnologies-Bricklayers.

## Code of Conduct

By participating in this project, you agree to abide by the community guidelines and maintain respectful, constructive communication.

## Developer Certificate of Origin (DCO)

This project uses the Developer Certificate of Origin (DCO) as defined in the [DCO file](./DCO). All contributions must be signed off to certify that you have the right to submit the contribution under the project's license.

### How to Sign Off Your Commits

To sign off your commits, add the `-s` flag when committing:

```bash
git commit -s -m "Your commit message"
```

This adds a `Signed-off-by` line to your commit message, which looks like:
```
Signed-off-by: Your Name <your.email@example.com>
```

### Setting Up Git for Automatic Sign-off

You can configure git to automatically sign off commits:

```bash
git config user.name "Your Name"
git config user.email "your.email@example.com"
git config format.signoff true
```

## Contributing Process

### 1. Fork and Clone

1. Fork the repository on GitHub
2. Clone your fork locally:
   ```bash
   git clone https://github.com/yourusername/OrcaSlicerTest.git
   cd OrcaSlicerTest
   ```

### 2. Development Setup

Follow the build instructions in [How to build](https://github.com/SoftFever/OrcaSlicer/wiki/How-to-build) for your platform.

### 3. Making Changes

1. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. Make your changes following the coding guidelines below
3. Test your changes thoroughly
4. Commit your changes with DCO sign-off:
   ```bash
   git commit -s -m "Brief description of changes"
   ```

### 4. Submitting Pull Requests

1. Push your branch to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```

2. Create a pull request on GitHub
3. Fill out the pull request template completely
4. Ensure all checks pass, including DCO verification

## Coding Guidelines

### C++ Code Style

- Follow C++17 standard
- Use existing patterns found in libslic3r for consistency
- Follow existing naming conventions:
  - PascalCase for classes and structs
  - snake_case for functions and variables
  - UPPER_CASE for constants and macros

### Code Organization

- **libslic3r/**: Core slicing engine modifications
- **src/slic3r/GUI/**: GUI-related changes
- **src/libslic3r/**: Platform-independent functionality
- **resources/**: Resources like profiles and translations

### Testing

- Run existing tests to ensure no regressions
- Add tests for new functionality when applicable
- Tests are located in the `tests/` directory

## Types of Contributions

### Bug Fixes
- Include clear reproduction steps
- Reference the issue number if one exists
- Test the fix thoroughly

### New Features
- Discuss significant features in an issue first
- Follow the existing architecture patterns
- Update documentation as needed

### Documentation
- Use clear, concise language
- Include examples where helpful
- Follow existing documentation structure

### Profiles and Configurations
- Add printer profiles in `resources/profiles/`
- Follow existing profile structure and naming

## Attribution and Credits

This contribution framework incorporates governance elements from TengerTechnologies-Bricklayers, ensuring proper legal and procedural foundations for community contributions.

## Getting Help

- **Documentation**: Check the [OrcaSlicer Wiki](https://github.com/SoftFever/OrcaSlicer/wiki)
- **Discord**: Join the [community Discord](https://discord.gg/P4VE9UY9gJ)
- **Issues**: Search existing issues before creating new ones

## License

By contributing to OrcaSlicer, you agree that your contributions will be licensed under the GNU Affero General Public License v3.0, as stated in the [LICENSE.txt](./LICENSE.txt) file.

## Review Process

All contributions go through a review process:

1. **Automated Checks**: DCO verification, build checks, and automated testing
2. **Code Review**: Maintainer review for code quality, adherence to guidelines
3. **Testing**: Verification that changes work as intended
4. **Merge**: Integration into the main branch

Thank you for contributing to OrcaSlicer and helping make 3D printing more accessible and powerful!