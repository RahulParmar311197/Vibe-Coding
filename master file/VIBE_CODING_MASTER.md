# VIBE CODING MASTER FRAMEWORK

## Universal AI-Assisted Software Development Operating System

**Version:** 1.0
**Purpose:** Build, validate, deploy, and operate software projects from idea to production.

---

# 1. PURPOSE

This document defines the operating rules for an AI-assisted development project.

The AI agent must use this document as the project's engineering constitution.

The objective is:

> Transform a software idea into a tested, secure, maintainable, observable, deployable, production-ready system.

This framework applies to:

* SaaS
* Web applications
* Mobile applications
* AI applications
* AI agents
* APIs
* ERP systems
* Financial systems
* Trading systems
* Automation platforms
* Data platforms
* Internal business software
* Developer tools
* Consumer applications

---

# 2. CORE PRINCIPLE

AI must NOT behave as:

> Prompt → Generate code → Next feature.

AI must behave as:

> Understand → Inspect → Plan → Implement → Test → Verify → Document → Integrate → Review → Continue.

Never assume that generated code is correct.

Never mark a task complete merely because implementation exists.

---

# 3. PROJECT LIFECYCLE

Every project follows:

```text
IDEA
 ↓
DISCOVERY
 ↓
REQUIREMENTS
 ↓
PRODUCT DESIGN
 ↓
ARCHITECTURE
 ↓
TECHNOLOGY SELECTION
 ↓
PROJECT FOUNDATION
 ↓
IMPLEMENTATION
 ↓
TESTING
 ↓
SECURITY
 ↓
PERFORMANCE
 ↓
INTEGRATION
 ↓
STAGING
 ↓
PRODUCTION
 ↓
MONITORING
 ↓
MAINTENANCE
 ↓
CONTINUOUS IMPROVEMENT
```

---

# 4. STANDARD PROJECT STRUCTURE

```text
PROJECT/
│
├── 00_DISCOVERY/
│
├── 01_REQUIREMENTS/
│
├── 02_PRODUCT/
│
├── 03_ARCHITECTURE/
│
├── 04_UX_UI/
│
├── 05_DATABASE/
│
├── 06_API/
│
├── 07_BACKEND/
│
├── 08_FRONTEND/
│
├── 09_AI_ML/
│
├── 10_INTEGRATIONS/
│
├── 11_DATA/
│
├── 12_SECURITY/
│
├── 13_TESTING/
│
├── 14_PERFORMANCE/
│
├── 15_OBSERVABILITY/
│
├── 16_DEVOPS/
│
├── 17_ENVIRONMENTS/
│
├── 18_DOCUMENTATION/
│
├── 19_OPERATIONS/
│
├── 20_RELEASE/
│
├── .ai/
│
├── .github/
│
├── scripts/
│
├── tests/
│
├── docker/
│
├── README.md
├── LICENSE
├── CHANGELOG.md
└── .gitignore
```

Not every project needs every directory.

Unused modules should be explicitly marked:

```text
NOT_REQUIRED
```

Do not create unnecessary complexity.

---

# 5. AI PROJECT MEMORY

The `.ai/` directory is the persistent engineering memory.

```text
.ai/
│
├── SYSTEM.md
├── PROJECT_CONTEXT.md
├── RULES.md
├── ARCHITECTURE_RULES.md
├── CODING_RULES.md
├── SECURITY_RULES.md
├── TESTING_RULES.md
├── AGENT_WORKFLOW.md
│
├── CURRENT_STATE.md
├── MASTER_TASKS.md
├── COMPLETED.md
├── PENDING.md
├── BLOCKED.md
├── BUGS.md
├── TECH_DEBT.md
│
├── DECISIONS.md
├── CHANGE_POLICY.md
└── DEFINITION_OF_DONE.md
```

The AI MUST read the relevant `.ai/` files before making major changes.

---

# 6. PROJECT CONTEXT

Maintain:

```text
.ai/PROJECT_CONTEXT.md
```

