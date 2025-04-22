# Open Source and Commercial Data Governance Tool Capability Tracker

## Tool Evaluation Matrix

| Tool Name | Version | License Type | Deployment Options (Self-Hosted/Cloud) | Primary Focus | Maturity Level | Federal Agency Usage |
|-----------|---------|--------------|----------------------------------------|--------------|----------------|---------------------|
| [Apache Atlas](https://atlas.apache.org/#/) | [2.4.0 (Jan 2025)](https://github.com/apache/atlas/releases/tag/release-2.4.0) | Apache License 2.0 | Self-Hosted | Data Governance & Metadata Management (primarily for Hadoop) | High ([Graduated from Apache Incubator in 2017](https://incubator.apache.org/projects/atlas.html#:~:text=The%20Atlas%20project%20graduated%20on%202017%2D06%2D21)) | [Dept. of Veterans Affairs](https://www.oit.va.gov/Services/TRM/ToolPage.aspx?tid=15357#:~:text=Users%20must%20ensure%20sensitive%20data%20is%20properly,(ISO)%2C%20Facility%20Chief%20Information%20Officer%20(CIO)%2C%20or) |
| AWS (Lake Formation & Glue Data Catalog) | [Varies by service](https://aws.amazon.com/lake-formation/) | [AWS Service Terms](https://aws.amazon.com/service-terms/) (commercial) | Cloud | Centralized Data Lake Governance & Metadata Management | High (Continuously updated) | [Several US federal agencies](https://aws.amazon.com/government-education/government/) |
| [CKAN](https://ckan.org/) | [2.11.2 (Feb 2025)](https://github.com/ckan/ckan/releases/tag/ckan-2.11.2) | GNU Affero General Public License 3.0 | Self-Hosted/Cloud | Open Data Portal & Catalog Platform | High (Recognized as a [Digital Public Good](https://ckan.org/blog/CKAN-2023-a-year-of-milestones)) | [data.gov](https://resources.data.gov/categories/data-tools/), [Federal Aviation Administration](https://catalog.data.faa.gov/about), and several other governments worldwide |
| [Collibra Data Intelligence Platform](https://www.collibra.com/products/collibra-platform) | [2025.04 (April 2025)](https://productresources.collibra.com/docs/collibra/latest/Content/ReleaseNotes/ref_release-calendar.htm) | [Master Collibra Agreement](https://www.collibra.com/legal/documents/master-collibra-agreement) (commercial) | Self-Hosted/Cloud | Unified Data Intelligence & Governance | High (Leader in [2025 Gartner Magic Quadrant](https://www.collibra.com/company/newsroom/press-releases/collibra-named-a-leader-in-the-first-ever-gartner-magic-quadrant-for-data-and-analytics)) | [Health Resources and Services Administration](https://orangeslices.ai/contract-award-hrsa-oit-collibra-data-software-catalog/), [Office of the Secretary of Defense](https://www.collibra.com/customer-stories/office-of-the-secretary-of-defense), [Dept. of Veterans Affairs](https://orangeslices.ai/contract-award-va-collibra-enterprise-platform/), [Others](https://www.globenewswire.com/news-release/2020/03/05/1995793/0/en/Collibra-Announces-Customer-Momentum-with-Leading-Federal-Agencies.html) |
| [Databricks Unity Catalog](https://www.databricks.com/product/unity-catalog) | [Continuously updated](https://www.databricks.com/product/unity-catalog) | [Databricks Terms](https://www.databricks.com/legal/terms-of-use) (commercial with open source components) | Cloud/Self-Hosted | Unified Data & AI Asset Governance | High (Integrated with Databricks Lakehouse Platform) | [US Postal Service, Dept. of the Air Force, Office of the Inspector General, Others](https://www.databricks.com/solutions/industries/public-sector) |
| [DataHub](https://datahubproject.io/) | [1.0.0 (March 2025)](https://datahubproject.io/docs/releases/) | Apache License 2.0 | Self-Hosted/Cloud | Data & AI Metadata Platform for Discovery, Observability & Governance | High (Actively maintained by [LinkedIn, Acryl Data](https://www.acryldata.io/press/founded-by-airbnb-and-linkedin-data-veterans-acryl-data-re-imagines-metadata-management-with-dollar9-million-in-seed-funding)) | Limited information available |
| [dbt](https://www.getdbt.com/) | [Core 1.10.0b2 (Apr 2025)](https://github.com/dbt-labs/dbt-core/releases), [Cloud (Apr 2025)](https://docs.getdbt.com/docs/dbt-versions/dbt-cloud-release-notes) | Apache License 2.0 | Self-Hosted/Cloud | Data Transformation, Testing, Documentation & Metrics Management | High (Widely adopted, active development) | Limited information available |
| [Great Expectations](https://greatexpectations.io/) | [1.4.0 (Apr 2025)](https://github.com/great-expectations/great_expectations/releases/tag/1.4.0) | Apache License 2.0 | Self-Hosted/Cloud | Data Quality Testing, Validation & Observability | High (Widely adopted, active development) | Limited information available |
| Oracle - Native | | | | | | |
| [OpenMetadata](https://open-metadata.org/) | [1.7.0 (Apr 2025)](https://github.com/open-metadata/OpenMetadata/releases/tag/1.7.0-release) | Apache License 2.0 | Self-Hosted/Cloud (Collate SaaS) | Unified Metadata Platform for Discovery, Governance & Observability | High (Active development since 2021) | Limited information available |

## Core Capabilities

| Tool Name | Data Catalog | Metadata Management | Data Lineage | Audit Trail Logs | Data Quality Testing | Role-Based Access Control | Data Classification |
|-----------|--------------|---------------------|--------------|------------------|---------------------|---------------------------|---------------------|
| Apache Atlas | FS | FS | FS | [FS](https://www.clearpeaks.com/data-governance-with-apache-atlas-introduction-to-atlas/) | LS | FS | [FS](https://atlas.apache.org/1.2.0/ClassificationPropagation.html) |
| AWS Lake Formation/Glue | FS | FS | [FS](https://aws.amazon.com/blogs/aws/introducing-end-to-end-data-lineage-preview-visualization-in-amazon-datazone/) | [FS](https://docs.aws.amazon.com/lake-formation/latest/dg/security-event-logging.html) | [FS](https://aws.amazon.com/glue/features/data-quality/) | [FS](https://docs.aws.amazon.com/lake-formation/latest/dg/lf-permissions-overview.html) | FS ([classifiers](https://docs.aws.amazon.com/glue/latest/dg/add-classifier.html) + separate [PII detection](https://docs.aws.amazon.com/glue/latest/dg/detect-PII.html)) |
| CKAN | FS | [PS](https://github.com/ckan/ckanext-scheming) | [LS](https://github.com/ahussein/ckanext-datalineage) | [LS](https://github.com/ckan/ckan/issues/3998) | [PS](https://ckan.org/blog/introducing-ckanext-validation-data-validation-and-reporting-integrated-in-ckan) | FS | LS |
| Collibra Data Intelligence Platform | FS | FS | [FS](https://www.collibra.com/products/data-lineage#sub-menu-features) | [FS](https://productresources.collibra.com/docs/collibra/latest/Content/Architecture/co_audit-logging.htm) | [FS](https://www.collibra.com/products/data-quality-and-observability) | [FS](https://www.collibra.com/products/data-quality-and-observability) | [FS](https://productresources.collibra.com/docs/collibra/latest//Content/Catalog/DataClassification/co_about-data-classification.htm) |
| Databricks Unity Catalog | [FS](https://docs.databricks.com/aws/en/data-governance/unity-catalog/) | FS | [FS](https://docs.databricks.com/aws/en/data-governance/unity-catalog/data-lineage) | [FS](https://docs.databricks.com/aws/en/data-governance/unity-catalog/audit) | [FS](https://www.databricks.com/discover/pages/data-quality-management) | [FS](https://docs.databricks.com/aws/en/data-governance/unity-catalog/manage-privileges) | [PS](https://docs.databricks.com/aws/en/lakehouse-monitoring/data-classification) |
| DataHub | [FS](https://datahubproject.io/docs/features/) | [FS](https://datahubproject.io/docs/features/) | [FS](https://datahubproject.io/docs/api/tutorials/lineage/) | [FS](https://datahubproject.io/docs/what/mxe/) | [FS](https://datahubproject.io/docs/assertions/open-assertions-spec/) | [PS](https://datahubproject.io/docs/authorization/roles) (custom roles planned) | [FS](https://medium.com/datahub-project/pii-classification-just-got-easier-with-datahub-6bab2b63abcb) |
| dbt | [PS](https://www.getdbt.com/product/integrations) | [PS](https://atlan.com/dbt-metadata-management/) | [FS](https://docs.getdbt.com/docs/collaborate/explore-projects#example-of-full-lineage-graph) | [FS](https://docs.getdbt.com/docs/cloud/manage-access/audit-log) (Enterprise) | [FS](https://www.getdbt.com/blog/building-a-data-quality-framework-with-dbt-and-dbt-cloud) | [FS](https://docs.getdbt.com/docs/cloud/manage-access/about-user-access) | [PS](https://www.getdbt.com/blog/critical-tools-data-governance) |
| Great Expectations | NS | PS | NS | FS | FS | FS | LS |
| Oracle - Native | | | | | | | |
| OpenMetadata | FS | FS | FS | FS | FS | FS | FS |

## Query & Analytics Capabilities

| Tool Name | Query Engine | Federated Query | Anomaly Detection | Handles Structured Data | Handles Unstructured Data | Search Capabilities |
|-----------|--------------|-----------------|-------------------|-------------------------|---------------------------|---------------------|
| Apache Atlas | PS | PS | LS | FS | LS | FS |
| AWS Lake Formation/Glue | FS | FS | PS | FS | PS | FS |
| CKAN | LS | LS | NS | FS | PS | FS |
| Collibra Data Intelligence Platform | FS | FS | FS | FS | PS | FS |
| Databricks Unity Catalog | FS | FS | FS | FS | FS | FS |
| DataHub | PS | PS | FS | FS | PS | FS |
| dbt | FS | PS | PS | FS | PS | FS |
| Great Expectations | PS | NS | FS | FS | LS | LS |
| Oracle - Native | | | | | | |
| OpenMetadata | | | | | | |

## Integration & Development

| Tool Name | Pre-Built Connectors | Automation Capabilities | CI/CD Integration | SDK Availability | API Documentation | Extensibility |
|-----------|----------------------|-------------------------|-------------------|------------------|-------------------|---------------|
| Apache Atlas | PS | PS | PS | FS | FS | FS |
| AWS Lake Formation/Glue | FS (50+) | FS | FS | FS | FS | FS |
| CKAN | PS | PS | PS | FS | FS | FS |
| Collibra Data Intelligence Platform | FS (150+) | FS | FS | FS | FS | FS |
| Databricks Unity Catalog | FS (90+) | FS | FS | FS | FS | FS |
| DataHub | FS (50+) | FS | PS | FS | FS (GraphQL & REST) | FS |
| dbt | FS | FS | FS | FS | FS | FS |
| Great Expectations | FS | FS | FS | FS | FS | FS |
| Oracle - Native | | | | | | |
| OpenMetadata | FS (90+) | FS | PS | FS | FS | FS |

## Infrastructure & Resources

| Tool Name | Data Storage Options | Computational Resources | Scalability | Performance | On-Prem Support | Cloud Support |
|-----------|----------------------|-------------------------|-------------|------------|-----------------|---------------|
| Apache Atlas | HBase (JanusGraph 1.0.0) | Medium-High | FS | PS | FS | PS |
| AWS Lake Formation/Glue | S3/Various AWS Services | Medium-High | FS | FS | NS | FS |
| CKAN | PostgreSQL/Solr | Low-Medium | PS | PS | FS | PS |
| Collibra Data Intelligence Platform | Multiple options | Medium | FS | FS | FS | FS |
| Databricks Unity Catalog | Delta Lake/Various Cloud Storage | Medium-High | FS | FS | PS | FS |
| DataHub | MySQL/Elasticsearch/Neo4j | Medium-High | FS | FS | FS | FS |
| dbt | Works with existing data warehouse | Low | FS | FS | FS | FS |
| Great Expectations | No storage (validates in-place) | Low | FS | PS | FS | FS |
| Oracle - Native | | | | | | |
| OpenMetadata | MySQL/PostgreSQL, Elasticsearch/OpenSearch | Low-Medium | FS | FS | FS | FS |

## Compliance & Security

| Tool Name | GDPR Compliance | HIPAA Compliance | Security Compliance | FedRAMP Status | Data Encryption | Authentication Methods | Notes |
|-----------|-----------------|------------------|------------------|----------------|-----------------|------------------------|-----------------|
| Apache Atlas | LS | LS | U | Only applicable to cloud services | FS | [File, Kerberos, LDAP](https://atlas.apache.org/1.1.0/Atlas-Authentication.html), [SSL, Service Authentication, SPNEGO-based HTTP Authentication](https://atlas.apache.org/1.1.0/Security.html) | Not explicitly compliant but can be used to achieve compliance with GDPR, HIPAA, ISO 27001 |
| AWS Lake Formation/Glue | FS | FS | [Security compliances listed](https://aws.amazon.com/compliance/iso-certified/) | [Authorized (High)](https://aws.amazon.com/compliance/fedramp/) | FS | [IAM](https://docs.aws.amazon.com/iam/)| |
| CKAN | [LS](https://github.com/ckan/ckan/issues/4361)/[PS](https://www.datopian.com/showcase/case-studies/ubdc-data-portal-revamp-ckan-powered-secure-gdpr-compliant) | [PS](https://www.keitaro.com/insights/2023/08/07/streamlining-data-management-with-ckan-and-keycloak-integration/) | [NS](https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/998119544445508) | U | NS | [SSO](https://extensions.ckan.org/extension/saml2auth/), [Basic Auth (MFA via Keycloak)](https://www.keitaro.com/insights/2023/08/07/streamlining-data-management-with-ckan-and-keycloak-integration/), [Public key authentication](https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/998119544445508) | [CKANEXT-SECURITY](https://github.com/data-govt-nz/ckanext-security) |
| Collibra Data Intelligence Platform | FS | FS | [Security compliances listed](https://www.collibra.com/company/trust-center#sub-menu-compliance) | [Authorized (Moderate)](https://www.collibra.com/resources/collibra-and-fedramp) | FS | [SSO](https://productresources.collibra.com/docs/collibra/latest/Content/Console/Infrastructure/DGCService/SecurityConfiguration/co_single-sign-on.htm), [LDAP](https://productresources.collibra.com/docs/collibra/latest/Content/Console/Infrastructure/DGCService/SecurityConfiguration/co_LDAP-configuration.htm), [SAML](https://productresources.collibra.com/docs/collibra/latest/Content/Console/Infrastructure/DGCService/SecurityConfiguration/SAML/co_about-saml.htm), [JSON Web Token](https://productresources.collibra.com/docs/collibra/latest/Content/Console/Infrastructure/DGCService/SecurityConfiguration/JWT/to_JWT-authentication.htm) | |
| Databricks Unity Catalog | [FS](https://www.databricks.com/trust/compliance/gdpr) | [FS](https://docs.databricks.com/aws/en/security/privacy/hipaa) | [Security compliances listed](https://www.databricks.com/trust/compliance/iso-27001) | [Integrates with High and Moderate supported clouds (AWS and Azure)](https://www.databricks.com/trust/compliance/fedramp) | FS | [SSO, OAuth](https://docs.databricks.com/aws/en/security/auth) | |
| DataHub | LS | LS | U  | U | U | [SSO, JaaS, Basic Auth, Access Tokens](https://datahubproject.io/docs/authentication) | Not explicitly compliant but can be used to achieve compliance with GDPR, HIPAA, ISO 27001 |
| dbt | FS | FS | [Security compliances listed](https://www.getdbt.com/security) | U | FS | [SSO and OAuth](https://docs.getdbt.com/docs/cloud/manage-access/sso-overview), [Authentication Tokens](https://docs.getdbt.com/docs/dbt-cloud-apis/authentication) | |
| Great Expectations | U | U | [SOC 2 Type II](https://trust.greatexpectations.io/) | U | FS | [SSH, Basic Auth](https://trust.greatexpectations.io/controls#infrastructure-security), [SSO (Enterprise), Access Tokens](https://docs.greatexpectations.io/docs/cloud/users/manage_users)| |
| Oracle - Native | | | | | | | |
| OpenMetadata | PS | PS | U | U | PS | [SSO](https://docs.open-metadata.org/latest/deployment/security), [Basic Auth](https://docs.open-metadata.org/latest/deployment/security/basic-auth), [LDAP](https://docs.open-metadata.org/latest/deployment/security/ldap), [SSL](https://docs.open-metadata.org/latest/deployment/security/enable-ssl), [JWT Tokens](https://docs.open-metadata.org/latest/deployment/security/enable-jwt-tokens) | |

## Notes & References

| Tool Name | Key Strengths | Key Limitations | Notable Use Cases | Documentation Link | Community/Forum Link | Last Evaluated |
|-----------|---------------|-----------------|-------------------|-------------------|---------------------|----------------|
| Apache Atlas | Strong Hadoop integration, Mature data classification, Good for compliance, Modernized tech stack with JanusGraph 1.0.0 support, Enhanced notification handling via REST APIs | Complex setup, Hadoop-centric, Requires significant Java expertise | Financial services compliance, Healthcare data governance | [Documentation](https://atlas.apache.org/) | [GitHub](https://github.com/apache/atlas) | April 2025 |
| AWS Lake Formation/Glue | Seamless integration with AWS ecosystem, Comprehensive access controls, Centralized governance, No-ETL data sharing, Built-in auditing capabilities | Limited to AWS ecosystem, Requires AWS expertise, Cost scales with usage | Cross-account data lake governance, Fine-grained access control, Regulatory compliance, Centralized data catalogs | [Documentation](https://docs.aws.amazon.com/lake-formation/) | [AWS Forums](https://forums.aws.amazon.com/) | April 2025 |
| CKAN | Widespread adoption, Strong open data portal capabilities, Proven at scale, Rich extension ecosystem, Deep government sector experience | Limited data governance capabilities, Basic metadata management, Requires significant customization for enterprise needs | Open data portals, Government transparency initiatives, Public data sharing | [Documentation](https://docs.ckan.org/) | [GitHub](https://github.com/ckan/ckan) | April 2025 |
| Collibra Data Intelligence Platform | Best-in-class business glossary and data governance workflows, Strong integration with enterprise systems, FedRAMP authorized for federal use, AI-enhanced automatic data classification, Unified platform approach with strong lineage capabilities, Robust workflow and collaboration features | Higher cost compared to open source alternatives, Requires dedicated personnel for maintenance, Some advanced functionality requires implementation expertise, Can be complex to fully configure | Federal agency data governance programs, Cross-agency data sharing initiatives, Privacy and compliance management, Enterprise-wide metadata management, Sensitive data discovery and classification | [Documentation](https://productresources.collibra.com/docs/collibra/latest/Content/Home.htm?utm_source=Bevy&utm_medium=community&utm_campaign=Bevy&utm_content=Documentation/) | [Community Portal](https://community.collibra.com/) | April 2025 |
| Databricks Unity Catalog | Unified governance for data and AI assets, Strong lineage tracking, Native integration with Databricks platform, Column/row-level access control, Comprehensive audit logging | Primarily designed for Databricks ecosystem, Higher cost as part of Databricks platform, Limited open source components | Unified data and AI governance, ML model tracking, Cross-cloud data governance, Data mesh implementations | [Documentation](https://www.databricks.com/product/unity-catalog) | [Databricks Community](https://community.databricks.com/) | April 2025 |
| DataHub | Unified data & AI metadata support, Enterprise scale, Advanced lineage capabilities, Intuitive platform-based navigation, End-to-end ML model tracking | Complex architecture, Requires more resources than some alternatives | Enterprise data cataloging, AI/ML asset governance, Model lineage tracking, Iceberg table management | [Documentation](https://datahubproject.io/docs/) | [GitHub](https://github.com/datahub-project/datahub) | April 2025 |
| dbt | Excellent data testing, Documentation generation, SQL/Python transformations, Semantic layer for metrics, Microbatch incremental models, Strong collaboration features | Not a complete governance solution, Requires integration with other tools | Data transformation workflows, SQL/Python transformations, Metrics standardization, Data documentation, Centralized metrics management | [Documentation](https://docs.getdbt.com/) | [GitHub](https://github.com/dbt-labs/dbt-core) | April 2025 |
| Great Expectations | Excellent data validation, Flexible expectations framework, Python-based, AI-recommended expectations, Comprehensive integration ecosystem, SaaS deployment option with GX Cloud | Not a complete metadata solution, Focus only on data quality | Data quality validation, Pipeline testing, Automated data profiling, Continuous validation monitoring | [Documentation](https://docs.greatexpectations.io/) | [GitHub](https://github.com/great-expectations/great_expectations) | April 2025 |
| Oracle - Native | | | | | | |
| OpenMetadata | Modern architecture, 90+ connectors, Streamlined 4-component structure, Robust data quality capabilities, Auto-classification workflows, ER diagrams for visualizing table connections | Newer platform compared to some alternatives | Cross-system metadata management, Data discovery, Data observability, Data governance, Data quality management | [Documentation](https://docs.open-metadata.org/) | [GitHub](https://github.com/open-metadata/OpenMetadata) | April 2025 |

## Evaluation Ratings Legend

For each capability, consider using a standardized rating system:
- **Full Support (FS)**: Feature is fully implemented and robust
- **Partial Support (PS)**: Feature exists but may have limitations
- **Limited Support (LS)**: Basic implementation with significant limitations
- **Planned (P)**: On the roadmap but not yet implemented
- **Not Supported (NS)**: Not currently available or supported
- **Unknown (U)**: Information not available

## Tool Evaluation Summary

| Tool Name | Overall Score (1-10) | Best For | Not Recommended For | Final Recommendation |
|-----------|----------------------|----------|---------------------|----------------------|
| Apache Atlas | 7 | Hadoop-centric environments, Compliance-focused needs | Cloud-native deployments, Small teams with limited resources | Consider for agencies with existing Hadoop infrastructure and strong security/compliance requirements |
| AWS Lake Formation/Glue | 8.5 | AWS-centric organizations, Data lake governance, Cross-account data sharing | Organizations not using AWS, Budget-sensitive deployments, Complete vendor independence | Strong **commercial** option for agencies already invested in AWS ecosystem seeking centralized governance with federal compliance capabilities |
| CKAN | 6 | Public data sharing, Open data portals, Government transparency initiatives | Enterprise data governance, Sensitive data handling, Complex compliance requirements | Best suited for public-facing data portals rather than internal governance of sensitive information |
| Collibra Data Intelligence Platform | 9 | Agencies requiring FedRAMP compliance, Organizations with complex governance requirements, Environments with sensitive data requiring strong controls, Cross-agency data sharing and collaboration | Small teams with limited budgets, Projects requiring minimal governance, Organizations without dedicated data governance personnel | Highly recommended **commercial solution** for ACF given the need to handle sensitive information across programs while ensuring regulatory compliance. The FedRAMP authorization and established federal agency usage make it a lower-risk choice for implementation. |
| Databricks Unity Catalog | 8 | Organizations using Databricks, Unified governance of data and AI assets, Multi-cloud deployments | Organizations not using Databricks, Budget-constrained deployments | Best for agencies already using or planning to use Databricks as their analytics platform |
| DataHub | 8.5 | Organizations with complex data ecosystems that include both traditional data assets and AI/ML workloads | Small teams with limited resources or technical expertise | Strong candidate for larger agencies with complex data ecosystems, especially those involved in AI/ML initiatives |
| dbt | 7.5 | Data transformation workflows, Data testing, Pipeline documentation, Centralized metrics management | Complete data governance solution, Data discovery without additional tools | Good complementary tool to pair with a dedicated data catalog/governance platform, excellent for standardizing metrics definitions across tools |
| Great Expectations | 7.5 | Data quality validation, Automated data testing, Schema enforcement, Continuous data monitoring | Full data governance, Metadata management | Excellent complementary tool focused on data quality that integrates well with broader data platforms; superior choice for automated testing with AI assistance |
| Oracle - Native | | | | |
| OpenMetadata | 8.5 | Organizations seeking a unified metadata platform with strong governance capabilities and extensive connector support | Organizations with limited technical resources requiring minimal setup | Strong candidate for agencies seeking a modern, well-supported solution with broad connector support and comprehensive governance features |