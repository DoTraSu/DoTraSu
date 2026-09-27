# DoTraSu Constitution

## Core Principles

### I. CLI-First Architecture

DoTraSu is a CLI application first; a future frontend is optional.
Every feature must work through the command line.
All core logic must be importable as a library for future reuse.

### II. Input Validation

Validate early, reject loudly, and provide clear error messages.
Input validation is non-negotiable and applies to every entry point.

### III. Security

Secrets must never be committed to version control.
Never hardcode API keys, passwords, tokens, or credentials.
Use environment variables or a secrets manager for sensitive data.
Add secrets to .gitignore and document the required variables in README.
Audit dependencies for known vulnerabilities before adding new ones.

### IV. Code Quality

Keep it simple. Use simple architectures with no unnecessary abstractions.
Prefer readable, straightforward code over clever one-liners.
Each module should do one thing well and expose a clear interface.
Complex logic must have explanatory comments describing the rationale.
ASD-STE100 (Simplified Technical English) governs all written text:
short sentences, active voice, one meaning per sentence, no jargon.
Code comments, documentation, and user-facing messages follow ASD-STE100.
The application must be easily extensible, closed for modification.

## Platform Independence

The application must run on all major operating systems (Windows, macOS, Linux).
Use only platform-independent libraries and standard library features.
Avoid OS-specific path separators, line endings, or shell commands.
Where platform-specific behavior is unavoidable, abstract it behind a
clear interface with platform-specific implementations.

## Documentation

README must be kept up to date with accurate setup and usage instructions.
The README must include: what the app does, installation steps,
configuration requirements, and basic usage examples.
Update the README with every change that affects setup, configuration,
or user-facing behavior.

## Governance

This constitution supersedes all other development practices in this project.
Amendments require a clear rationale and must be recorded in this file.
Versioning follows semantic versioning (MAJOR.MINOR.PATCH):

- MAJOR: principle removal or backward-incompatible redefinition.
- MINOR: new principle or section added, or materially expanded guidance.
- PATCH: wording clarifications, typo fixes, non-semantic refinements.

All changes to this constitution are tracked via git commits with
descriptive messages referencing the constitution version.

**Version**: 1.0.0 | **Ratified**: 2026-09-27 | **Last Amended**: 2026-09-27
