# Honeycomb Security | AppSec Testing Lab

## Overview

Dedicated Application Security and DevSecOps laboratory
for validating security tools, automated security controls,
and software supply chain practices.

This repository is maintained by Honeycomb-Security.

## Objectives

- Validate application security tools and detection capabilities.
- Implement automated security testing in CI/CD pipelines.
- Evaluate security controls throughout the SSDLC.
- Analyze vulnerabilities and false positives.
- Generate reproducible security testing evidence.
- Evaluate software supply chain security controls.

## Scope

| Domain | Planned tools |
| --- | --- |
| SAST | CodeQL, Semgrep, SonarQube |
| SCA | OSV Scanner, Trivy, Dependabot |
| DAST | OWASP ZAP |
| Secret Scanning | GitHub Secret Scanning, Gitleaks |
| IaC Security | Trivy |
| Container Security | Trivy |
| Vulnerability Management | DefectDojo |
| SBOM | Trivy, Dependency-Track |
| CI/CD | GitHub Actions |

## Repository Structure

    appsec-testing-lab/
    ├── .github/workflows/
    ├── sast/
    ├── sca/
    ├── dast/
    ├── secrets/
    ├── iac/
    ├── containers/
    ├── docs/
    ├── .gitignore
    ├── README.md
    └── LICENSE

## Security Governance

The repository follows the Honeycomb Security baseline,
aligned with the principles of:

- NIST Secure Software Development Framework (SSDF).
- OWASP Software Assurance Maturity Model (SAMM).
- Supply-chain Levels for Software Artifacts (SLSA).

Configured repository controls include:

- Protected default branch.
- Mandatory pull request workflow.
- Linear commit history.
- Restricted GitHub Actions.
- Full-length SHA pinning for actions.
- Read-only default workflow permissions.
- Secret Scanning and Push Protection.
- CodeQL Default Setup.
- Dependabot Security Updates.

## Testing Methodology

1. Define a controlled security test case.
2. Introduce an intentionally vulnerable sample.
3. Execute the selected security scanner.
4. Validate expected and actual findings.
5. Analyze false positives and false negatives.
6. Document results and remediation guidance.

## Security Disclaimer

This repository is intended exclusively for educational,
research, and authorized security testing purposes.

It may contain intentionally vulnerable code, insecure
configurations, and synthetic credential samples.

- Never use real credentials or customer information.
- Never deploy vulnerable samples to production.
- Execute vulnerable applications in isolated environments.
- Do not expose vulnerable services to the public Internet.
- Review all changes before publishing them.

## Implementation Status

Initial repository hardening is configured.

Security tools, test cases, and automated pipelines
will be incorporated progressively. Functional validation
and security control verification remain in progress.

## Maintainer

Honeycomb-Security

## License

MIT License. See LICENSE for details.
