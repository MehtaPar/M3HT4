# Project Standards

## Documentation

- Use plain language before specialized terminology
- Explain why a component exists
- Keep pages focused and navigable
- Add diagrams where relationships matter
- Use placeholders in public examples
- Link every major milestone to lessons learned

## Naming

Public examples use generic names:

```text
pve.example.lab
dc01.example.lab
fw01.example.lab
10.10.10.0/24
```

## Change discipline

Major changes should have:

1. Objective
2. Scope
3. Backup or rollback point
4. Implementation notes
5. Validation
6. Documentation update

## Security

No credentials, secret material, externally exploitable details, or live management information belong in the public repository.
