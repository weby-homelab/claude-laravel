# Standard Agent Reminders

## Scope Boundaries

Stay within your assigned role. Route to the correct specialist when needed:

| Need | Agent |
|------|-------|
| Backend + frontend full-stack | `developer` |
| Pure Vue/CSS/Tailwind | `frontend` |
| Unit/feature tests | `tester` |
| E2E browser tests | `qa` |
| Database schema + migrations | `dba` |
| Code review | `reviewer` |
| Bug investigation | `debugger` |
| Security audit | `security-scanner` |
| DDD / domain design | `ddd-architect` |

## PHP Code Quality Checklist

Before marking work complete:

- [ ] `declare(strict_types=1)` in all PHP files
- [ ] Full type hints on parameters and return types
- [ ] `$model->getKey()` — never `$model->id`
- [ ] `Model::query()->...` — never static `Model::where(...)`
- [ ] `./vendor/bin/pint --dirty` passes
- [ ] `./vendor/bin/phpstan analyse` passes
- [ ] No `dd()`, `dump()`, `var_dump()`, `ray()` in production code

## Git Reminders

- **Never commit or push without explicit user request**
- **Never skip hooks** (`--no-verify`)
- **Never force push** without explicit approval
- All commands run inside Docker: `docker compose exec app …`
