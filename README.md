<h1 align="center">Miguel Ángel Núñez Silva</h1>
<p align="center">Encargado Informático LIMS · Minería · Integración de sistemas industriales<br/>
<sub>LIMS IT Lead · Mining · Industrial systems integration</sub></p>

<p align="center">
  <!-- TODO: reemplazar "#" por los links reales -->
  <a href="#"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="#"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

---

<details open>
<summary><b>Español</b> <sub>(clic para contraer)</sub></summary>

### Sobre mí

Ingeniero a cargo de sistemas críticos en la industria minera, en Calama, Chile. Administro el LIMS del Laboratorio Químico de Codelco División Radomiro Tomic, integro equipos analíticos con AVEVA PI System y desarrollo software a medida para la operación: inventario, KPIs, reportes y dashboards automatizados.

### Proyectos

#### Sistema de Inventario EPP – DRT
Aplicación web progresiva (PWA) para controlar el inventario de elementos de protección personal del laboratorio. Registra entradas, salidas y stock crítico, permite que los trabajadores soliciten EPP escaneando un código QR e importa y exporta datos en Excel. Es online-first, pero guarda una caché local en IndexedDB para zonas con poca señal. Los permisos se aplican en la base de datos con RLS y funciones SECURITY DEFINER para cuatro roles, y las Edge Functions administran usuarios y envían avisos de solicitudes.

**Stack:** React 19 · React Router 7 · Vite 8 · JavaScript · CSS/SVG propios · Service Worker · IndexedDB (idb) · Supabase (Postgres, Auth, RLS, Edge Functions en Deno) · SheetJS · qrcode · Vercel · ESLint

#### Asistencia FTE / HH – DRT
Sistema web de control de asistencia y cálculo de FTE y horas hombre por área. Tiene login propio con sesiones por token, cuatro roles (Admin, ADP, RRHH, Supervisor) con alcance por área, Cloudflare Turnstile y límite de intentos de login. Genera planillas Excel con un generador .xlsx escrito desde cero e incluye respaldos cifrados con AES-GCM y PBKDF2. Corre completo sobre Cloudflare, sin frameworks ni dependencias npm.

**Stack:** HTML · CSS · JavaScript puro · Cloudflare Pages · Cloudflare Workers · Cloudflare D1 (SQLite) · Cloudflare R2 · Wrangler · Node.js (node --test) · Python + openpyxl · *Repositorio privado*

#### RADIM – Unificación de sistemas de información minera DRT
Plataforma que reúne en una sola aplicación los datos de procesos de la división (DRT, SX-EW y lingadas). Consulta en vivo e historial de AVEVA PI System, cálculo de promedios, carga de CSV y exportación a Excel, con gráficos interactivos. Incluye autenticación JWT con roles, contraseñas con bcrypt, bloqueo por intentos fallidos y auditoría. Se usa como aplicación de escritorio mediante pywebview y está preparada para conectarse a Oracle.

**Stack:** Python 3.12 · FastAPI · Uvicorn · Pydantic · SQLite · JWT (python-jose) · passlib/bcrypt · PISDK (pywin32) · PIconnect · pandas · openpyxl · HTML/CSS/JS · Chart.js · pywebview · PyInstaller · *Repositorio privado*

#### Puente EAA – Integración de equipos analíticos con SampleManager LIMS
Aplicación de escritorio para Windows que conecta los equipos de absorción atómica (EAA) con SampleManager LIMS 21.3 sin tocar la base de datos. Lee los archivos de resultados del equipo y las hojas de etiquetas, detecta los lotes, y escribe archivos en una carpeta vigilada que procesa el Parsing Script del LIMS. Cada operación queda en una bitácora con hash SHA-256. Tiene módulos para Pb Cátodos, Soluciones y Orgánicos. Compila a un solo .exe sin dependencias externas, con un paquete de entrega preparado para revisión de ciberseguridad.

**Stack:** C# · .NET Framework 4.0 · Windows Forms · GDI+ · csc.exe (sin MSBuild/NuGet) · FileSystemWatcher · SHA-256 · archivos .ini

### Experiencia

**Encargado Informático LIMS** — SGS
*Abr. 2025 – actualidad · Calama, Región de Antofagasta, Chile · Presencial*
- Administración del gestor de muestras SampleManager LIMS del Laboratorio Químico de Codelco División Radomiro Tomic.
- Integración de equipos analíticos y sistemas informáticos con AVEVA PI System.
- Administración y consulta de bases de datos Oracle; monitoreo de información crítica para la operación.
- Creación de reportes y dashboards automatizados en Excel mediante PI DataLink.
- Desarrollo de software para minería: gestor de inventario, automatización de KPIs e informes automáticos.
- Soporte técnico general y apoyo a la continuidad de sistemas del laboratorio.
- Uso de herramientas de IA como Claude Code, Codex, OpenCode y Antigravity.

**Soporte TI (Práctica profesional)** — Centro Educacional de Alta Tecnología
*May. 2023 – jul. 2023 · San Pedro de la Paz, Biobío, Chile · Presencial*
- Soporte TI y administración de Linux Virtual Server.

</details>

