# Open Source and Commercial Data Governance Tool Capability Tracker

## Tool Evaluation Matrix

| Tool Name | Version | License Type | Deployment Options (Self-Hosted/Cloud) | Maturity Level | Federal Agency Usage |
|-----------|---------|--------------|----------------------------------------|--------------|----------------
| [Apache Atlas](https://atlas.apache.org/#/) | [2.4.0 (Jan 2025)](https://github.com/apache/atlas/releases/tag/release-2.4.0) | Apache License 2.0 | Self-Hosted | High ([Graduated from Apache Incubator in 2017](https://incubator.apache.org/projects/atlas.html#:~:text=The%20Atlas%20project%20graduated%20on%202017%2D06%2D21)) | [Dept. of Veterans Affairs](https://www.oit.va.gov/Services/TRM/ToolPage.aspx?tid=15357#:~:text=Users%20must%20ensure%20sensitive%20data%20is%20properly,(ISO)%2C%20Facility%20Chief%20Information%20Officer%20(CIO)%2C%20or) |
| AWS (Lake Formation & Glue Data Catalog) | [Varies by service](https://aws.amazon.com/lake-formation/) | [AWS Service Terms](https://aws.amazon.com/service-terms/) (commercial) | Cloud | High (Continuously updated) | [Several US federal agencies](https://aws.amazon.com/government-education/government/) |
| [CKAN](https://ckan.org/) | [2.11.2 (Feb 2025)](https://github.com/ckan/ckan/releases/tag/ckan-2.11.2) | GNU Affero General Public License 3.0 | Self-Hosted/Cloud | High (Recognized as a [Digital Public Good](https://ckan.org/blog/CKAN-2023-a-year-of-milestones)) | [data.gov](https://resources.data.gov/categories/data-tools/), [Federal Aviation Administration](https://catalog.data.faa.gov/about), and several other governments worldwide |
| [Collibra](https://www.collibra.com/products/collibra-platform) | [2025.04 (April 2025)](https://productresources.collibra.com/docs/collibra/latest/Content/ReleaseNotes/ref_release-calendar.htm) | [Master Collibra Agreement](https://www.collibra.com/legal/documents/master-collibra-agreement) (commercial) | Self-Hosted/Cloud | High (Leader in [2025 Gartner Magic Quadrant](https://www.collibra.com/company/newsroom/press-releases/collibra-named-a-leader-in-the-first-ever-gartner-magic-quadrant-for-data-and-analytics)) | [Health Resources and Services Administration](https://orangeslices.ai/contract-award-hrsa-oit-collibra-data-software-catalog/), [Office of the Secretary of Defense](https://www.collibra.com/customer-stories/office-of-the-secretary-of-defense), [Dept. of Veterans Affairs](https://orangeslices.ai/contract-award-va-collibra-enterprise-platform/), [Others](https://www.globenewswire.com/news-release/2020/03/05/1995793/0/en/Collibra-Announces-Customer-Momentum-with-Leading-Federal-Agencies.html) |
| [Databricks](https://www.databricks.com/product/unity-catalog) | [Continuously updated](https://www.databricks.com/product/unity-catalog) | [Databricks Terms](https://www.databricks.com/legal/terms-of-use) (commercial with open source components) | Cloud/Self-Hosted | High (Integrated with Databricks Lakehouse Platform) | [US Postal Service, Dept. of the Air Force, Office of the Inspector General, Others](https://www.databricks.com/solutions/industries/public-sector) |
| [DataHub](https://datahubproject.io/) | [1.0.0 (March 2025)](https://datahubproject.io/docs/releases/) | Apache License 2.0 | Self-Hosted/Cloud | High (Actively maintained by [LinkedIn, Acryl Data](https://www.acryldata.io/press/founded-by-airbnb-and-linkedin-data-veterans-acryl-data-re-imagines-metadata-management-with-dollar9-million-in-seed-funding)) | Limited information available |
| [dbt](https://www.getdbt.com/) | [Core 1.10.0b2 (Apr 2025)](https://github.com/dbt-labs/dbt-core/releases), [Cloud (Apr 2025)](https://docs.getdbt.com/docs/dbt-versions/dbt-cloud-release-notes) | Apache License 2.0 | Self-Hosted/Cloud | High (Widely adopted, active development) | Limited information available |
| [Great Expectations](https://greatexpectations.io/) | [1.4.0 (Apr 2025)](https://github.com/great-expectations/great_expectations/releases/tag/1.4.0) | Apache License 2.0 | Self-Hosted/Cloud | High (Active development since 2017) | Limited information available |
| Oracle - Native | | | | | |
| [OpenMetadata](https://open-metadata.org/) | [1.7.0 (Apr 2025)](https://github.com/open-metadata/OpenMetadata/releases/tag/1.7.0-release) | Apache License 2.0 | Self-Hosted/Cloud (Collate SaaS) | High (Active development since 2021) | Limited information available |

## Tool Evaluation Summary

| Tool Name | Overall Score (1-10) | Best For | Not Recommended For | Final Recommendation |
|-----------|----------------------|----------|---------------------|----------------------|
| Apache Atlas | | | | |
| AWS | | | | |
| CKAN | | | | |
| Collibra | | | |
| Databricks | | | | |
| DataHub | | | | |
| dbt | | | | |
| Great Expectations | | | | |
| Oracle - Native | | | | |
| OpenMetadata | | | | |

## Full Evaluation

### Evaluation Ratings Legend

For each capability, consider using a standardized rating system:
- **Full Support (FS)**: Feature is fully implemented and robust
- **Partial Support (PS)**: Feature exists but may have limitations
- **Limited Support (LS)**: Basic implementation with significant limitations
- **Planned (P)**: On the roadmap but not yet implemented
- **Not Supported (NS)**: Not currently available or supported
- **Unknown (U)**: Information not available

### Core Capabilities

| Tool Name | Data Catalog | Metadata Management | Data Lineage | Audit Trail Logs | Data Quality Testing | Role-Based Access Control | Data Classification |
|-----------|--------------|---------------------|--------------|------------------|---------------------|---------------------------|---------------------|
| Apache Atlas | FS | FS | FS | [FS](https://www.clearpeaks.com/data-governance-with-apache-atlas-introduction-to-atlas/) | LS | FS | [FS](https://atlas.apache.org/1.2.0/ClassificationPropagation.html) |
| AWS | FS | FS | [FS](https://aws.amazon.com/blogs/aws/introducing-end-to-end-data-lineage-preview-visualization-in-amazon-datazone/) | [FS](https://docs.aws.amazon.com/lake-formation/latest/dg/security-event-logging.html) | [FS](https://aws.amazon.com/glue/features/data-quality/) | [FS](https://docs.aws.amazon.com/lake-formation/latest/dg/lf-permissions-overview.html) | FS ([classifiers](https://docs.aws.amazon.com/glue/latest/dg/add-classifier.html) + separate [PII detection](https://docs.aws.amazon.com/glue/latest/dg/detect-PII.html)) |
| CKAN | FS | [PS](https://github.com/ckan/ckanext-scheming) | [LS](https://github.com/ahussein/ckanext-datalineage) | [LS](https://github.com/ckan/ckan/issues/3998) | [PS](https://ckan.org/blog/introducing-ckanext-validation-data-validation-and-reporting-integrated-in-ckan) | FS | LS |
| Collibra | FS | FS | [FS](https://www.collibra.com/products/data-lineage#sub-menu-features) | [FS](https://productresources.collibra.com/docs/collibra/latest/Content/Architecture/co_audit-logging.htm) | [FS](https://www.collibra.com/products/data-quality-and-observability) | [FS](https://www.collibra.com/products/data-quality-and-observability) | [FS](https://productresources.collibra.com/docs/collibra/latest//Content/Catalog/DataClassification/co_about-data-classification.htm) |
| Databricks | [FS](https://docs.databricks.com/aws/en/data-governance/unity-catalog/) | FS | [FS](https://docs.databricks.com/aws/en/data-governance/unity-catalog/data-lineage) | [FS](https://docs.databricks.com/aws/en/data-governance/unity-catalog/audit) | [FS](https://www.databricks.com/discover/pages/data-quality-management) | [FS](https://docs.databricks.com/aws/en/data-governance/unity-catalog/manage-privileges) | [PS](https://docs.databricks.com/aws/en/lakehouse-monitoring/data-classification) |
| DataHub | [FS](https://datahubproject.io/docs/features/) | [FS](https://datahubproject.io/docs/features/) | [FS](https://datahubproject.io/docs/api/tutorials/lineage/) | [FS](https://datahubproject.io/docs/what/mxe/) | [FS](https://datahubproject.io/docs/assertions/open-assertions-spec/) | [PS](https://datahubproject.io/docs/authorization/roles) (custom roles planned) | [FS](https://medium.com/datahub-project/pii-classification-just-got-easier-with-datahub-6bab2b63abcb) |
| dbt | [PS](https://www.getdbt.com/product/integrations) | [PS](https://atlan.com/dbt-metadata-management/) | [FS](https://docs.getdbt.com/docs/collaborate/explore-projects#example-of-full-lineage-graph) | [FS](https://docs.getdbt.com/docs/cloud/manage-access/audit-log) (Enterprise) | [FS](https://www.getdbt.com/blog/building-a-data-quality-framework-with-dbt-and-dbt-cloud) | [FS](https://docs.getdbt.com/docs/cloud/manage-access/about-user-access) | [PS](https://www.getdbt.com/blog/critical-tools-data-governance) |
| Great Expectations | [NS](https://greatexpectations.io/blog/data-catalogs-and-data-quality-using-great-expectations-with-data-catalog/) (requires integration with a data catalog) | PS | [NS](https://openlineage.io/docs/integrations/great-expectations/)(requires integration with OpenLineage) | NS (relies on integrations) | [FS](https://greatexpectations.io/expectations/) | [PS](https://docs.greatexpectations.io/docs/cloud/users/manage_users) | PS |
| Oracle - Native | | | | | | | |
| OpenMetadata | [FS](https://docs.open-metadata.org/latest/how-to-guides/data-discovery) | [FS](https://docs.open-metadata.org/latest/how-to-guides/data-discovery/details) | [FS](https://docs.open-metadata.org/latest/how-to-guides/data-lineage) | [FS](https://docs.open-metadata.org/latest/connectors/ingestion/versioning/change-feeds) | [FS](https://docs.open-metadata.org/latest/how-to-guides/data-quality-observability) | [FS](https://docs.open-metadata.org/latest/how-to-guides/admin-guide/teams-and-users) | [FS](https://docs.open-metadata.org/latest/how-to-guides/data-governance/classification) |

### Query & Analytics Capabilities

| Tool Name | Query Engine | Federated Query | Anomaly Detection | Handles Structured Data | Handles Unstructured Data |
|-----------|--------------|-----------------|-------------------|-------------------------|---------------------------|
| Apache Atlas | [FS](https://atlas.apache.org/2.0.0/Search-Advanced.html) (DSL) | [LS](https://www.mongodb.com/docs/atlas/data-federation/overview/) (available for MongoDB) | NS | FS | FS | 
| AWS | [FS](https://aws.amazon.com/athena/) | [FS](https://docs.aws.amazon.com/athena/latest/ug/federated-queries.html) | [FS](https://docs.aws.amazon.com/glue/latest/dg/data-quality-anomaly-detection.html) | FS | [FS](https://aws.amazon.com/blogs/big-data/unstructured-data-management-and-governance-using-aws-ai-ml-and-analytics-services/) | 
| CKAN | [FS](https://docs.ckan.org/en/2.9/maintaining/datastore.html) (PostgreSQL; [open issue](https://github.com/ckan/ckan/issues/7551) on other SQL engines | [FS](https://ckan.org/features/federate) | NS | FS | FS |
| Collibra | [FS](https://www.collibra.com/products/core-services/data-notebook) | [FS](https://www.collibra.com/products/core-services) | [FS](https://www.collibra.com/products/data-quality-and-observability#sub-menu-features) | FS | [PS](https://marketplace.collibra.com/listings/data-x-ray-for-collibra-unstructured-data-intelligence/) |
| Databricks | [FS](https://www.databricks.com/product/photon) | [FS](https://docs.databricks.com/aws/en/sql/language-manual/sql-ref-federated-queries) | [FS](https://www.databricks.com/blog/near-real-time-anomaly-detection-delta-live-tables-and-databricks-machine-learning) | FS | [FS](https://www.databricks.com/resources/webinar/hassle-free-data-ingestion-part-3) | 
| DataHub | [NS](https://datahubproject.io/docs/api/graphql/overview/) (uses GraphQL API instead) | [FS](https://datahubproject.io/docs/architecture/architecture/) | [FS](https://datahubproject.io/cloud/) (Cloud)| FS | PS |
| dbt | NS (relies on query engine of underlying database) | NS | NS | FS | LS |
| Great Expectations | NS | NS | [LS](https://qxf2.com/blog/outlier-detection-algorithms-using-great-expectations/) | FS | LS |
| Oracle - Native | | | | | |
| OpenMetadata | [PS](https://atlan.com/open-source-data-catalog-tools/) (uses integration with Elasticsearch and PostgreSQL) | [PS](https://github.com/open-metadata/OpenMetadata) (uses a central metadata repository) | [FS](https://docs.open-metadata.org/latest/how-to-guides/data-quality-observability/anomaly-detection) | FS | [FS](https://docs.open-metadata.org/latest/connectors/storage) |

### Integration & Development

| Tool Name | Pre-Built Connectors | Automation Capabilities | CI/CD Integration | SDK Availability | API Documentation |
|-----------|----------------------|-------------------------|-------------------|------------------|-------------------|
| Apache Atlas |  |  | | | |
| AWS | | | | | |
| CKAN | [FS](https://extensions.ckan.org/) |  |  | [FS](https://github.com/ckan/awesome-ckan) | [FS](https://docs.ckan.org/en/2.11/api/index.html) |
| Collibra | | | | | |
| Databricks | | | | | |
| DataHub | | | | | |
| dbt | | | | | |
| Great Expectations | | | | | |
| Oracle - Native | | | | | |
| OpenMetadata | | | | | |

### Infrastructure & Resources

| Tool Name | Data Storage Options | On-Prem Support | Cloud Support |
|-----------|----------------------|-------------|------------|
| Apache Atlas | HBase (JanusGraph 1.0.0) |  |  |
| AWS | S3/Various AWS Services |  |  |
| CKAN | [Datastore](https://ckan.org/features/datastore) |  |  |
| Collibra | Multiple options |  |  |
| Databricks | Delta Lake/Various Cloud Storage |  |  |
| DataHub | MySQL/Elasticsearch/Neo4j |  |  |
| dbt | Works with existing data warehouse  |  |  |
| Great Expectations | No storage (validates in-place) |  |  |
| Oracle - Native | | | |
| OpenMetadata | MySQL/PostgreSQL, Elasticsearch/OpenSearch |  |  |

### Compliance & Security

| Tool Name | GDPR Compliance | HIPAA Compliance | Security Compliance | FedRAMP Status | Data Encryption | Authentication Methods | Notes |
|-----------|-----------------|------------------|------------------|----------------|-----------------|------------------------|-----------------|
| Apache Atlas | LS | LS | U | Only applicable to cloud services | FS | [File, Kerberos, LDAP](https://atlas.apache.org/1.1.0/Atlas-Authentication.html), [SSL, Service Authentication, SPNEGO-based HTTP Authentication](https://atlas.apache.org/1.1.0/Security.html) | Not explicitly compliant but can be used to achieve compliance with GDPR, HIPAA, ISO 27001 |
| AWS | FS | FS | [Security compliances listed](https://aws.amazon.com/compliance/iso-certified/) | [Authorized (High)](https://aws.amazon.com/compliance/fedramp/) | FS | [IAM](https://docs.aws.amazon.com/iam/)| |
| CKAN | [LS](https://github.com/ckan/ckan/issues/4361)/[PS](https://www.datopian.com/showcase/case-studies/ubdc-data-portal-revamp-ckan-powered-secure-gdpr-compliant) | [PS](https://www.keitaro.com/insights/2023/08/07/streamlining-data-management-with-ckan-and-keycloak-integration/) | [NS](https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/998119544445508) | U | NS | [SSO](https://extensions.ckan.org/extension/saml2auth/), [Basic Auth (MFA via Keycloak)](https://www.keitaro.com/insights/2023/08/07/streamlining-data-management-with-ckan-and-keycloak-integration/), [Public key authentication](https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/998119544445508) | [CKANEXT-SECURITY](https://github.com/data-govt-nz/ckanext-security) |
| Collibra | FS | FS | [Security compliances listed](https://www.collibra.com/company/trust-center#sub-menu-compliance) | [Authorized (Moderate)](https://www.collibra.com/resources/collibra-and-fedramp) | FS | [SSO](https://productresources.collibra.com/docs/collibra/latest/Content/Console/Infrastructure/DGCService/SecurityConfiguration/co_single-sign-on.htm), [LDAP](https://productresources.collibra.com/docs/collibra/latest/Content/Console/Infrastructure/DGCService/SecurityConfiguration/co_LDAP-configuration.htm), [SAML](https://productresources.collibra.com/docs/collibra/latest/Content/Console/Infrastructure/DGCService/SecurityConfiguration/SAML/co_about-saml.htm), [JSON Web Token](https://productresources.collibra.com/docs/collibra/latest/Content/Console/Infrastructure/DGCService/SecurityConfiguration/JWT/to_JWT-authentication.htm) | |
| Databricks | [FS](https://www.databricks.com/trust/compliance/gdpr) | [FS](https://docs.databricks.com/aws/en/security/privacy/hipaa) | [Security compliances listed](https://www.databricks.com/trust/compliance/iso-27001) | [Integrates with High and Moderate supported clouds (AWS and Azure)](https://www.databricks.com/trust/compliance/fedramp) | FS | [SSO, OAuth](https://docs.databricks.com/aws/en/security/auth) | |
| DataHub | LS | LS | U  | U | U | [SSO, JaaS, Basic Auth, Access Tokens](https://datahubproject.io/docs/authentication) | Not explicitly compliant but can be used to achieve compliance with GDPR, HIPAA, ISO 27001 |
| dbt | FS | FS | [Security compliances listed](https://www.getdbt.com/security) | U | FS | [SSO and OAuth](https://docs.getdbt.com/docs/cloud/manage-access/sso-overview), [Authentication Tokens](https://docs.getdbt.com/docs/dbt-cloud-apis/authentication) | |
| Great Expectations | U | U | [SOC 2 Type II](https://trust.greatexpectations.io/) | U | FS | [SSH, Basic Auth](https://trust.greatexpectations.io/controls#infrastructure-security), [SSO (Enterprise), Access Tokens](https://docs.greatexpectations.io/docs/cloud/users/manage_users)| |
| Oracle - Native | | | | | | | |
| OpenMetadata | PS | PS | U | U | PS | [SSO](https://docs.open-metadata.org/latest/deployment/security), [Basic Auth](https://docs.open-metadata.org/latest/deployment/security/basic-auth), [LDAP](https://docs.open-metadata.org/latest/deployment/security/ldap), [SSL](https://docs.open-metadata.org/latest/deployment/security/enable-ssl), [JWT Tokens](https://docs.open-metadata.org/latest/deployment/security/enable-jwt-tokens) | |

### Notes & References

| Tool Name | Key Strengths | Key Limitations | Notable Use Cases | Documentation Link | Community/Forum Link |
|-----------|---------------|-----------------|-------------------|-------------------|---------------------|
| Apache Atlas | | | | [Documentation](https://atlas.apache.org/) | [GitHub](https://github.com/apache/atlas) | 
| AWS | | | | [Documentation](https://docs.aws.amazon.com/) | [AWS Forums](https://forums.aws.amazon.com/) |
| CKAN | | | | [Documentation](https://docs.ckan.org/) | [GitHub](https://github.com/ckan/ckan) |
| Collibra | | | | [Documentation](https://productresources.collibra.com/docs/collibra/latest/Content/Home.htm?utm_source=Bevy&utm_medium=community&utm_campaign=Bevy&utm_content=Documentation/) | [Community Portal](https://community.collibra.com/) | 
| Databricks | | | | [Documentation](https://www.databricks.com/product/unity-catalog) | [Databricks Community](https://community.databricks.com/) | 
| DataHub | | | | [Documentation](https://datahubproject.io/docs/) | [GitHub](https://github.com/datahub-project/datahub) | 
| dbt | | | | [Documentation](https://docs.getdbt.com/) | [GitHub](https://github.com/dbt-labs/dbt-core) | 
| Great Expectations | | | | [Documentation](https://docs.greatexpectations.io/) | [GitHub](https://github.com/great-expectations/great_expectations) | 
| Oracle - Native | | | | | | |
| OpenMetadata | | | | [Documentation](https://docs.open-metadata.org/) | [GitHub](https://github.com/open-metadata/OpenMetadata) | 