It should contain:

```text
Project name
Project purpose
Target users
Primary problem
Business objective
Major features
Technology stack
Architecture style
Deployment environment
External services
Database
Authentication
Known constraints
Important decisions
Current development phase
```

This file must remain current.

---

# 7. CURRENT STATE

Maintain:

```text
.ai/CURRENT_STATE.md
```

Track:

```text
Current phase
Completed systems
In-progress systems
Pending systems
Known bugs
Known limitations
Technical debt
Deployment state
Test state
Production state
```

The AI must inspect this before deciding what to work on next.

---

# 8. MASTER TASK SYSTEM

Maintain:

```text
.ai/MASTER_TASKS.md
```

Every task should have:

```text
ID
Description
Priority
Dependencies
Status
Owner/Agent
Files affected
Acceptance criteria
Tests
```

Recommended statuses:

```text
BACKLOG
READY
IN_PROGRESS
BLOCKED
IMPLEMENTED
TESTING
FAILED
FIXING
REVIEW
STAGING
PRODUCTION_READY
DONE
```

---

# 9. PRIORITY SYSTEM

Use:

```text
P0 = Critical
P1 = High
P2 = Medium
P3 = Low
P4 = Future
```

Rules:

* P0 issues take priority over features.
* Security issues take priority over convenience features.
* Data corruption takes priority over UI improvements.
* Production failures take priority over new development.

---

# 10. REQUIREMENTS

Every major feature must have:

```text
Requirement
 ↓
User story
 ↓
Acceptance criteria
 ↓
Implementation task
 ↓
Tests
 ↓
Verification
```

Example:

```text
REQ-001

Requirement:
Users can securely log in.

Acceptance:
- Valid credentials succeed.
- Invalid credentials fail.
- Sessions expire correctly.
- Unauthorized users cannot access protected resources.
```

---

# 11. DEFINITION OF DONE

A feature is NOT DONE until applicable items pass:

```text
[ ] Requirement implemented
[ ] Acceptance criteria satisfied
[ ] Architecture respected
[ ] Database changes complete
[ ] API complete
[ ] Frontend complete
[ ] Validation implemented
[ ] Error handling implemented
[ ] Authentication checked
[ ] Authorization checked
[ ] Unit tests pass
[ ] Integration tests pass
[ ] E2E tests pass where applicable
[ ] Security reviewed
[ ] Performance reviewed
[ ] Logging implemented
[ ] Metrics implemented
[ ] Documentation updated
[ ] Configuration updated
[ ] Migration created
[ ] Regression tests pass
[ ] Build succeeds
[ ] Deployment succeeds
```

Only then may the task be marked:

```text
DONE
```

---

# 12. ARCHITECTURE RULES

Before major implementation:

```text
Understand existing architecture.
Identify dependencies.
Identify affected components.
Identify data flow.
Identify API contracts.
Identify database impact.
Identify security impact.
Identify deployment impact.
```

Never introduce a new architectural pattern without justification.

Avoid:

```text
Duplicate services
Duplicate business logic
Unnecessary abstractions
Unnecessary microservices
Circular dependencies
Hidden global state
Hard-coded configuration
```

Prefer simple architecture until complexity is justified.

---

# 13. CODEBASE INSPECTION

Before changing existing code:

```text
1. Locate relevant files.
2. Read surrounding implementation.
3. Identify callers.
4. Identify dependencies.
5. Identify tests.
6. Identify configuration.
7. Identify database impact.
8. Identify external integrations.
9. Determine backward compatibility requirements.
```

Never blindly overwrite existing code.

---

# 14. IMPLEMENTATION LOOP

For every task:

```text
READ
 ↓
UNDERSTAND
 ↓
PLAN
 ↓
IMPLEMENT
 ↓
FORMAT
 ↓
LINT
 ↓
TYPE CHECK
 ↓
UNIT TEST
 ↓
INTEGRATION TEST
 ↓
DEBUG
 ↓
SECURITY CHECK
 ↓
REGRESSION TEST
 ↓
DOCUMENT
 ↓
UPDATE STATE
 ↓
REVIEW
```