<details>
<summary><b>English</b> <sub>(click to expand)</sub></summary>

### About me

Engineer in charge of critical systems in the mining industry, based in Calama, Chile. I manage the LIMS of the Chemical Laboratory at Codelco Radomiro Tomic Division, integrate analytical instruments with AVEVA PI System, and build custom software for operations: inventory, KPIs, reports and automated dashboards.

### Projects

#### PPE Inventory System – DRT
Progressive web app (PWA) that tracks the laboratory's personal protective equipment inventory. It records stock in and out and critical stock levels, lets workers request PPE by scanning a QR code, and imports and exports Excel data. It is online-first but keeps a local IndexedDB cache for areas with poor signal. Permissions are enforced in the database with RLS and SECURITY DEFINER functions for four roles, and Edge Functions handle user management and request notifications.

**Stack:** React 19 · React Router 7 · Vite 8 · JavaScript · custom CSS/SVG · Service Worker · IndexedDB (idb) · Supabase (Postgres, Auth, RLS, Deno Edge Functions) · SheetJS · qrcode · Vercel · ESLint

#### FTE / Man-Hours Attendance – DRT
Web system for attendance tracking and FTE and man-hour calculation by area. It has its own login with token sessions, four roles (Admin, ADP, HR, Supervisor) scoped by area, Cloudflare Turnstile and login rate limiting. It produces Excel sheets with an .xlsx generator written from scratch and includes backups encrypted with AES-GCM and PBKDF2. It runs entirely on Cloudflare, with no frameworks or npm dependencies.

**Stack:** HTML · CSS · vanilla JavaScript · Cloudflare Pages · Cloudflare Workers · Cloudflare D1 (SQLite) · Cloudflare R2 · Wrangler · Node.js (node --test) · Python + openpyxl · *Private repository*

#### RADIM – Mining information systems unification, DRT
Platform that brings the division's process data (DRT, SX-EW and copper bundles) into a single application. It provides live and historical AVEVA PI System queries, averages, CSV upload and Excel export, with interactive charts. It includes JWT authentication with roles, bcrypt passwords, lockout after failed attempts and an audit log. It runs as a desktop app through pywebview and is ready to connect to Oracle.

**Stack:** Python 3.12 · FastAPI · Uvicorn · Pydantic · SQLite · JWT (python-jose) · passlib/bcrypt · PISDK (pywin32) · PIconnect · pandas · openpyxl · HTML/CSS/JS · Chart.js · pywebview · PyInstaller · *Private repository*

#### EAA Bridge – Analytical instrument integration with SampleManager LIMS
Windows desktop app that connects atomic absorption (AAS) instruments to SampleManager LIMS 21.3 without touching the database. It reads the instrument's result files and label sheets, detects batches, and writes files to a watched folder that the LIMS Parsing Script processes. Every operation is logged with a SHA-256 hash. It has modules for Pb Cathodes, Solutions and Organics. It compiles to a single .exe with no external dependencies, plus a delivery package prepared for cybersecurity review.

**Stack:** C# · .NET Framework 4.0 · Windows Forms · GDI+ · csc.exe (no MSBuild/NuGet) · FileSystemWatcher · SHA-256 · .ini files

### Experience

**LIMS IT Lead** — SGS
*Apr 2025 – present · Calama, Antofagasta Region, Chile · On-site*
- Administration of the SampleManager LIMS at the Chemical Laboratory of Codelco Radomiro Tomic Division.
- Integration of analytical instruments and IT systems with AVEVA PI System.
- Oracle database administration and querying; monitoring of operation-critical data.
- Automated Excel reports and dashboards with PI DataLink.
- Software development for mining: inventory manager, KPI automation and automated reports.
- General technical support and continuity of laboratory systems.
- Use of AI tools such as Claude Code, Codex, OpenCode and Antigravity.

**IT Support (Internship)** — Centro Educacional de Alta Tecnología
*May 2023 – Jul 2023 · San Pedro de la Paz, Biobío, Chile · On-site*
- IT support and Linux Virtual Server administration.

</details>

---

### Lenguajes y herramientas · Languages & Tools

<p>
  <img src="https://skillicons.dev/icons?i=py,cs,dotnet,js,ts,html,css,powershell" alt="Lenguajes"/><br/>
  <img src="https://skillicons.dev/icons?i=react,vite,nextjs,tailwind,nodejs,fastapi,deno,electron" alt="Frameworks"/><br/>
  <img src="https://skillicons.dev/icons?i=sqlite,postgres,supabase,cloudflare,vercel,git,github,vscode" alt="Datos / Infra"/>
</p>
<p>
  <img src="https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white" alt="Oracle"/>
  <img src="https://img.shields.io/badge/AVEVA%20PI%20System-0067B1?style=for-the-badge" alt="AVEVA PI System"/>
  <img src="https://img.shields.io/badge/SampleManager%20LIMS-4B5563?style=for-the-badge" alt="SampleManager LIMS"/>
  <img src="https://img.shields.io/badge/Excel%20%2F%20PI%20DataLink-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" alt="Excel / PI DataLink"/>
  <img src="https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white" alt="Chart.js"/>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux"/>
</p>
