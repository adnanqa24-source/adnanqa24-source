<div align="center">

# ADNAN UMER
### Software Quality Assurance Automation Engineer & SDET

<p>
  <a href="https://adnanqa24-source.github.io/"><b>Live Portfolio</b></a> &nbsp;•&nbsp;
  <a href="https://www.linkedin.com/in/adnan-umer-b9040220a"><b>LinkedIn</b></a> &nbsp;•&nbsp;
  <a href="mailto:adnanqa24@gmail.com"><b>Email</b></a>
</p>

<p>
  <i>Specializing in Playwright automation architecture, autonomous test generation pipelines, and CI/CD test infrastructure on remote Linux servers.</i>
</p>

</div>

---

### Core Systems & Implementations

#### 1. Autonomous AI QA Pipeline (Jam CLI + Playwright CLI)

A decoupled 3-agent orchestration system (Planner, Executor, Healer) engineered to translate browser screen recordings into strongly-typed Playwright test suites without passing heavy video streams or raw DOM dumps into model contexts.

* **Intent Telemetry:** Jam CLI captures user interaction streams into clean JSON intent trees (&lt;1.8k tokens per scenario), avoiding multimodal frame tokens.
* **Local Evaluation:** Live DOM attributes are queried locally via `playwright-cli eval` to dynamically synthesize resilient multi-condition XPath unions.
* **Autonomous Self-Healing:** The healing agent attaches directly to failing runs (`playwright-cli attach`) to inspect mutated DOM elements and update Page Objects without human intervention.

**Operational Impact & Telemetry:**
* **-89.8% Token Overhead:** Context payload dropped from ~88k to ~8.9k tokens via structured intent extraction.
* **50x Authoring Speed:** Scenario turnaround compressed from 2.5 hours down to 3.5 minutes per journey.
* **83% Maintenance Reduction:** Self-healing selector resolution fixed UI drift automatically in active test runs.

---

#### 2. Scalable Playwright Framework & Remote CI/CD

An end-to-end automation infrastructure built on TypeScript and Playwright, backed by dedicated remote server orchestration.

* **Session Storage Caching:** Employs `storageState` caching to preserve auth states, eliminating repeated login steps across multi-tier test suites.
* **Environment Parity:** Configured runtime-driven environment isolation targeting Dev, Staging, and Production without script changes.
* **Remote Linux CI Runner:** Maintained a dedicated Linux server hosting Jenkins on a custom port, managing server upgrades, dependencies, and scheduled cron executions (peak-hour smoke runs and off-peak regression suites).
* **Execution Telemetry:** Built-in Allure test reporting directly embedded in the build lifecycle for rapid defect triage.

**Operational Impact & Telemetry:**
* **Accelerated Execution Runs:** Eliminating login loops via session caching reduced overall test execution durations significantly.
* **Zero Configuration Drift:** 100% parameter reuse across deployment stages with clean multi-environment isolation.

---

### Methodologies & Quality Governance

* **Test Planning & Site Coverage:** Architecting comprehensive coverage matrices across functional surface areas, mapping acceptance criteria, core workflows, and boundary conditions.
* **User Journey Isolation:** Deconstructing multi-step flows into isolated, deterministic user paths to eliminate flaky cross-module dependencies.
* **Accessibility Auditing (WCAG 2.0):** Executing automated and manual accessibility audits via Axe-core, validating keyboard tab order, ARIA landmark roles, screen reader compatibility, and contrast thresholds.
* **Compliance Boundary Testing:** Validating system workflows against HIPAA and FERPA protocols to ensure data privacy, strict access permissions, and proper field masking.

---

### Technical Capabilities

<table>
  <tr>
    <td width="25%"><b>Test Automation</b></td>
    <td>Playwright, TypeScript, Selenium, Postman (REST API), Axe-core</td>
  </tr>
  <tr>
    <td><b>Visual Testing</b></td>
    <td>Pixelmatch, Percy, Applitools Eyes</td>
  </tr>
  <tr>
    <td><b>DevOps & Infrastructure</b></td>
    <td>Jenkins (Declarative Pipelines), Remote Linux Server Administration, SSH, Git, GitHub</td>
  </tr>
  <tr>
    <td><b>Autonomous Tooling</b></td>
    <td>Jam CLI, Playwright CLI, Multi-Condition XPath Union Synthesis</td>
  </tr>
  <tr>
    <td><b>Standards & Compliance</b></td>
    <td>WCAG 2.0 (Level AA), HIPAA Data Privacy, FERPA Regulatory Compliance</td>
  </tr>
  <tr>
    <td><b>Project Governance</b></td>
    <td>Jira (Defect Lifecycle Triage), Confluence, Notion, Agile / Scrum</td>
  </tr>
</table>

---

<div align="center">
  <sub>Lahore, Pakistan • Open to SQA Automation, SDET, and Quality Engineering Opportunities</sub>
</div>