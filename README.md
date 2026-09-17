# Adnan Umer
Software Quality Assurance & Automation Engineering  
Lahore, Pakistan · adnanqa24@gmail.com · [Live Portfolio](https://adnanqa24-source.github.io/) · [LinkedIn](https://www.linkedin.com/in/adnan-umer-b9040220a)

---

### Systems & Implementations

#### Autonomous Test Ingestion & Dynamic Healing System
A decoupled three-agent orchestration pipeline (Planner, Executor, Healer) that compiles end-to-end browser test suites from user interaction recordings without feeding raw video streams or unstructured DOM trees into large language models.

* **Telemetry Ingestion:** Jam CLI captures keystrokes, pointer interactions, and network payloads, producing low-volume intent trees under 1,800 tokens per workflow.
* **Local Evaluation:** Rather than querying models for element detection, `playwright-cli eval` directly queries live document states locally to synthesize multi-condition XPath union locators.
* **Autonomous Repair:** When application UI shifts cause locator failure, a background healer connects to the paused process via `playwright-cli attach`, inspects mutated element attributes, and updates the Page Object without human triage.

##### Observed System Metrics
* **Token Consumption:** Reduced average model context usage from ~88,000 down to ~8,900 tokens (-89.8%).
* **Creation Cycle:** Reduced average test authoring turnaround from 2.5 hours down to 3.5 minutes per journey (50x).
* **Maintenance Overhead:** Automated selector healing resolved ~83% of UI drift failures without manual intervention.

---

#### Enterprise Test Infrastructure & Execution Engine
Scalable end-to-end automation infrastructure built on Playwright and TypeScript, executed against dedicated continuous integration environments.

* **State Persistence:** Implemented Playwright `storageState` caching to retain user sessions across test lifecycles, bypassing repeated authentication flows during multi-tier test suites.
* **Environment Parity:** Configured runtime-driven environment isolation, allowing a single test suite to target Development, Staging, or Production builds without code adjustments.
* **Dedicated Test Runner:** Configured a remote Linux server over SSH, hosting headless Jenkins runners on custom network ports with cron schedules: smoke sweeps during core hours, full regression sweeps off-peak.
* **Defect Telemetry:** Integrated Allure test reports directly into the build pipeline to generate artifact-linked failure histories.

##### Observed System Metrics
* **Runtime Efficiency:** Session caching eliminated redundant login steps, accelerating test execution.
* **Configuration Drift:** Achieved 100% parameter reuse across deployment stages without script branching.

---

### Technical Capabilities

```text
Core Languages       : TypeScript, JavaScript, Python
Frameworks & Tools   : Playwright, Selenium, Postman (API), Axe-core
Visual Testing       : Pixelmatch, Percy, Applitools Eyes
Systems & CI/CD      : Linux Server Administration, Jenkins (Declarative), Bash, SSH, Git
Compliance Protocols : WCAG 2.0 Level AA, HIPAA Data Boundaries, FERPA Access Rules
Operations           : Jira, Confluence, Notion, Agile / Scrum