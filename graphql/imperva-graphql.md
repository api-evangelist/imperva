# Imperva GraphQL

## Title
Imperva Cloud Application Security GraphQL Schema

## Description
Imperva (a Thales company) is a leading cybersecurity provider offering cloud WAF, DDoS protection, bot management, API security, CDN, and data security fabric solutions. Imperva's primary developer interface is REST-based, documented at the Thales/Imperva developer portal. The platform does not currently publish a native GraphQL endpoint; this schema is a conceptual GraphQL representation of Imperva's data model derived from their REST API surface, OpenAPI specification, and product documentation.

The types cover the Cloud Application Security API (cloud WAF, DDoS, CDN, bot management), the SecureSphere on-premises API (MX appliance management, server groups, web services, security policies), the API Security product (API discovery, threat detection, policy enforcement), and the Data Security Fabric (DSF) API (database auditing, compliance, data monitoring).

## Endpoint
- Native GraphQL endpoint: Not publicly available
- REST API base URL: https://api.imperva.com
- API documentation: https://docs-cybersec.thalesgroup.com/bundle/cloud-application-security/page/apiv2/cloud-api.htm
- Legacy docs: https://docs.imperva.com/bundle/cloud-application-security/page/api-reference.htm

## GraphQL Support Notes
Imperva does not expose a public GraphQL endpoint as of mid-2026. Their developer APIs are REST/JSON with API key authentication (API ID + API key from the Imperva management console). The SecureSphere on-premises platform uses username/password authenticated REST. An imperva-sdk Python library wraps the SecureSphere API.

This schema models Imperva's domain entities as GraphQL types to enable tooling integration, schema federation, and API catalog enrichment. It is a conceptual SDL derived from:
- Imperva Cloud WAF REST API (OpenAPI: cwaf-v1-swagger-3.json)
- SecureSphere Open API (github.com/imperva-dev/securesphere-swagger)
- Imperva product documentation and feature sets
- Public GitHub repositories under github.com/imperva

## References
- https://docs-cybersec.thalesgroup.com/bundle/cloud-application-security/page/apiv2/cloud-api.htm
- https://docs-cybersec.thalesgroup.com/bundle/api-docs/page/api/api-overview.htm
- https://github.com/imperva/imperva-web-api-composer
- https://github.com/imperva-dev/securesphere-swagger
- https://www.imperva.com/products/
