## Technology / Project exchange - May 9, 2018
---
### Projects in Angular / WebAPI
- DealerCenter NG
  - Retail Deal
  - Desking
  - Deal filter
  - Report scheduler
- WFS Marketing
- CULA

---
### Technology
- Client-side
  - Angular
  - Kendo UI
- Server-side
  - ASP.net WebAPI
  - Swagger (open API)
- Test Automation
  - Protractor (E2E testing)

---
### Technology (cont'd)
- Hosting server
  - NGINX in Docker Container hosted on Kubernetes (Angular app)
  - IIS hosted on Windows server (ASP.net)
- Build and Deployment pipeline
  - Jenkins
---
### Technology (cont'd)
- Source control
  - GIT (in TFS and GitHub)
- IDE
  - Visual Studio Code
  - Visual Studio 2017

---
Demo - Desking

---?image=assets/servers.png&title=Server Setup&size=70% auto&color=white

---

### WebAPI - reused from DMSAPP
- Use swashbuckle for generating the open API doc
- Use swagger for client proxy generation
- Create separate DTO classes
- DateTime in open API - https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.1.md#dataTypes
- Enums are created manually

---

### Overall approach for Angular app
- Define module (lazy-loading unit)
- Define component list
- Identify container / presentation components
- Note on form - reactive form
- Be proficient with rxjs - you'll need that. See exercise at https://github.com/NowcomCorporation/playground-rxjs
---

### Notes on Angular components
- Communication from Parent to Child via @Input
- Communication from Child to Parent via Event (@Output) 
- Avoid non-presentation-related state in components
- Use immutable objects
- Utilize async pipe with observables
- Use OnPush change detection as default

---

### Notes on Angular services / DI
- Used for state management
- Lifetime can be longer than the page component
- Be aware of the Dependency Injection scope
- In consideration of adopting NGRX

---

### Notes on VS Code
- Ensure you have the following extensions:
  - TSLint
  - Angular Language Service
  - GitLens
