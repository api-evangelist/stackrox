# StackRox

StackRox is the open source upstream project for Red Hat Advanced Cluster Security for Kubernetes. It provides risk analysis, visibility, runtime alerts, and recommendations to proactively improve security by hardening containerized environments across build, deploy, and runtime stages. The platform performs compliance checking against standards like CIS, NIST, and PCI-DSS, and manages security policies across Kubernetes clusters.

**Website:** [https://www.stackrox.io/](https://www.stackrox.io/)
**Documentation:** [https://www.stackrox.io/docs/](https://www.stackrox.io/docs/)
**GitHub:** [https://github.com/stackrox/stackrox](https://github.com/stackrox/stackrox)
**Red Hat Product:** [Advanced Cluster Security](https://www.redhat.com/en/technologies/cloud-computing/openshift/advanced-cluster-security-kubernetes)

## Tags

- Compliance, Container Security, Kubernetes, Open Source, Runtime Protection, Security

## APIs

### StackRox API
REST API for the StackRox Kubernetes Security Platform. 128 endpoints covering alerts, policies, deployments, images, compliance, clusters, roles, and vulnerability management.

- **Base URL:** `https://{central-host}`
- **Authentication:** API Token via `Authorization: Bearer {token}` header
- **Token generation:** `POST /v1/apitokens/generate`

## OpenAPI Specifications

| Spec | Path |
|---|---|
| StackRox API | [openapi/stackrox-openapi.yml](openapi/stackrox-openapi.yml) |

## Spectral Rules

| Ruleset | Path |
|---|---|
| StackRox API Rules | [rules/stackrox-rules.yml](rules/stackrox-rules.yml) |

## Naftiko Capabilities

### Shared Definitions

| API | Path |
|---|---|
| StackRox API | [capabilities/shared/stackrox-api.yaml](capabilities/shared/stackrox-api.yaml) |

### Workflow Capabilities

| Workflow | Description | Path |
|---|---|---|
| Kubernetes Security | Alert triage, policy management, image scanning, compliance, cluster monitoring | [capabilities/kubernetes-security.yaml](capabilities/kubernetes-security.yaml) |

## JSON Schema

| Schema | Path |
|---|---|
| Alert | [json-schema/stackrox-alert-schema.json](json-schema/stackrox-alert-schema.json) |
| Security Policy | [json-schema/stackrox-policy-schema.json](json-schema/stackrox-policy-schema.json) |

## JSON Structure

| Structure | Path |
|---|---|
| Alert | [json-structure/stackrox-alert-structure.json](json-structure/stackrox-alert-structure.json) |

## JSON-LD

| Context | Path |
|---|---|
| StackRox Context | [json-ld/stackrox-context.jsonld](json-ld/stackrox-context.jsonld) |

## Examples

| Example | Path |
|---|---|
| List Alerts | [examples/stackrox-list-alerts-example.json](examples/stackrox-list-alerts-example.json) |

## Vocabulary

| Vocabulary | Path |
|---|---|
| StackRox Vocabulary | [vocabulary/stackrox-vocabulary.yml](vocabulary/stackrox-vocabulary.yml) |

## Timestamps

- **Created:** 2026-03-26
- **Modified:** 2026-05-02
