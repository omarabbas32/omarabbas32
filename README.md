<h1 align="center">Omar Abbas</h1>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&duration=2800&pause=900&color=512BD4&center=true&vCenter=true&width=560&height=45&lines=Backend+C%23+%2F+.NET+Developer;ASP.NET+Core+%7C+EF+Core+%7C+Blazor;PostgreSQL+%7C+MySQL+%7C+Docker;Shipping+systems+real+clients+use+daily" alt="Backend C# / .NET Developer"/>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/omar-abbas-934086388">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="mailto:abbas8989omar@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
  <img src="https://img.shields.io/badge/Open_to_Remote_Work-2EA44F?style=for-the-badge" alt="Open to Remote Work"/>
</p>

<br/>

## About

Backend developer working in **C# / ASP.NET Core**, based in Egypt. I build production systems for real clients, currently a project-management, time-tracking and HR/payroll backend. I care about systems that stay maintainable as they grow: clear boundaries, predictable data access, and deployments that don't surprise anyone.

- Design REST APIs with **Clean Architecture**, **CQRS** (MediatR) and **FluentValidation**
- Build secure authentication: **JWT** with rotating refresh tokens, policy-based and dynamic permission-based authorization
- Ship real-time features with **SignalR** and interactive UIs with **Blazor Server**
- Model and tune databases with **EF Core** and **Dapper**: fixing N+1 queries, optimistic concurrency, migrations
- Build reliable background work: **outbox** sync, idempotent messaging, reconciliation jobs
- Deploy with **Docker** on VPS (Dokploy), and on IIS when the host requires it

Currently going deeper on **Redis caching, Azure, distributed systems, and performance engineering**.

<br/>

## Selected Work

### Project Management, Time Tracking & HR Platform &nbsp;<sub><i>Production · private repo</i></sub>
Backend for an agency: projects, file reviews and approvals, task time tracking, and HR attendance, leave and payroll.

- Built on **ASP.NET Core (.NET 9)** with **EF Core / PostgreSQL**, layered services and DTOs. The HR module was later refactored into **vertical slices** behind characterization tests
- **JWT** access and refresh tokens (stored hashed), role-based access, and **SignalR** notifications authenticated per user
- An **interval-merge "union time"** algorithm, so parallel tasks aren't double-counted. Auto-pause when a task exceeds its estimate
- Detected fingerprint-device errors that were causing false payroll deductions, with a unit-tested punch-pairing detector
- Fixed an **N+1** hotspot with bulk queries. Fixed production **CORS** errors that were hiding 500s. Rendered Arabic PDF reports
- Shipped with a multi-stage **Docker** build on a VPS (Dokploy). File storage on S3-compatible **Cloudflare R2**

<img src="https://img.shields.io/badge/C%23-239120?style=flat-square&logo=c-sharp&logoColor=white" alt="C#"/>
<img src="https://img.shields.io/badge/ASP.NET_Core-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt="ASP.NET Core"/>
<img src="https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/SignalR-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt="SignalR"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker"/>

### Car Rental Web API
A car rental marketplace API with renters, owners, bookings and live updates.

- **Clean Architecture + CQRS** with MediatR and a **FluentValidation** pipeline behavior
- **EF Core / PostgreSQL**, **JWT** with rotating refresh tokens and BCrypt, **SignalR** notifications, Cloudinary for images
- Security hardening: blocked self-registration as Admin, took the user's identity from the token instead of the request body (IDOR), removed secrets from Git with a CI check
- Correct HTTP semantics: **409** for conflicts, **404** for missing resources, **401** for unauthenticated requests. Swagger docs

<img src="https://img.shields.io/badge/C%23-239120?style=flat-square&logo=c-sharp&logoColor=white" alt="C#"/>
<img src="https://img.shields.io/badge/ASP.NET_Core-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt="ASP.NET Core"/>
<img src="https://img.shields.io/badge/CQRS-4B6584?style=flat-square" alt="CQRS"/>
<img src="https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
&nbsp;
<a href="https://github.com/omarabbas32/CarRentalWebApp"><img src="https://img.shields.io/badge/Source-181717?style=flat-square&logo=github&logoColor=white" alt="Source"/></a>

### Store Builder Platform
Backend for a multi-store platform that manages stores, products and user operations.

- Built REST APIs for store, product and user operations, integrated with the frontend team
- Modelled the PostgreSQL schema with Prisma ORM, using migrations to keep environments in sync
- Backend work outside the .NET stack, in Node.js

