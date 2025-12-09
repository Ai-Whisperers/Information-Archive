# Rules 81-90: Quality & Testing

Standards for code quality, testing, and deployment safety.

---

## Rule 81: Code Review Requirements

All code changes require review:
- **Solo projects**: Self-review after 24h cooling period
- **Team projects**: At least 1 reviewer
- **Critical systems**: 2 reviewers required

**Review checklist:**
- [ ] Code works as intended
- [ ] No obvious bugs or security issues
- [ ] Tests included for new functionality
- [ ] Documentation updated

---

## Rule 82: Testing Levels

Projects should have appropriate test coverage:

| Project Type | Minimum Coverage |
|--------------|------------------|
| Client projects | 60% critical paths |
| Internal tools | 40% core functions |
| Prototypes | Manual testing OK |
| APIs | 80% endpoint coverage |

**Critical paths** = user-facing features, payment flows, auth

---

## Rule 83: Pre-commit Checks

Repositories SHOULD have pre-commit hooks for:
- Linting (ESLint, Pylint, etc.)
- Formatting (Prettier, Black, etc.)
- Type checking (TypeScript, mypy)
- Secret detection (git-secrets, detect-secrets)

**Setup:**
```bash
# .pre-commit-config.yaml or husky
npm run lint && npm run format:check
```

---

## Rule 84: CI/CD Pipeline

Production projects MUST have CI/CD:
- **CI**: Run tests on every PR
- **CD**: Auto-deploy to staging on merge
- **Production**: Manual approval required

**Minimum pipeline:**
1. Install dependencies
2. Run linter
3. Run tests
4. Build
5. Deploy (staging auto, prod manual)

---

## Rule 85: Branch Protection

Main branches MUST be protected:
- `main`/`master`: No direct pushes
- Require PR with at least 1 approval
- Require passing CI checks
- No force pushes allowed

**GitHub Settings:**
- Require pull request reviews
- Require status checks to pass
- Include administrators

---

## Rule 86: Environment Separation

Projects MUST separate environments:

| Environment | Purpose | Data |
|-------------|---------|------|
| Development | Local testing | Mock/seed data |
| Staging | Pre-production testing | Anonymized prod copy |
| Production | Live users | Real data |

**Never** use production data in development without anonymization.

---

## Rule 87: Rollback Procedures

Every deployment MUST have rollback plan:
- Document rollback steps before deploying
- Keep previous version available for 7 days
- Test rollback procedure quarterly
- Maximum rollback time: 15 minutes

**Rollback triggers:**
- Error rate > 5%
- Response time > 2x baseline
- Critical feature broken

---

## Rule 88: Dependency Management

Keep dependencies secure and current:
- Run `npm audit` / `pip-audit` weekly
- Update patch versions monthly
- Update minor versions quarterly
- Major versions: Plan and test

**Auto-update tools:**
- Dependabot (GitHub)
- Renovate

---

## Rule 89: Error Handling

All code MUST handle errors gracefully:
- Log errors with context (not just stack trace)
- User-facing errors: Friendly messages
- Internal errors: Detailed for debugging
- Never expose system details to users

**Good:**
```javascript
try {
  await processPayment(order);
} catch (error) {
  logger.error('Payment failed', { orderId: order.id, error: error.message });
  throw new UserError('Payment could not be processed. Please try again.');
}
```

---

## Rule 90: Performance Baselines

Critical systems MUST have performance baselines:
- API response time < 500ms (p95)
- Page load < 3 seconds
- Background jobs complete within SLA
- Monitor and alert on degradation

**Monitoring:**
- Set up alerts for > 2x baseline
- Review performance weekly
- Document performance improvements

---

## Quick Reference

| Rule | Topic | Key Point |
|------|-------|-----------|
| 81 | Code Review | All changes need review |
| 82 | Test Coverage | 40-80% based on project type |
| 83 | Pre-commit | Lint, format, type check |
| 84 | CI/CD | Auto test, manual prod deploy |
| 85 | Branch Protection | No direct pushes to main |
| 86 | Environments | Dev, Staging, Production |
| 87 | Rollback | 15-minute rollback capability |
| 88 | Dependencies | Weekly audit, monthly patches |
| 89 | Error Handling | Log context, friendly user messages |
| 90 | Performance | Baselines and monitoring |
