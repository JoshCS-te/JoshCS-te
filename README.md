# Olusegun Joshua Adeoluwa
### Cybersecurity Specialist & Software Engineer

I am a Computer Science graduate and the founder of **NEMSEC**. I bridge the gap between robust software engineering and security operations by building evidence-centric investigation tools and secure, production-grade applications. 

Every system in my portfolio is designed, built, and verified end-to-end—backed by **over 520 automated tests** and a school management platform running live in production.

---

## 🛠️ Technical Skillset

- **Security & Forensics:** Phishing & Email Forensics, Log Analysis, Detection Rule Engineering, Evidence Integrity & Chain of Custody (SHA-256), Malware Static Analysis, Sandbox Orchestration (CAPEv2), Secure Web Development (OWASP Top 10 mitigation), Network Security.
- **Software Engineering:** Python (FastAPI, PySide6, pytest), TypeScript/JavaScript (Next.js, NestJS, React, Node.js), Databases (PostgreSQL, SQLite, Prisma ORM, SQLAlchemy), Deployment (Supabase, Render, Netlify), Git.

---

## 🚀 Featured Projects

### 🛡️ Cybersecurity & Investigation Tools

#### [Phishing Investigation Workbench](https://github.com)
*Next.js, TypeScript, FastAPI, SQLite, CAPEv2, ReportLab | 70 backend tests*
- **Evidence Preservation:** Imports and preserves raw `.eml` files using SHA-256 hashing to guarantee chain of custody.
- **Sandboxed Analysis:** Renders safe email previews within a strict sandboxed iframe (`default-src 'none'`) with `nh3` HTML sanitization.
- **Static Defenses:** Inspects attachments (Office macros via `oletools`, PE headers, archive depth/zip-bomb thresholds) in an isolated, resource-constrained static worker process.
- **Dynamic Detonation:** Integrates a CAPEv2 API adapter for opt-in malware detonation with post-run environment reset verification.
- **Analyst-First Logic:** Discards arbitrary "threat scores" in favor of 30+ deterministic rules that map observed indicators to clear benign or malicious context.

#### [Incident Investigation & Report Builder](https://github.com)
*Next.js, TypeScript, FastAPI, SQLite, ReportLab | 56 backend tests*
- **Timeline Normalization:** ingests mixed-offset raw security logs as immutable, hash-verified evidence and outputs a UTC-normalized timeline tracing events to exact line numbers.
- **Correlated Detection Chain:** Implements stateful detection rules tracking an actor's lifecycle: `Failed-Login Burst` ➔ `Success After Burst` ➔ `Privilege Change` ➔ `Data Export`.
- **Tamper-Evident Reporting:** Features a versioned case-management interface requiring direct log citations for findings, producing freeze-locked PDF incident reports.

---

### 🌐 Secure Production Applications

#### [School Management Information System (SMIS)](https://github.com)
*NestJS, Prisma, PostgreSQL (Supabase), Vanilla JS | 144 API endpoints | 208 automated tests*
- **Production Status:** Built and delivered through NEMSEC; currently driving daily admissions, academics, and grading workflows live at BE RADIANT SCHOOLS.
- **Financial Engineering:** Manages student ledgers and automates multi-tier billing templates integrated with Paystack and Flutterwave webhooks inside strict database transactions.
- **Hardened RBAC:** Restricts access across 9 discrete user roles using an additive 41-permission matrix on the backend, fortified by failed-login lockouts, session timeouts, and immutable audit logs.
*(Note: Production codebase is proprietary; link points to fully functional public demonstration suite).*

#### [EduOS: School Timetable Engine](https://github.com)
*React, Vite, Node.js, SQLite | Version v1.9.9*
- **Constraint Satisfaction:** Automatically compiles secondary-school timetables using a backtracking search algorithm optimized with Minimum Remaining Values (MRV) and forward checking.
- **Relaxation Fallback:** Employs a deterministic 7-tier relaxation pipeline that gracefully handles impossible constraints by double-booking teachers/rooms as a last resort and flagging conflicts for manual review.

---

### 🖥️ Desktop & Research Engines

#### [NEM: Priority Assistant for Windows](https://github.com)
*Python, PySide6 (Qt), SQLite, Vosk, PyInstaller | 188 automated tests*
- **Offline Architecture:** A local-first productivity assistant operating with zero cloud dependencies or external API surface.
- **Ranking Engine:** Features a custom 6-factor task priority model with dependency cycle detection and a local-first NLP parser for understanding temporal conflicts.
- **Voice UI:** Implements offline speech-to-text and text-to-speech engine utilizing Vosk, triggered by a custom local wake word.

#### [Dataset Integrity Checker](https://github.com)
*FastAPI, SQLAlchemy, React, Tailwind, JWT + Argon2*
- **ML Supply Chain Security:** Audits incoming training datasets for label-poisoning vectors before ingestion into biometric classifiers.
- **Defensive Calibration:** Flags class imbalances and structural duplication, calculating high/medium/low integrity risk scores alongside accuracy-loss projections verified against empirical clean-vs-poisoned classifier testing.

#### [Blockchain Certificate Verification System](https://github.com)
*Python, Terminal UI (Colorama)*
- **Cryptographic Ledgers:** Simulates a tamper-evident blockchain ledger to verify graduate credentials, where any unauthorized field modification instantly invalidates downstream block hashes.

---

## 🔒 Security Commitments Across My Work
- **Input Hardening:** Parameterized SQL queries, zero usage of unsafe evaluation blocks (e.g., `dangerouslySetInnerHTML`), and XML-escaped data boundaries.
- **Traffic Protection:** Context-specific Content Security Policies (CSP) and strict localhost-binding defaults for investigation sandboxes.
- **Log Hygiene:** Automated regex scrubbing to guarantee no API keys, tokens, or credential hashes are exposed to environment stdout or disk logging.

---

## 📬 Contact & Professional Links

- **Email:** adeoluwa23joshua@gmail.com
- **LinkedIn:** [://linkedin.com](https://://linkedin.com)
- **Company Website:** [nemsec.com.ng](https://nemsec.com.ng)