---

# 15. CODING RULES

Code must be:

* Readable
* Testable
* Modular
* Maintainable
* Explicit
* Consistent
* Secure
* Observable

Avoid:

```text
Magic numbers
Hard-coded secrets
Duplicated logic
Huge functions
Huge classes
Dead code
Unused dependencies
Unexplained workarounds
Silent exception handling
```

---

# 16. ERROR HANDLING

Every external boundary must be treated as unreliable.

Examples:

```text
Database
API
Network
File system
Queue
Broker
Payment provider
LLM
Authentication provider
Third-party service
```

Handle:

```text
Timeout
Retry
Rate limit
Invalid response
Unavailable service
Partial failure
Duplicate request
Malformed input
Authentication failure
Authorization failure
```

Never silently swallow important errors.

---

# 17. DATABASE RULES

Database changes must be:

```text
Version controlled
Migratable
Reversible where practical
Tested
Documented
```

Never modify production schemas manually without a controlled migration process.

Track:

```text
Schema
Indexes
Constraints
Relationships
Migrations
Seed data
Retention
Backups
```

---

# 18. API RULES

APIs must define:

```text
Endpoint
Method
Request
Response
Validation
Authentication
Authorization
Errors
Rate limits
Versioning
```

Maintain an API specification where practical.

Never break an existing API without explicitly handling compatibility.

---

# 19. FRONTEND RULES

Frontend must handle:

```text
Loading
Success
Empty state
Error state
Offline state where applicable
Validation
Authentication
Authorization
Responsive layout
Accessibility
```

Do not build only the happy path.

---

# 20. AI/ML RULES

For AI systems maintain:

```text
Models
Prompts
Datasets
Parameters
Evaluation
Benchmarks
Experiments
Model versions
Prompt versions
Guardrails
Costs
Latency
Failure cases
```

Never assume AI output is deterministic unless verified.

AI decisions must have appropriate validation and fallback mechanisms.

For high-impact systems, AI should not directly bypass deterministic safety controls.

---

# 21. SECURITY

Security must be implemented throughout development.

Check:

```text
Authentication
Authorization
RBAC
Input validation
Output validation
Secrets
Encryption
Session security
Rate limiting
CORS
CSRF where applicable
SQL injection
XSS
SSRF
Dependency vulnerabilities
Container vulnerabilities
Audit logging
Data access
File uploads
Webhooks
API abuse
```

Never store secrets in source control.

---

# 22. TESTING PYRAMID

Use:

```text
             E2E
              ▲
             / \
        Integration
           /   \
          /     \
        Unit Tests
```

Testing should include:

```text
Unit
Integration
API
Database
E2E
Regression
Security
Performance
Load
Failure scenarios
```

Tests must validate behavior, not merely code coverage.

---

# 23. QUALITY GATE

Before merging:

```text
[ ] Build passes
[ ] Lint passes
[ ] Type checking passes
[ ] Tests pass
[ ] No critical vulnerabilities
[ ] No accidental secrets
[ ] Database migration tested
[ ] API compatibility checked
[ ] Documentation updated
```

---

# 24. PERFORMANCE

Define measurable targets where appropriate:

```text
Latency
Throughput
Concurrency
Memory
CPU
Database performance
Queue latency
Page performance
Error rate
```

Measure before optimizing.

Do not perform premature optimization.

---

# 25. OBSERVABILITY

Production systems should provide:

```text
Logs
Metrics
Traces where appropriate
Health checks
Alerts
Dashboards
Audit events
```

Typical endpoints:

```text
/health
/live
/ready
/metrics
```

Never log:

```text
Passwords
API keys
Tokens
Private credentials
Sensitive personal information
```

---

# 26. DEPLOYMENT

Deployment must support appropriate environments:

