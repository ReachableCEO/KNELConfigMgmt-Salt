# Agent Guidelines

## Git Commit Requirements

When making changes to this repository, ALWAYS:

1. **Commit atomically**: Each logical change should be its own commit
2. **Use conventional commit format**:
   - `feat(scope): description` - New feature
   - `fix(scope): description` - Bug fix
   - `docs: description` - Documentation changes
   - `refactor(scope): description` - Code refactoring
   - `test(scope): description` - Test additions/changes
   - `chore: description` - Maintenance tasks
3. **Write verbose, beautifully formatted messages**:
   - Title line (50 chars max)
   - Blank line
   - Body explaining WHAT and WHY (not how)
   - Reference related files/issues
   - Include footer with attribution

## Example Commit

```
feat(security-hardening): implement SCAP-STIG compliance logic

Refactor apply script to implement comprehensive security hardening:

- Add GRUB bootloader permission hardening (root:root, mode 0400)
- Disable and remove autofs service per STIG requirements
- Deploy modprobe configurations for kernel module blacklisting
- Create STIG-compliant network protocol blacklist

This ensures servers meet DoD security requirements for production
deployment.

🤖 Generated with [Crush](https://github.com/charmassociates/crush)

Assisted-by: GLM-5 via Crush <crush@charm.land>
```

## Important

**NEVER wait to be asked to commit and push your work.**
**Commit immediately after each logical unit of work.**
