![React](https://img.shields.io/badge/React-19-B63D20?style=for-the-badge&logo=react&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-171714?style=for-the-badge&logo=typescript&logoColor=white)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-10-B63D20?style=for-the-badge&logo=dotnet&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-171714?style=for-the-badge)
![Azure](https://img.shields.io/badge/Azure-B63D20?style=for-the-badge)

# Dynamic Construction

Developed as a group academic project.

## Overview

Dynamic Construction combines a public website, client portal and staff workspace. It supports estimates, quotations, project tracking, documents and financial records, with role-based access and administrative controls.

## Project links

| Resource | Location |
|---|---|
| Hosted application | [Open the live application](https://app-dc-pilot-kc023-bhesg0a5g8ewhken.southafricanorth-01.azurewebsites.net/) |
| Demo video | [Watch the demonstration](https://youtu.be/r0GW_skkptA) |
| Build and deployment configuration | [CI workflow](./.github/workflows/ci.yml) |
| Code attribution | [CODE_ATTRIBUTION.txt](./CODE_ATTRIBUTION.txt) |


## Application screenshots

Select an image to open it at full size. Expand the galleries below for additional screens. Application captures were refreshed on **20 October 2026**. The public portfolio capture shows the live site's project photo panels; account and workflow screens use fictional local demonstration records and illustrative prices.

**Public Website**

[![Public Website](./docs/screenshots/public-website.jpg)](./docs/screenshots/public-website.jpg)

<details>
<summary><strong>Public portfolio</strong></summary>

**Public Portfolio**

[![Public Portfolio](./docs/screenshots/public-portfolio.jpg)](./docs/screenshots/public-portfolio.jpg)

</details>

<details>
<summary><strong>Three-step quote builder, validation and custom requests</strong></summary>

**Quote Calculated Estimate**

[![Quote Calculated Estimate](./docs/screenshots/quote-calculated-estimate.jpg)](./docs/screenshots/quote-calculated-estimate.jpg)

**Quote Validation**

[![Quote Validation](./docs/screenshots/quote-validation.jpg)](./docs/screenshots/quote-validation.jpg)

**Quote Contact Details**

[![Quote Contact Details](./docs/screenshots/quote-contact-details.jpg)](./docs/screenshots/quote-contact-details.jpg)

**Quote Review**

[![Quote Review](./docs/screenshots/quote-review.jpg)](./docs/screenshots/quote-review.jpg)

**Quote Confirmation**

[![Quote Confirmation](./docs/screenshots/quote-confirmation.jpg)](./docs/screenshots/quote-confirmation.jpg)

**Custom Project Request**

[![Custom Project Request](./docs/screenshots/quote-custom-request.jpg)](./docs/screenshots/quote-custom-request.jpg)

</details>

<details>
<summary><strong>Account validation and trusted-device MFA</strong></summary>

**Client Registration Validation**

[![Client Registration Validation](./docs/screenshots/account-validation.jpg)](./docs/screenshots/account-validation.jpg)

**Authenticator Sign-in**

[![Authenticator Sign-in](./docs/screenshots/account-mfa.jpg)](./docs/screenshots/account-mfa.jpg)

**Forget This Device**

[![Forget This Device](./docs/screenshots/account-security.jpg)](./docs/screenshots/account-security.jpg)

</details>

<details>
<summary><strong>Client project, published progress and documents</strong></summary>

**Client Overview**

[![Client Overview](./docs/screenshots/client-overview.jpg)](./docs/screenshots/client-overview.jpg)

**Client Project Overview**

[![Client Project Overview](./docs/screenshots/client-project-overview.jpg)](./docs/screenshots/client-project-overview.jpg)

**Client Progress**

[![Client Progress](./docs/screenshots/client-progress.jpg)](./docs/screenshots/client-progress.jpg)

**Client Documents**

[![Client Documents](./docs/screenshots/client-documents.jpg)](./docs/screenshots/client-documents.jpg)

**Client Change History**

[![Client Change History](./docs/screenshots/client-change-history.jpg)](./docs/screenshots/client-change-history.jpg)

**Client Notifications**

[![Client Notifications](./docs/screenshots/client-notifications.jpg)](./docs/screenshots/client-notifications.jpg)

**Client Project List**

[![Client Project List](./docs/screenshots/client-project-list.jpg)](./docs/screenshots/client-project-list.jpg)

</details>

<details>
<summary><strong>Staff quotation and project workspace</strong></summary>

**Staff Quotation**

[![Staff Quotation](./docs/screenshots/staff-quotation.jpg)](./docs/screenshots/staff-quotation.jpg)

**Staff Operations**

[![Staff Operations](./docs/screenshots/staff-operations.jpg)](./docs/screenshots/staff-operations.jpg)

**Staff Progress**

[![Staff Progress](./docs/screenshots/staff-progress.jpg)](./docs/screenshots/staff-progress.jpg)

**Staff Documents**

[![Staff Documents](./docs/screenshots/staff-documents.jpg)](./docs/screenshots/staff-documents.jpg)

**Staff Project Overview**

[![Staff Project Overview](./docs/screenshots/staff-project-overview.jpg)](./docs/screenshots/staff-project-overview.jpg)

**Staff Change Decision**

[![Staff Change Decision](./docs/screenshots/staff-change-decision.jpg)](./docs/screenshots/staff-change-decision.jpg)

</details>

<details>
<summary><strong>Budgets, invoices, paid amounts and outstanding balances</strong></summary>

**Staff Finance**

[![Staff Finance](./docs/screenshots/staff-finance.jpg)](./docs/screenshots/staff-finance.jpg)

**Client Finance**

[![Client Finance](./docs/screenshots/client-finance.jpg)](./docs/screenshots/client-finance.jpg)

</details>

<details>
<summary><strong>Mobile layout</strong></summary>

**Mobile Public Home**

<a href="./docs/screenshots/mobile-public-home.jpg"><img src="./docs/screenshots/mobile-public-home.jpg" alt="Mobile Public Home" width="320" /></a>

**Mobile Public Navigation**

<a href="./docs/screenshots/mobile-public-navigation.jpg"><img src="./docs/screenshots/mobile-public-navigation.jpg" alt="Mobile Public Navigation" width="320" /></a>

**Mobile Quote Builder**

<a href="./docs/screenshots/mobile-quote-builder.jpg"><img src="./docs/screenshots/mobile-quote-builder.jpg" alt="Mobile Quote Builder" width="320" /></a>

**Mobile Client Overview**

<a href="./docs/screenshots/mobile-client-overview.jpg"><img src="./docs/screenshots/mobile-client-overview.jpg" alt="Mobile Client Overview" width="320" /></a>

**Mobile Client Navigation**

<a href="./docs/screenshots/mobile-client-navigation.jpg"><img src="./docs/screenshots/mobile-client-navigation.jpg" alt="Mobile Client Navigation" width="320" /></a>

</details>

## Hosting services

The original application uses Azure services in South Africa North.

| Service | Configuration and purpose |
|---|---|
| Azure App Service | Linux, .NET 10; serves the frontend and API from one HTTPS origin. |
| App Service plan | F1 (Free), one instance. |
| Azure SQL Database | General Purpose, serverless Gen5, 2 vCores under the free offer; stores application records. |
| Azure Blob Storage | Standard locally redundant storage (LRS); private project documents and protected identity keys. |
| Azure Key Vault | Standard tier; protects the identity key ring's encryption key. |
| Application Insights | Request telemetry, failures and server response times. |


## Features

| Area | Functionality |
|---|---|
| Public website | Services, staged project photographs with playback controls, published portfolio details, contact and enquiries. |
| Estimates | Boundary wall, concrete deck, gunite pool and room addition calculations using published server-managed rates. The three-step pop-up includes interactive build drawings, dimensions, contact details, review and confirmation. Estimates retain pricing assumptions and rate versions. |
| Custom requests | **Something else** requests capture a project description for pricing after a site assessment. Unpublished rates also produce an unpriced request. |
| Client portal | Linked projects, published milestones, progress, documents, financial summaries and change requests. |
| Project operations | Quotation review and acceptance, project conversion, lifecycle transitions, milestones, progress publication and document access. |
| Finance | Budgets, invoices, paid amounts and outstanding balances with validation and concurrency checks. |
| Administration | Accounts, roles, suspension, notifications, audit records, pricing and public content. |
| Account access | Immediate sign-up and sign-in field validation, authenticator MFA, optional seven-day device trust, device forgetting and recovery codes. |
| Interface | Rust-and-charcoal branding, responsive layouts, labelled forms, keyboard interaction and loading, error and confirmation states. |
| Performance | Quote builder and portal features load on demand. Public build assets use response compression and long-lived caching for versioned assets. |

Estimates are indicative; final pricing requires a formal quotation. Public registration creates client accounts. Finance features record transactions; they do not process online payments.

### Selected improvements

| Area | Current implementation |
|---|---|
| Quotation experience | Homepage estimate card opens a three-step pop-up with animated, adjustable build drawings. Project choices survive an accidental close for the current browser session; contact details are not stored in the draft. |
| Project scope and pricing | Four priced project types use one published rate each. Custom work is described in words and priced after assessment; unavailable online rates never display a fabricated price. |
| Interface and account access | Updated homepage, services, staged project photo panels, privacy navigation and responsive layouts; clearer registration and sign-in validation; optional seven-day trusted-device MFA. |
| Search discovery | Added a [sitemap](./src/web/public/sitemap.xml) for public routes and [robots.txt](./src/web/public/robots.txt) with crawling rules for account, portal and API paths. |
| Verification pipeline | Frontend and backend build checks run in parallel. API, security and browser suites use separate API processes to isolate rate-limit counters, with logs retained as test evidence. |

## Architecture and security

```mermaid
flowchart LR
    subgraph Public["Public access boundary"]
        Browser["Visitor, client or staff browser"]
    end

    subgraph Azure["Single Azure App Service"]
        Web["React and TypeScript frontend"]
        API["ASP.NET Core API"]
        Identity["Identity, MFA and access policies"]
        Business["Quotes, projects, finance and audit"]
    end

    subgraph Data["Restricted data services"]
        SQL[("Azure SQL")]
        Files["Private Blob containers"]
        Keys["Key Vault encryption key"]
    end

    Browser -->|HTTPS| Web
    Web -->|Same-origin /api requests| API
    API --> Identity
    Identity --> Business
    Business -->|EF Core| SQL
    Business -->|Authorised file access| Files
    API -->|Protect shared identity keys| Keys
    API -->|Persist protected key ring| Files

    classDef rust fill:#B63D20,stroke:#8F2E17,color:#FFFFFF,stroke-width:2px;
    classDef charcoal fill:#171714,stroke:#B63D20,color:#FFFFFF,stroke-width:2px;
    classDef light fill:#F7F3F0,stroke:#B63D20,color:#171714,stroke-width:2px;

    class Browser,Web light;
    class API,Identity,Business rust;
    class SQL,Files,Keys charcoal;

    style Public fill:#FCFAF8,stroke:#B63D20,stroke-width:2px,color:#171714
    style Azure fill:#F6EAE5,stroke:#B63D20,stroke-width:2px,color:#171714
    style Data fill:#EFEFED,stroke:#171714,stroke-width:2px,color:#171714

    linkStyle default stroke:#6A625E,stroke-width:2px;
```

*Figure 1. Target hosting architecture and access boundaries.*

The deployment design uses one Azure App Service to serve React and `/api` from the same HTTPS origin. Azure SQL provides database storage; private Blob Storage holds documents and the protected identity key ring; Key Vault protects the key ring's encryption key.

The API uses feature-based controllers and services, EF Core and ASP.NET Core Identity. Local development uses SQLite and local file storage. Test fixtures are isolated from normal startup and deployment.

### Authentication and authorisation

Identity cookies establish sessions. Staff and administrator operations require the appropriate role and, in production, MFA. The API checks ownership and publication rules for projects, documents and financial records, applying access decisions to individual resources (Microsoft, 2026d).

After entering a valid authenticator code, optionally select **Remember this device for 7 days** on a trusted device. Subsequent sign-ins still require the password, but omit the authenticator challenge while device trust remains valid. Signing out preserves the original trust expiry. In **My account → Authenticator security**, select **Forget this device** to require a code on the next sign-in. Password changes and account recovery invalidate existing device trust.

The frontend obtains an antiforgery token from `/api/auth/csrf`, sends it in `X-CSRF-TOKEN` on protected writes and refreshes it after authentication changes. HTTPS does not replace antiforgery validation (Microsoft, 2026c).

### Account recovery

Generate recovery codes in **My account → Account recovery**, or save the ten codes shown when enabling MFA. Store them privately; new codes replace previous codes.

Select **Sign in → Lost access? Use a recovery code** and enter your email, a saved code and a new password. Recovery resets the authenticator, revokes existing sessions and invalidates old codes. Sign in again, re-enrol MFA and save new codes.

Recovery requires a previously saved code and cannot bypass suspension or temporary lockout.

### Data integrity and private information

Server-side validation controls quotation inputs, rates and state transitions. Version checks reject stale updates, following optimistic concurrency principles (Microsoft, 2026b). Database constraints and idempotency checks protect duplicate-sensitive operations.

Important business changes are audited. Private documents are served through authorised application operations.

The hosted configuration uses managed identity for runtime access to Azure SQL (Microsoft, 2026e). Database migration permissions are separate from runtime permissions. The runtime database identity must not update or delete existing audit records.

Identity keys are persisted in private Blob Storage and encrypted using Key Vault (Microsoft, 2026a). Keep credentials and customer data out of the repository.

### Repository structure

```text
src/
  DynamicConstruction.Api/    API, Identity, domain and EF Core migrations
  web/                       React frontend, styling and browser tests
docs/
  screenshots/               Application screenshots and workflow examples
tests/
  DynamicConstruction.Tests/ Unit tests
  FixtureLoader/             Isolated test-data loader
  integration.py             SQL-backed API regression
  security.py                Identity, MFA and access-control regression
  bootstrap.py               Administrator bootstrap regression
  load.py                    Local load check
scripts/
  local.mjs                  Setup, startup, checks and combined publishing
  smoke-hosted.py             Combined frontend/API hosting checks
.github/workflows/           Build verification and deployment
CODE_ATTRIBUTION.txt
README.md
```

## Setup and running

### Prerequisites

- Git and PowerShell 7.
- Node.js 22.13 or later in the 22.x line.
- The .NET 10 SDK selected by `global.json`.
- For full regression testing: Python 3.12, an isolated SQL Server database and Playwright Chromium.

Run commands from the repository root.

```powershell
npm run setup
npm run check
```

`setup` restores .NET tools and locked dependencies. `check` builds the application and runs xUnit and Vitest tests. API and browser regression tests run separately.

### First local administrator

Stop any running API. These settings select local development storage.

```powershell
$env:ASPNETCORE_ENVIRONMENT = 'Development'
$env:Database__Provider = 'Sqlite'
$env:Storage__Provider = 'Local'
$env:ConnectionStrings__Database = 'Data Source=App_Data/dynamic.db'
$env:Bootstrap__Email = Read-Host 'Local administrator email'
$credential = Get-Credential -UserName $env:Bootstrap__Email -Message 'Choose a 12+ character password with uppercase, lowercase, digit and symbol'
$env:Bootstrap__Password = $credential.GetNetworkCredential().Password
try {
    dotnet run --project src/DynamicConstruction.Api --no-launch-profile -- --bootstrap-admin
    if ($LASTEXITCODE -ne 0) { throw 'Administrator bootstrap failed.' }
}
finally {
    Remove-Item Env:Bootstrap__Email, Env:Bootstrap__Password -ErrorAction SilentlyContinue
    Remove-Variable credential -ErrorAction SilentlyContinue
}
```

Bootstrap is blocked when an administrator already exists. Use that account or the administration interface to manage additional accounts.

### Start the application

```powershell
npm run dev
```

Open **http://127.0.0.1:5173**. The frontend proxies API requests to port 5080. Use the same hostname consistently for cookies. Press `Ctrl+C` to stop both servers.

```powershell
Invoke-WebRequest http://127.0.0.1:5080/api/health | Select-Object StatusCode, Content
```

The expected response is HTTP 200 with `Healthy` text. This checks database connectivity.

Enrol administrator MFA through `/profile` and create staff accounts through **Clients & users**. Before customer use, publish approved business content and rates.

`App_Data` holds local data, files and development identity keys and is ignored by Git. `.env.example` is a configuration reference and is not loaded automatically.

### Publish frontend and API together

After dependency setup:

```powershell
npm run publish -- --output artifacts/release-1
```

This builds React into the API's `wwwroot`. Use a new directory inside `artifacts/` for each release. Local `App_Data` is excluded.

If you run a published package locally, create a fresh package before deployment to exclude any newly generated development data and keys.

Check the running combined application:

```powershell
python scripts/smoke-hosted.py https://app-dc-pilot-kc023-bhesg0a5g8ewhken.southafricanorth-01.azurewebsites.net
```

This checks pages, assets, routing, security and cache headers, database connectivity and anonymous API access restrictions.

### Hosted configuration

The hosted environment uses one Linux App Service, Azure SQL, private Blob Storage, a Key Vault encryption key and Application Insights. See [Hosting services](#hosting-services) for configuration screenshots.

**Region:** South Africa North · **App Service plan:** F1 (Free) · **SQL tier:** General Purpose, serverless Gen5, 2 vCores (free offer)

| App Service setting | Value or purpose |
|---|---|
| `ASPNETCORE_ENVIRONMENT` | `Production` |
| `ASPNETCORE_FORWARDEDHEADERS_ENABLED` | `true`, for the Azure hosting proxy |
| `Database__Provider` | `SqlServer` |
| `ConnectionStrings__Database` | Azure SQL connection using managed identity, encryption and certificate validation |
| `Storage__Provider` | `Azure` |
| `Storage__ContainerUri` | Private `project-files` container URI |
| `DataProtection__BlobUri` | `keys.xml` blob URI in the private `data-protection` container |
| `DataProtection__KeyIdentifier` | Versionless Key Vault URI for the `data-protection` key |
| `APPLICATIONINSIGHTS_CONNECTION_STRING` | Telemetry connection; also enable App Service instrumentation |
| `SCM_DO_BUILD_DURING_DEPLOYMENT` | `false`; deploy the prebuilt package |

Grant the API identity:

- Required runtime database permissions, without schema-owner rights.
- **Storage Blob Data Contributor** on both containers.
- **Key Vault Crypto User** on the encryption key.

Retain previous encryption-key versions. Do not create an empty `keys.xml`; the application manages the key ring (Microsoft, 2026a).

The current workflow uses repository-level Actions variables (Settings → Secrets and variables → Actions); no GitHub environment is required:

```text
DEPLOYMENT_ENABLED
AZURE_CLIENT_ID
AZURE_TENANT_ID
AZURE_SUBSCRIPTION_ID
AZURE_RESOURCE_GROUP
AZURE_SQL_SERVER
AZURE_WEBAPP_NAME
APP_URL
```

Add the repository Actions secret `SQL_MIGRATION_CONNECTION`. Configure the deployment identity's federated credential for the repository's `main` branch, using the subject printed by the workflow's federation-settings step (GitHub, 2026).

SQL migrations use a separate credential. Azure login does not give the runner the application's SQL managed identity.

When the workflow is enabled, `DEPLOYMENT_ENABLED=true` permits deployment after successful verification on `main`. The workflow is configured to apply migrations, deploy the combined package, run smoke checks and remove its temporary SQL firewall rule.

Create the initial hosted administrator through App Service SSH, using temporary `Bootstrap__Email` and `Bootstrap__Password` environment variables:

```text
cd /home/site/wwwroot
dotnet DynamicConstruction.Api.dll --bootstrap-admin
```

Clear both variables after bootstrap. Enrol staff and administrator MFA through `/profile`. Keep `FixtureLoader` restricted to disposable test databases.

## Testing and evidence

### SQL-backed API and browser regression

Use a fresh disposable database. These tests create and modify fictional records.

In **Terminal A**, at the repository root:

```powershell
$env:ASPNETCORE_ENVIRONMENT = 'Development'
$env:Database__Provider = 'SqlServer'
$env:Storage__Provider = 'Local'
$env:ConnectionStrings__Database = Read-Host 'Disposable test SQL connection string'
$env:TEST_PASSWORD = Read-Host 'Test-only password meeting the password rules'
$env:Fixture__Password = $env:TEST_PASSWORD
$env:FIXTURE_DATABASE_CONFIRMATION = 'isolated-test-database'
dotnet build -c Release
dotnet ef database update --project src/DynamicConstruction.Api --configuration Release --no-build
dotnet ef database update --project src/DynamicConstruction.Api --configuration Release --no-build
dotnet run --project tests/FixtureLoader -c Release --no-build --no-launch-profile
dotnet run --project src/DynamicConstruction.Api -c Release --no-build --no-launch-profile --urls http://127.0.0.1:5081
```

The second migration command checks repeat application. Check each command's exit code before continuing.

In **Terminal B**, at the repository root:

```powershell
$env:TEST_BASE_URL = 'http://127.0.0.1:5081'
$env:TEST_PASSWORD = Read-Host 'The same test-only password as Terminal A'
python tests/integration.py
python tests/bootstrap.py
Start-Sleep -Seconds 61
python tests/security.py
Start-Sleep -Seconds 61
$env:API_TARGET = $env:TEST_BASE_URL
cd src/web
npx playwright install chromium
npm run test:e2e
cd ../..
Start-Sleep -Seconds 61
python tests/load.py
```

Run integration tests before browser tests because publication tests change rates. Stop other Vite instances so Playwright uses the intended API. Pauses allow shared rate-limit windows to reset. Browser tests cover desktop and mobile Chromium.

Regression coverage includes the three-step quote flow, custom requests, responsive navigation, registration validation, trusted-device MFA and recovery. These suites are defined in the repository; a successful run and hosted acceptance evidence must be checked for the final release.

CI reports use `artifacts/`. Playwright reports use `src/web/playwright-report/` and `src/web/test-results/`. Exclude credentials and customer records from evidence.


## Version control and deployment

Feature branches merge into `develop` through reviewed pull requests. The integrated application then merges into `main`.

```mermaid
flowchart LR
    Feature["Feature branches"] --> Review["Pull request review"]
    Review --> Develop["develop"]
    Develop --> Main["main"]
    Main --> Verify["Build, unit, SQL, security and browser checks"]
    Verify --> Package["Versioned release artifact"]
    Package --> Production["Migrate and deploy to the live App Service"]
    Production --> Acceptance["Hosted smoke checks and acceptance"]

    classDef rust fill:#B63D20,stroke:#8F2E17,color:#FFFFFF,stroke-width:2px;
    classDef charcoal fill:#171714,stroke:#B63D20,color:#FFFFFF,stroke-width:2px;
    classDef light fill:#F7F3F0,stroke:#B63D20,color:#171714,stroke-width:2px;

    class Feature,Review light;
    class Develop,Main charcoal;
    class Verify,Package rust;
    class Acceptance light;
    class Production charcoal;

    linkStyle default stroke:#B63D20,stroke-width:2px;
```

*Figure 2. Intended verification and release process.*

The [CI workflow](./.github/workflows/ci.yml) defines verification for pushes to `main`, pull requests into `main` or `develop`, and manual runs. Feature and `develop` changes are verified through pull requests rather than duplicate push runs. Deployment is configured for verified pushes to `main` when enabled. Hosted acceptance includes separate functional checks.

Frontend and backend builds run in parallel, followed by SQL migration and API, identity/security and browser regression checks. Each regression suite starts its own API process against the disposable SQL database, isolating in-memory rate limits. The same verified frontend/API package is used for combined-hosting smoke checks and deployment.

Release artifacts are configured for **3-day retention**, and test evidence for **1-day retention**. Rollback requires a previous successful artifact compatible with the current database schema; deploying older code does not reverse migrations. Load testing runs separately from CI.

## Contributors

**Group: ETC ETC**

| Contributor | Role | Contribution |
|---|---|---|
| Khayden Chetty | Designer | Original public website and quote journey, pricing, published content, shared visual design and Azure hosting setup |
| Rivaan Kawulesar | Developer | Database and migrations, client portal, finance and workflows, CI/CD pipeline, authenticator improvements, trusted-device MFA and account validation |
| Stephane Nsengiyumva | Tester | Quotation queue, project workspace, lifecycle rules, private files, change requests and regression test foundation |
| Zenwyn Naicker | Project Manager | Identity and security, account administration, notifications and audit, quote builder redesign and build animations, homepage project panels, portal UX, performance, startup and final documentation |


## Acknowledgements

Frameworks, libraries and adopted implementation patterns are acknowledged in [CODE_ATTRIBUTION.txt](./CODE_ATTRIBUTION.txt). The references below support the technical explanations in this README.

## References

GitHub, 2026. *Configuring OpenID Connect in Azure*. [online] Available at: <https://docs.github.com/en/actions/how-tos/secure-your-work/security-harden-deployments/oidc-in-azure> [Accessed 24 September 2026].

Microsoft, 2026a. *Configure ASP.NET Core Data Protection*. [online] Available at: <https://learn.microsoft.com/en-us/aspnet/core/security/data-protection/configuration/overview?view=aspnetcore-10.0> [Accessed 24 September 2026].

Microsoft, 2026b. *Handling concurrency conflicts*. [online] Available at: <https://learn.microsoft.com/en-us/ef/core/saving/concurrency> [Accessed 24 September 2026].

Microsoft, 2026c. *Prevent Cross-Site Request Forgery (XSRF/CSRF) attacks in ASP.NET Core*. [online] Available at: <https://learn.microsoft.com/en-us/aspnet/core/security/anti-request-forgery?view=aspnetcore-10.0> [Accessed 24 September 2026].

Microsoft, 2026d. *Resource-based authorization in ASP.NET Core MVC*. [online] Available at: <https://learn.microsoft.com/en-us/aspnet/core/mvc/security/authorization/resource-based?view=aspnetcore-10.0> [Accessed 24 September 2026].

Microsoft, 2026e. *Securely connect .NET apps to Azure SQL Database using managed identity*. [online] Available at: <https://learn.microsoft.com/en-us/azure/app-service/tutorial-connect-msi-sql-database> [Accessed 24 September 2026].