```text
Development
 ↓
Testing
 ↓
Staging
 ↓
Production
```

Production configuration must be isolated from development configuration.

---

# 27. CI/CD

CI should automatically perform applicable checks:

```text
Install
 ↓
Lint
 ↓
Type check
 ↓
Unit tests
 ↓
Integration tests
 ↓
Security scan
 ↓
Build
 ↓
Package
 ↓
Deploy
```

Deployment should fail safely.

---

# 28. ROLLBACK

Every production release should have a rollback strategy.

```text
Release
 ↓
Health check
 ↓
Verification
 ↓
Success
```

or:

```text
Release
 ↓
Failure
 ↓
Rollback
 ↓
Investigate
 ↓
Fix
 ↓
Redeploy
```

---

# 29. FEATURE FLAGS

Use feature flags for risky or gradual releases where useful.

Example:

```text
FEATURE_NEW_DASHBOARD=false
FEATURE_NEW_AI_ENGINE=false
FEATURE_NEW_PAYMENT_FLOW=false
```

Never use feature flags as a substitute for proper architecture.

---

# 30. DATA BACKUP

Define:

```text
What is backed up?
How often?
Where?
How long?
How is it encrypted?
How is restoration tested?
```

A backup that has never been restored successfully should not be considered fully reliable.

---

# 31. DISASTER RECOVERY

Document:

```text
RTO
RPO
Backup strategy
Restore procedure
Failover procedure
Emergency contacts/process
Data recovery
Infrastructure recovery
```

Test recovery periodically where appropriate.

---

# 32. GIT RULES

Use meaningful commits.

Examples:

```text
feat: add user authentication
fix: handle expired sessions
refactor: simplify order service
test: add payment integration tests
docs: update deployment guide
chore: update dependencies
```

Avoid:

```text
stuff
changes
final
final2
new
test
```

---

# 33. ARCHITECTURE DECISION RECORDS

Important decisions must be documented.

Example:

```text
ADR-001

Decision:
Use PostgreSQL as primary relational database.

Context:
The application requires transactional consistency and relational queries.

Alternatives:
MySQL
MongoDB

Reason:
PostgreSQL provides required relational features and ecosystem support.

Status:
Accepted
```

Never repeatedly reconsider an already-settled decision without new evidence.

---

# 34. TECHNICAL DEBT

Maintain:

```text
.ai/TECH_DEBT.md
```

Each item:

```text
ID
Problem
Impact
Severity
Proposed solution
Priority
```

Technical debt must be visible rather than forgotten.

---

# 35. BUG MANAGEMENT

Every significant bug should contain:

```text
Bug ID
Severity
Reproduction
Expected behavior
Actual behavior
Root cause
Fix
Regression test
Status
```

Fix root causes where practical.

Do not repeatedly patch symptoms.

---

# 36. DOCUMENTATION

Maintain appropriate:

```text
README
Architecture
Setup
Development
API
Database
Deployment
Operations
Troubleshooting
Security
User documentation
```

Documentation must evolve with implementation.

---

# 37. REQUIREMENT TRACEABILITY

Every important requirement should be traceable:

```text
REQ
 ↓
FEATURE
 ↓
TASK
 ↓
CODE
 ↓
TEST
 ↓
ACCEPTANCE
```

Example:

```text
REQ-023
 ↓
FEATURE-014
 ↓
TASK-091
 ↓
backend/payment/service.py
 ↓
test_payment_service.py
 ↓
ACCEPTED
```

---

# 38. PRODUCTION READINESS

Before production:

```text
[ ] Requirements complete
[ ] Critical features complete
[ ] Database production-ready
[ ] APIs stable
[ ] Frontend stable
[ ] Authentication secure
[ ] Authorization verified
[ ] Secrets configured
[ ] Backups configured
[ ] Restore tested
[ ] Monitoring configured
[ ] Alerts configured
[ ] Error tracking configured
[ ] Performance tested
[ ] Security tested
[ ] Load tested where necessary
[ ] CI/CD working
[ ] Staging verified
[ ] Rollback tested
[ ] Documentation complete
[ ] Runbook complete
```

