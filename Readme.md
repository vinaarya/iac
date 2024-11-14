[Skip to main content](#main)

[HashiConf 2024Now streaming live from Boston!Attend for free](https://live.hashiconf.com)

Dismiss alert

Sign In [Sign Up](/sign-up)

Theme

DarkLightSystem

[Associate Prep](/terraform/tutorials/certification-003)

The Terraform Associate certification is for cloud engineers specializing in operations, IT, or development who know the basic concepts and skills of HashiCorp Terraform. While experience using Terraform in production is helpful, performing the exam objectives in a demo environment can be sufficient to pass the exam. The exam expects familiarity with the enterprise features available in HCP Terraform, and what Terraform Community Edition does and does not support.

This guide lists the specific exam objectives and resources you can study to demonstrate those objectives. Review our
[learning path](/terraform/tutorials/certification-003/associate-study-003) for a start-to-finish list of resources you can use to prepare for the exam. While the tutorials listed may use specific cloud providers to introduce the learning objectives, provider-specific knowledge is not necessary for the exam.

Visit the [HashiCorp Cloud Engineer Certification page](/certifications/infrastructure-automation) for more information and to register for the exam.

## [exam content list permalink](/terraform/tutorials/certification-003/associate-review-003\#exam-content-list) Exam content list

Below is a direct mapping of each HashiCorp Certified: Terraform Associate exam
objective to a documentation page or tutorial that demonstrates it.
Experienced candidates can use this as a reference to focus on the specific
objectives they need to review in more detail.

|  |  |  |  |
| --- | --- | --- | --- |
| **1** | **Understand Infrastructure as Code (IaC) concepts** | **Documentation** | **Tutorial** |
| 1a | Explain what IaC is | [What is Terraform?](/terraform/intro)<br>[Infrastructure as Code in a Private or Public Cloud](https://www.hashicorp.com/blog/infrastructure-as-code-in-a-private-or-public-cloud) | [Introduction to Infrastructure as Code with Terraform](/terraform/tutorials/aws-get-started/infrastructure-as-code) |
| 1b | Describe advantages of IaC patterns | [Infrastructure as code video](https://www.hashicorp.com/resources/what-is-infrastructure-as-code)<br>[Infrastructure as Code in a Private or Public Cloud](https://www.hashicorp.com/blog/infrastructure-as-code-in-a-private-or-public-cloud) | [Introduction to Infrastructure as Code with Terraform](/terraform/tutorials/aws-get-started/infrastructure-as-code) |
| **2** | **Understand the purpose of Terraform (vs other IaC)** | **Documentation** | **Tutorial** |
| 2a | Explain multi-cloud and provider-agnostic benefits | [Multi-Cloud Deployment](/terraform/intro/use-cases#multi-cloud-deployment) |  |
| 2b | Explain the benefits of state | [Purpose of Terraform State](/terraform/language/v1.1.x/state/purpose) | [Manage Resources in Terraform State](/terraform/tutorials/state/state-cli) |
| **3** | **Understand Terraform basics** | **Documentation** | **Tutorial** |
| 3a | Install and version Terraform providers | [Providers](/terraform/language/v1.1.x/providers/configuration)<br>[Specifiying Provider Requirements](/terraform/language/settings#specifying-provider-requirements)<br>[Dependency Lock File](/terraform/language/files/dependency-lock) | [Manage Terraform Versions](/terraform/tutorials/configuration-language/versions)<br>[Lock and Upgrade Provider Versions](/terraform/tutorials/configuration-language/provider-versioning) |
| 3b | Describe plugin-based architecture | [Providers Summary](/terraform/language/providers)<br>[How Terraform Works with Plugins](/terraform/plugin/how-terraform-works) | [Community Provider tutorials](/terraform/tutorials/community-providers) |
| 3c | Write Terraform configuration using multiple providers | [Provider Configuration](/terraform/language/providers/configuration) | [Define Infrastructure with Terraform Resources](/terraform/tutorials/configuration-language/resource) |
| 3d | Describe how Terraform finds and fetches providers | [Provider Configuration](/terraform/language/v1.1.x/providers/configuration) | [Initialize Terraform Configuration](/terraform/tutorials/cli/init) |
| **4** | **Use Terraform outside the core workflow** | **Documentation** | **Tutorial** |
| 4a | Describe when to use `terraform import` to import existing infrastructure into your Terraform state | [Command: import](/terraform/cli/v1.1.x/commands/import)<br>[Import usage tips](/terraform/cli/import/usage) |  |
| 4b | Use `terraform state` to view Terraform state | [State Command](/terraform/cli/v1.1.x/commands/state) | [Manage Resources in Terraform State](/terraform/tutorials/state/state-cli) |
| 4c | Describe when to enable verbose logging and what the outcome/value is | [Debugging Terraform](/terraform/internals/v1.1.x/debugging) | [Troubleshoot Terraform](/terraform/tutorials/configuration-language/troubleshooting-workflow#enable-terraform-logging) |
| **5** | **Interact with Terraform modules** | **Documentation** | **Tutorial** |
| 5a | Contrast and use different module source options including the public Terraform Registry | [Finding and Using Modules](/terraform/registry/modules/use) | [Modules Overview](/terraform/tutorials/modules/module)<br>[Use Modules from the Registry](/terraform/tutorials/modules/module-use) |
| 5b | Interact with module inputs and outputs | [Input Variables](/terraform/language/values/variables)<br>[Accessing Module Output Values](/terraform/language/v1.1.x/modules/syntax#accessing-module-output-values) | [Use Modules from the Registry](/terraform/tutorials/modules/module-use) |
| 5c | Describe variable scope within modules/child modules | [Input Variables](/terraform/language/v1.1.x/values/variables)<br>[Calling a Child Module](/terraform/language/v1.1.x/modules/syntax) | [Build and Use a Local Module](/terraform/tutorials/modules/module-create) |
| 5d | Set module version | [Module Versions](/terraform/language/v1.1.x/modules/syntax#version) | [Use Modules from the Registry](/terraform/tutorials/modules/module-use) |
| **6** | **Use the core Terraform workflow** | **Documentation** | **Tutorial** |
| 6a | Describe Terraform workflow ( Write -> Plan -> Create ) | [The Core Terraform Workflow](https://www.terraform.io/guides/core-workflow.html) | [Build Infrastructure](/terraform/tutorials/aws-get-started/aws-build) |
| 6b | Initialize a Terraform working directory ( `terraform init`) | [Command: init](/terraform/cli/v1.1.x/commands/init) | [Initialize Terraform Configuration](/terraform/tutorials/cli/init) |
| 6c | Validate a Terraform configuration ( `terraform validate`) | [Command: validate](/terraform/cli/v1.1.x/commands/validate) | [Troubleshoot Terraform](/terraform/tutorials/configuration-language/troubleshooting-workflow#validate-your-configuration) |
| 6d | Generate and review an execution plan for Terraform ( `terraform plan`) | [Command: plan](/terraform/cli/v1.1.x/commands/plan) | [Create a Terraform Plan](/terraform/tutorials/cli/plan) |
| 6e | Execute changes to infrastructure with Terraform ( `terraform apply`) | [Command: apply](/terraform/cli/v1.1.x/commands/apply) | [Apply Terraform Configuration](/terraform/tutorials/cli/apply) |
| 6f | Destroy Terraform managed infrastructure ( `terraform destroy`) | [Command: destroy](/terraform/cli/v1.1.x/commands/destroy) | [Destroy Infrastructure](/terraform/tutorials/aws-get-started/aws-destroy) |
| 6g | Apply formatting and style adjustments to a configuration ( `terraform fmt`) | [Command: fmt](/terraform/cli/v1.1.x/commands/fmt) | [Troubleshoot Terraform](/terraform/tutorials/configuration-language/troubleshooting-workflow#format-the-configuration) |
| **7** | **Implement and maintain state** | **Documentation** | **Tutorial** |
| 7a | Describe default `local` backend | [Backends](/terraform/language/v1.1.x/settings/backends)<br>[Backend Type: `local`](/terraform/language/v1.1.x/settings/backends/local) | [Initialize Terraform Configuration](/terraform/tutorials/cli/init) |
| 7b | Describe state locking | [State Locking](/terraform/language/v1.1.x/state/locking) |  |
| 7c | Handle backend and cloud integration authentication methods | [Command: login](/terraform/cli/commands/login) | [Log in to HCP Terraform from the CLI](/terraform/tutorials/cloud-get-started/cloud-login) |
| 7d | Differentiate remote state back end options | [Backend Types](/terraform/language/v1.1.x/settings/backends) | [Store Remote State](/terraform/tutorials/aws-get-started/aws-remote) |
| 7e | Manage resource drift and Terraform state | [Refresh-Only Mode](/terraform/cloud-docs/run/modes-and-options#refresh-only-mode) | [Manage Resource Drift](/terraform/tutorials/state/resource-drift)<br>[Use Refresh-Only Mode to Sync Terraform State](/terraform/tutorials/state/refresh) |
| 7f | Describe `backend` block and cloud integration in configuration | [HCP Terraform Configuration](/terraform/language/settings/terraform-cloud)<br>[Backend Configuration](/terraform/language/v1.1.x/settings/backends/configuration) | [Create a Workspace](/terraform/tutorials/cloud-get-started/cloud-workspace-create)<br>[Store Remote State](/terraform/tutorials/aws-get-started/aws-remote) |
| 7g | Understand secret management in state files | [Sensitive Data in State](/terraform/language/v1.1.x/state/sensitive-data) | [Protect Sensitive Input Variables](/terraform/tutorials/configuration-language/sensitive-variables#sensitive-values-in-state) |
| **8** | **Read, generate, and modify configuration** | **Documentation** | **Tutorial** |
| 8a | Demonstrate use of variables and outputs | [Input Variables](/terraform/language/v1.1.x/values/variables)<br>[Output Values](/terraform/language/v1.1.x/values/outputs) | [Customize Terraform Configuration with Variables](/terraform/tutorials/configuration-language/variables)<br>[Output Data from Terraform](/terraform/tutorials/configuration-language/outputs) |
| 8b | Describe secure secret injection best practice | [Vault Provider for Terraform](https://registry.terraform.io/providers/hashicorp/vault/latest/docs) | [Inject Secrets into Terraform Using the Vault Provider](/terraform/tutorials/secrets/secrets-vault) |
| 8c | Understand the use of collection and structural types | [Complex Types](/terraform/language/v1.1.x/expressions/type-constraints#complex-types) | [Customize Terraform Configuration with Variables](/terraform/tutorials/configuration-language/variables) |
| 8d | Create and differentiate `resource` and `data` configuration | [Resources](/terraform/language/v1.1.x/resources)<br>[Data Sources](/terraform/language/v1.1.x/data-sources) | [Query Data Sources](/terraform/tutorials/configuration-language/data-sources) |
| 8e | Use resource addressing and resource parameters to connect resources together | [Resource Addressing](/terraform/cli/v1.1.x/state/resource-addressing)<br>[References to Named Values](/terraform/language/v1.1.x/expressions/references) | [Create Resource Dependencies](/terraform/tutorials/configuration-language/dependencies) |
| 8f | Use HCL and Terraform functions to write configuration | [Built-in Functions](/terraform/language/v1.1.x/functions) | [Perform Dynamic Operations with Functions](/terraform/tutorials/configuration-language/functions)<br>[Create Dynamic Expressions](/terraform/tutorials/configuration-language/expressions) |
| 8g | Describe built-in dependency management (order of execution based) | [Resource Graph](/terraform/internals/v1.1.x/graph) | [Create Resource Dependencies](/terraform/tutorials/configuration-language/dependencies)<br>[Target resources](/terraform/tutorials/state/resource-targeting) |
| **9** | **Understand HCP Terraform capabilities** | **Documentation** | **Resource** |
| 9a | Explain how HCP Terraform helps to manage infrastructure | [HCP Terraform Overview](/terraform/cloud-docs)<br>[HCP Terraform Workflow](/terraform/cloud-docs/overview#terraform-workflow)<br>[Workspaces](/terraform/cloud-docs/workspaces) | [HCP Terraform Get Started Collection](/terraform/tutorials/cloud-get-started)<br>[Share Modules in the Private Registry](/terraform/tutorials/modules/module-private-registry-share) |
| 9b | Describe how HCP Terraform enables collaboration and governance | [HCP Terraform Teams](/terraform/cloud-docs/users-teams-organizations/teams)<br>[Sentinel](/terraform/cloud-docs/policy-enforcement/sentinel) | [Manage Versions in HCP Terraform](/terraform/tutorials/cloud/cloud-versions)<br>[Manage Permissions in HCP Terraform](/terraform/tutorials/cloud/cloud-permissions)<br>[Enforce a Policy](/terraform/tutorials/cloud-get-started/policy-quickstart) |

## [next steps permalink](/terraform/tutorials/certification-003/associate-review-003\#next-steps) Next steps

Review the [learning path](/terraform/tutorials/certification-003/associate-study-003) to practice all of the exam objectives. Check out the [sample questions](/terraform/tutorials/certification-003/associate-questions) to review the exam question format.

**[Sign up for the exam here!](https://cp.certmetrics.com/hashicorp/en/login)**

**Was this tutorial helpful?**

YesNo

[Previous\\
Associate Learning Path](/terraform/tutorials/certification-003/associate-study-003) [Next\\
Associate Sample Questions](/terraform/tutorials/certification-003/associate-questions)

## Stay Informed

Sign up to be notified with updates to the HashiCorp Product Certifications program and to receive news and information about HashiCorp products.

Email\*

Send me news about HashiCorp products, releases and events.

By submitting this form, you acknowledge and agree that HashiCorp will process your personal information in accordance with the [Privacy Policy](https://www.hashicorp.com/privacy).

Submit