<img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white" alt="Node.js"/>
<img src="https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>
<img src="https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
&nbsp;
<a href="https://github.com/omarabbas32/StoreBuilder"><img src="https://img.shields.io/badge/Source-181717?style=flat-square&logo=github&logoColor=white" alt="Source"/></a>

<br/>

## Tech Stack

<table>
  <tr>
    <td><b>Languages&nbsp;&amp;&nbsp;Frameworks</b></td>
    <td>
      <img src="https://img.shields.io/badge/C%23-239120?style=flat-square&logo=c-sharp&logoColor=white" alt="C#"/>
      <img src="https://img.shields.io/badge/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt=".NET"/>
      <img src="https://img.shields.io/badge/ASP.NET_Core-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt="ASP.NET Core"/>
      <img src="https://img.shields.io/badge/Blazor-512BD4?style=flat-square&logo=blazor&logoColor=white" alt="Blazor"/>
      <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white" alt="Node.js"/>
      <img src="https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white" alt="Express.js"/>
    </td>
  </tr>
  <tr>
    <td><b>Architecture&nbsp;&amp;&nbsp;Patterns</b></td>
    <td>
      <img src="https://img.shields.io/badge/Clean_Architecture-2F4858?style=flat-square" alt="Clean Architecture"/>
      <img src="https://img.shields.io/badge/CQRS_·_MediatR-4B6584?style=flat-square" alt="CQRS / MediatR"/>
      <img src="https://img.shields.io/badge/Vertical_Slices-4B6584?style=flat-square" alt="Vertical Slices"/>
      <img src="https://img.shields.io/badge/Outbox_Pattern-4B6584?style=flat-square" alt="Outbox Pattern"/>
      <img src="https://img.shields.io/badge/REST_APIs-0F9D58?style=flat-square" alt="REST APIs"/>
      <img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white" alt="JWT"/>
      <img src="https://img.shields.io/badge/SignalR-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt="SignalR"/>
    </td>
  </tr>
  <tr>
    <td><b>Databases&nbsp;&amp;&nbsp;ORMs</b></td>
    <td>
      <img src="https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
      <img src="https://img.shields.io/badge/MySQL-005C84?style=flat-square&logo=mysql&logoColor=white" alt="MySQL"/>
      <img src="https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white" alt="SQL Server"/>
      <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white" alt="MongoDB"/>
      <img src="https://img.shields.io/badge/EF_Core-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt="EF Core"/>
      <img src="https://img.shields.io/badge/Dapper-6E4C9E?style=flat-square" alt="Dapper"/>
      <img src="https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white" alt="Prisma"/>
    </td>
  </tr>
  <tr>
    <td><b>Testing</b></td>
    <td>
      <img src="https://img.shields.io/badge/xUnit-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt="xUnit"/>
      <img src="https://img.shields.io/badge/Shouldly-512BD4?style=flat-square" alt="Shouldly"/>
      <img src="https://img.shields.io/badge/Integration_Tests-0F9D58?style=flat-square" alt="Integration Tests"/>
    </td>
  </tr>
  <tr>
    <td><b>Tools&nbsp;&amp;&nbsp;DevOps</b></td>
    <td>
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker"/>
      <img src="https://img.shields.io/badge/IIS-5E5E5E?style=flat-square&logo=windows&logoColor=white" alt="IIS"/>
      <img src="https://img.shields.io/badge/Cloudflare_R2-F38020?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare R2"/>
      <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git"/>
      <img src="https://img.shields.io/badge/Swagger-85EA2D?style=flat-square&logo=swagger&logoColor=black" alt="Swagger"/>
      <img src="https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white" alt="Postman"/>
    </td>
  </tr>
</table>

<br/>

## GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=omarabbas32&show_icons=true&theme=github_dark&hide_border=true&title_color=512BD4&icon_color=512BD4&count_private=true" height="165" alt="GitHub stats"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=omarabbas32&layout=compact&theme=github_dark&hide_border=true&title_color=512BD4" height="165" alt="Top languages"/>
</p>

<br/>

## Contact

**Email**: [abbas8989omar@gmail.com](mailto:abbas8989omar@gmail.com) &nbsp;·&nbsp; **LinkedIn**: [omar-abbas](https://www.linkedin.com/in/omar-abbas-934086388)

Open to **remote** backend roles and full-time contract work. I'm in Egypt (UTC+2/+3), which overlaps with European working hours.

<br/>

<p align="center"><i>Backend first. Architecture driven. Performance aware.</i></p>