---

# 39. RELEASE GATE

A release requires:

```text
CODE READY
+
TESTS PASSING
+
SECURITY ACCEPTABLE
+
PERFORMANCE ACCEPTABLE
+
DATABASE READY
+
DEPLOYMENT READY
+
ROLLBACK READY
+
MONITORING READY
+
DOCUMENTATION READY
```

Then:

```text
PRODUCTION_READY
```

---

# 40. POST-RELEASE

After deployment:

```text
Monitor
 ↓
Verify health
 ↓
Verify errors
 ↓
Verify metrics
 ↓
Verify critical workflows
 ↓
Review user impact
 ↓
Document issues
 ↓
Create follow-up tasks
```

Do not consider deployment the end of engineering.

---

# 41. PROJECT COMPLETION LEVELS

```text
L0  IDEA
L1  DISCOVERY_COMPLETE
L2  REQUIREMENTS_COMPLETE
L3  ARCHITECTURE_COMPLETE
L4  FOUNDATION_COMPLETE
L5  MVP_COMPLETE
L6  FEATURE_COMPLETE
L7  TEST_COMPLETE
L8  SECURITY_READY
L9  PERFORMANCE_READY
L10 STAGING_READY
L11 PRODUCTION_READY
L12 RELEASED
L13 OPERATING
```

The project should always have a clearly documented current level.

---

# 42. AI AGENT OPERATING MODES

The AI may operate in:

```text
DISCOVERY MODE
PLANNING MODE
ARCHITECT MODE
CODING MODE
DEBUG MODE
TESTING MODE
SECURITY MODE
PERFORMANCE MODE
REVIEW MODE
DEVOPS MODE
DOCUMENTATION MODE
RELEASE MODE
```

The agent should explicitly determine which mode is appropriate before substantial work.

---

# 43. AI AGENT SAFETY RULES

The AI must NOT:

```text
Delete production data without explicit authorization.
Expose secrets.
Commit credentials.
Disable security controls to make tests pass.
Delete tests merely because they fail.
Ignore failing tests.
Silently change requirements.
Silently change architecture.
Invent unavailable APIs.
Assume external services behave correctly.
Declare success without verification.
```

When uncertain:

```text
Inspect
Validate
Ask when necessary
```

---

# 44. CHANGE IMPACT ANALYSIS

Before significant changes:

```text
What files change?
What services change?
What APIs change?
What database objects change?
What tests change?
What integrations change?
What security implications exist?
What performance implications exist?
What deployment implications exist?
```

---

# 45. NO LOOK-AHEAD / DATA INTEGRITY

For systems involving analytics, finance, trading, forecasting, or ML:

```text
Historical data must remain historically valid.

No future information may leak into training,
features, signals, validation, or decisions.
```

Use:

```text
Time-aware splits
Walk-forward validation
Point-in-time data
Proper feature timestamps
Transaction-cost modeling
Slippage modeling
Data quality checks
```

---

# 46. FINANCIAL / HIGH-RISK SYSTEMS

For financial or otherwise high-impact systems:

```text
Deterministic risk controls
Independent validation
Audit logs
Position limits
Exposure limits
Kill switches
Failure handling
Reconciliation
Paper/sandbox testing
Explicit authorization
```

AI recommendations must not bypass deterministic risk controls.

---

# 47. COST CONTROL

For AI/cloud projects track:

```text
Infrastructure cost
Database cost
Storage
Bandwidth
API cost
LLM/token cost
Compute
Monitoring
Third-party services
```

Where useful measure:

```text
Cost per user
Cost per request
Cost per workflow
Cost per transaction
```

---

# 48. PROJECT HEALTH SCORE

Maintain a project health assessment:

```text
Requirements       %
Architecture       %
Implementation     %
Testing            %
Security           %
Performance        %
Documentation      %
Operations         %
Deployment         %
```

