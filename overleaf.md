::: center
**[Nguyen Van Tai]{.smallcaps}**\
+84 37 351 7718 $|$
[[nvtai24work@gmail.com]{.underline}](mailto:nvtai24work@gmail.com) $|$
[[github.com/nvtai24]{.underline}](https://github.com/nvtai24) $|$
[[nvtai24.site]{.underline}](https://nvtai24.site)
:::

# Summary

::: justify
Recent Software Engineering graduate with a strong passion for backend
development and software architecture. I enjoy learning new
technologies, solving challenging problems, and continuously improving
my technical skills while building reliable and maintainable software
solutions.
:::

# Education

- ------------------------------------ ----------------------
    **FPT University**                     Oct 2022 -- Sep 2026
    *Bachelor of Software Engineering*       *GPA: **3.6/4.0***
    ------------------------------------ ----------------------

# Experience

- -------------------------------------------------- ----------------------
    **National Citizen Commercial Joint Stock Bank**     May 2025 -- Sep 2025
    *Backend Developer Intern*                         
    -------------------------------------------------- ----------------------

  -  Analyzed banking business requirements and technical documentation
    to design and implement backend solutions that met functional
    requirements while ensuring code quality and maintainability.

  -  Developed and maintained **secure RESTful APIs** using Java Spring
    Boot, ensuring strict compliance with the bank's data security and
    transaction integrity standards.

  -  Collaborated effectively with cross-functional teams (including
    Business Analysts and QA) to clarify requirements, write unit tests,
    and resolve technical bugs during the UAT (User Acceptance Testing)
    phase.

- ----------------- ---------------------
    **FPTU IA Lab**     Apr 2026 -- Present
    *Developer*       
    ----------------- ---------------------

  -  Maintained a Kubernetes-based microservices CTF platform (FCTF),
    shipping **200+ fixes/improvements** to the contest--challenge
    lifecycle (dynamic deployment, cleanup jobs, stop-all with retry
    logic).

  -  Redesigned core database schema and wrote production-safe Alembic
    migrations for MySQL with **zero downtime**

  -  Set up and managed cloud infrastructure on Google Cloud for
    development and testing, and built **automated CI/CD pipelines**
    with GitHub Actions to streamline the build-and-deploy workflow.

# Projects

- --------------------------------------------------------------------------------------------------------- -----------------------------
    [**[FCTF]{.underline}**](https://github.com/hoaanhtuc113/FCTF) -- Scalable CTF Competition Platform                 Jun 2025 -- Present
    **Technologies**: *ASP.NET Core, Go, React, MariaDB, Redis, RabbitMQ, Kubernetes (K3s), Argo Workflows*     [[Live Demo]{.underline}]()
    --------------------------------------------------------------------------------------------------------- -----------------------------

  -  Built a **microservices CTF platform** for large-scale
    competitions. It includes a React 19 + TypeScript contestant portal,
    ASP.NET Core (.NET 8) backend services, and an admin control center
    based on CTFd (Flask), all backed by MariaDB.

  -  Created **on-demand challenge deployment**: each team gets its own
    challenge instance, started through RabbitMQ and Argo Workflows. A
    Kubernetes watcher service tracks each instance's status, and
    instances run sandboxed with **gVisor** and NetworkPolicy isolation.

  -  Wrote a **Challenge Gateway in Go** that forwards HTTP and TCP
    traffic to challenge instances. It checks each request's token and
    applies rate limits using Redis Lua scripts.

  -  Secured the APIs with JWT authentication and token revocation,
    Redis-backed rate limiting, and Cloudflare Turnstile. Fixed **race
    conditions** in flag submission, hint unlocking and challenge
    start/stop.

  -  Deployed on a **multi-node K3s cluster** with Helm, **autoscaling
    (HPA)**, NFS storage, cert-manager and Harbor as the private image
    registry. Built CI/CD with GitHub Actions that builds images, pushes
    them to Harbor and rolls them out with kubectl. Added monitoring
    with Prometheus, Grafana and Loki.

  -  Validated performance and correctness with **k6** load, stress,
    spike, soak and concurrency tests. Wrote a **Python migration tool**
    that moves data between CTFd and FCTF.

- -------------------------------------------------------------------------------------------------------------------------------------------- -------------------------------------------------------------------------------------------
    [**[DealMind]{.underline}**](https://github.com/nvtai24/dealmind) -- AI sales training platform with role-play, fact-checking, and scoring                                                                          Sep 2026 -- Oct 2026
    **Technologies**: *FastAPI, Next.js, PostgreSQL (pgvector), OpenAI API, Docker, GCP*                                                           https://dealmind.nvtai24.cloud/[[Live Demo]{.underline}](https://dealmind.nvtai24.cloud/)
    -------------------------------------------------------------------------------------------------------------------------------------------- -------------------------------------------------------------------------------------------

  -  Built an **AI-powered sales training platform** for real-estate
    agents (role-play calls with an AI customer, fact-checking claims
    against project documents, evidence-based scoring) with FastAPI,
    Next.js (App Router) and PostgreSQL + pgvector, as part of a
    **6-person team**

  -  Designed a code-first database schema with SQLAlchemy and Alembic
    migrations, and implemented **multi-tenant role-based access**
    (platform admin, company admin, team lead, sales) with
    admin-provisioned accounts and **per-tenant data isolation**

  -  Developed **REST APIs and dashboards for every role**:
    user/team/project management, document library, customer personas,
    versioned scoring rubrics and audit logs for admins; review queues,
    score overrides and assignments for leads; training paths,
    certifications and session reports for trainees

  -  Integrated MinIO (S3-compatible) object storage for project
    documents and recorded call audio

  -  Deployed with Docker Compose to a GCP Compute Engine VM behind
    Caddy (automatic HTTPS), with a GitHub Actions pipeline (lint,
    migration checks, **500+ tests**) on a self-hosted runner and
    **keyless deploys** via Workload Identity Federation; added
    pre-deploy database/storage backups and a web log viewer

- -------------------------------------------------------------------------------------------------------------------------------------- -----------------------------
    [**[MyQuiz]{.underline}**](https://github.com/nvtai24/myquiz-be) -- AI-powered quiz generation and flashcard-based learning platform            Dec 2025 -- Jan 2026
    **Technologies**: *ASP.NET Core, PostgreSQL, Redis, MediatR, OpenAI API, Docker*                                                         [[Live Demo]{.underline}]()
    -------------------------------------------------------------------------------------------------------------------------------------- -----------------------------

  -  Designed and built the backend of an AI-powered quiz-generation
    platform with ASP.NET Core 8 using **Clean Architecture**
    (Domain/Application/Infrastructure) and **CQRS** via MediatR

  -  Built an **AI quiz-generation pipeline** that extracts text from
    uploaded PDF/DOCX files and streams AI-generated questions to the
    client **in real time** using the OpenAI API and Server-Sent Events

  -  Implemented **JWT + refresh-token authentication** with ASP.NET
    Identity, Google OAuth2 login, and role-based authorization for
    Admin/User access

  -  Integrated PostgreSQL (EF Core) for persistence, Redis for rate
    limiting, AWS S3 for file storage, and a **subscription/payment
    module** with SePay webhook integration and a background job to
    auto-expire pending transactions

# Technical Skills

::: itemize
**Languages**: Java, C#, JavaScript/TypeScript, Dart, SQL\
**Frontend**: HTML, CSS, Bootstrap, TailwindCSS, jQuery, React\
**Backend**: Spring Boot, ASP.NET Core, RabbitMQ\
**Database**: SQL Server, MySQL, PostgreSQL, Redis\
**DevOps**: Git, Docker, CI/CD, Google Cloud\
:::
