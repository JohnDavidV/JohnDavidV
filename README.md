# Hi, I'm John David Vásquez 👋

**Full-stack developer** based in Colombia. I build and run the software a private security company depends on every day: a **mobile app published on Google Play** (ready for the App Store), the APIs behind it, web platforms for HR, billing and suppliers, **AI agents that run on-premise**, and the Windows/SQL Server infrastructure they all live on.

I like taking legacy systems that "just work" and making them **secure, observable and deployable with one command**, without stopping the business.

```
📱 Mobile        React Native · Expo · offline-first sync · GPS/geofencing · camera/QR/NFC · FCM · Play Store / App Store
🧩 Backend       Node.js · Express · TypeScript · Python · FastAPI · REST · WebSockets
🟦 .NET          VB.NET · C# · ASP.NET WebForms · ASP.NET Core · .NET Framework 4.8 / .NET 8 · ADO.NET · IIS
🗄️ Data          SQL Server · T-SQL · Prisma · Drizzle · SQLite · query tuning · backup/restore · cross-server migrations
🤖 AI            Local LLMs with Ollama · OCR (Tesseract, PyMuPDF) · grounded generation · document extraction
🛠️ Ops           IIS · NSSM services · PowerShell automation · Git-based deployments · CI (GitHub Actions, Codemagic)
🔐 Security      Hash migrations (PBKDF2) · secrets out of source · signed links · webhook signatures · least privilege
```

## What I've shipped in production

- **Field operations mobile app** (React Native). Shifts, geofenced check-in with selfie validation, patrol rounds with NFC/QR, incident reports, payroll self-service and push notifications. It works **offline** with a durable sync queue and is published on **Google Play**, with the iOS build ready for the App Store.
- **REST API for the app** (Node.js + SQL Server on IIS). More than 20 business modules, JWT, scheduled jobs, PDF generation and structured per-module logs with request IDs.
- **WhatsApp helpdesk** (Express, Prisma, Socket.IO, React). A bot menu that routes customers to several departments, live agent inbox, business hours, and dashboards.
- **On-premise AI agents** (Python, FastAPI, Ollama, OCR). Supplier invoice intake, accounting exports and billing files. They replaced hours of manual data entry and keep the data on the company's servers.
- **LLM-written executive reports** for clients, with every figure validated against the database.
- **Legacy modernization.** I moved hard-coded credentials into protected configuration, migrated plain-text passwords to salted hashes without forced resets, rewrote classic ASP endpoints, and added dev/prod profiles.
- **Infrastructure migration.** I moved the apps and databases to a new server (SQL Server 2016 → 2022, new IIS layout), with resumable attachment copies, schema comparison and scripted, versioned deployments with rollback.

## Featured repositories

These are clean-room portfolio versions of the patterns behind that work. They are written from scratch, use synthetic data, and come with tests and CI.

| Repository | Stack | Highlights |
|---|---|---|
| [**fieldops-offline-mobile**](https://github.com/JohnDavidV/fieldops-offline-mobile) | React Native · Expo · TypeScript | Durable offline outbox (idempotency keys, per-entity ordering, backoff with jitter, crash recovery), single-flight token refresh, accuracy-aware geofencing. 41 tests. |
| [**node-mssql-api**](https://github.com/JohnDavidV/node-mssql-api) | Node.js · TypeScript · SQL Server · IIS | Mobile-app backend: injection-proof SQL template, migrations, one-open-shift index, refresh-token rotation, cron jobs with a distributed lock, FCM push, email, PDF reports, per-module logs. Integration tests run on a real SQL Server in CI. |
| [**whatsapp-helpdesk**](https://github.com/JohnDavidV/whatsapp-helpdesk) | Node · Express · Socket.IO · Drizzle · React · Tailwind | Bot menu editor, least-loaded agent routing, queues, business hours, HMAC-verified webhooks, real-time inbox and dashboard. 28 tests. |
| [**invoice-ai-extractor**](https://github.com/JohnDavidV/invoice-ai-extractor) | Python · FastAPI · Tesseract · Ollama | Rules first, then a *grounded* local LLM. Colombian NIT check-digit validation, OCR fallback, accuracy gate in CI. 41 tests. |
| [**llm-report-writer**](https://github.com/JohnDavidV/llm-report-writer) | Python · Ollama · ReportLab | Executive PDF reports where the LLM writes and a guard rejects invented numbers, overlong paragraphs and repeated closings. |
| [**supplier-portal-webforms-vb**](https://github.com/JohnDavidV/supplier-portal-webforms-vb) | VB.NET · ASP.NET WebForms · .NET Framework 4.8 · SQL Server | Supplier portal in VB.NET: parameterized ADO.NET, PBKDF2 with legacy upgrade, CSRF protection, signed certificate links, least-privilege SQL. CI builds on Windows and runs an IIS Express smoke test. 28 tests. |
| [**aspnet-legacy-auth-migration**](https://github.com/JohnDavidV/aspnet-legacy-auth-migration) | .NET 8 · C# · SQL Server | From plain-text passwords to PBKDF2 with transparent upgrade on login, HMAC-signed expiring links, lockout with backoff. 18 tests. |
| [**windows-server-ops-toolkit**](https://github.com/JohnDavidV/windows-server-ops-toolkit) | PowerShell · IIS · SQL Server | Versioned zero-downtime IIS releases with auto-rollback, NSSM service updates from Git, resumable migrations, schema diff. Pester tests. |

## Get in touch

📫 jh.deivy@gmail.com · 💼 [LinkedIn](https://www.linkedin.com/in/your-profile) <!-- TODO: replace with your LinkedIn URL -->