Never calculate project completion using only lines of code.

---

# 49. AI DEVELOPMENT COMMAND

A generic command for the AI coding agent:

```text
You are the engineering agent for this project.

First inspect the repository and the .ai/ project memory.

Determine:
1. Current project phase.
2. Current state.
3. Completed work.
4. Pending work.
5. Blocked work.
6. Existing bugs.
7. Relevant architecture.
8. Relevant dependencies.

Do not immediately write code.

First create an implementation plan.

Then implement the smallest correct change.

Run appropriate tests.

If tests fail, diagnose the root cause and fix it.

Do not delete or weaken tests simply to obtain a passing result.

Check security and regression impact.

Update documentation and project state.

Only mark the task DONE after the Definition of Done is satisfied.

Then identify the highest-priority valid next task.

Never invent missing external APIs, credentials, data, or requirements.
```

---

# 50. AUTONOMOUS DEVELOPMENT LOOP

When authorized to continue automatically:

```text
while project_not_complete:

    inspect_current_state()

    select_highest_priority_task()

    analyze_dependencies()

    create_plan()

    implement()

    run_tests()

    if failure:
        diagnose()
        fix()
        rerun_tests()

    run_security_checks()

    run_regression_checks()

    update_documentation()

    update_project_state()

    commit_changes()

    verify_completion()

    select_next_task()
```

The loop must stop when:

```text
BLOCKED
REQUIRES_HUMAN_DECISION
SECURITY_RISK
DATA_LOSS_RISK
PRODUCTION_RISK
MISSING_CREDENTIAL
MISSING_EXTERNAL_RESOURCE
```

---

# 51. FINAL PROJECT AUDIT

Before declaring the entire project complete:

```text
PRODUCT
[ ] Requirements satisfied

ARCHITECTURE
[ ] Architecture consistent
[ ] Dependencies understood

CODE
[ ] Code quality acceptable
[ ] No critical dead code

DATABASE
[ ] Schema correct
[ ] Migrations correct
[ ] Backup verified

API
[ ] Contracts stable
[ ] Validation complete

FRONTEND
[ ] Core workflows work
[ ] Error/loading states work

AI/ML
[ ] Evaluation complete
[ ] Models/prompts versioned
[ ] Guardrails implemented

SECURITY
[ ] Authentication
[ ] Authorization
[ ] Secrets
[ ] Dependency scan
[ ] Security review

TESTING
[ ] Unit
[ ] Integration
[ ] E2E
[ ] Regression
[ ] Performance where required

OPERATIONS
[ ] Logging
[ ] Metrics
[ ] Alerts
[ ] Health checks
[ ] Runbook

DEVOPS
[ ] Docker/build
[ ] CI/CD
[ ] Staging
[ ] Production deployment

RECOVERY
[ ] Backup
[ ] Restore
[ ] Rollback

DOCUMENTATION
[ ] User
[ ] Developer
[ ] API
[ ] Deployment
[ ] Operations

RELEASE
[ ] Release checklist
[ ] Production acceptance
[ ] Monitoring
```

---

# 52. FINAL DEFINITION

A project is considered:

## PRODUCTION READY

only when the system can be:

```text
Built
+
Configured
+
Tested
+
Secured
+
Deployed
+
Monitored
+
Recovered
+
Maintained
```

A project is considered:

## PRODUCTION COMPLETE

only when:

```text
Business requirements
+
Technical requirements
+
Quality requirements
+
Security requirements
+
Operational requirements
+
Documentation
+
Acceptance criteria
```

have been satisfied.

---

# 53. GOLDEN RULE

Never optimize for:

> "How much code can the AI generate?"

Optimize for:

> "How reliably can the system move from requirement to verified production behavior?"

The AI is the implementation accelerator.

The framework is the control system.

The tests are the verification system.

The architecture is the structure.

The human remains the final authority for consequential decisions.

---

# END OF VIBE CODING MASTER FRAMEWORK
