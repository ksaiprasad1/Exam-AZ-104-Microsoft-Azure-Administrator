# Configure Azure Policy (5 of 31)

Learn how to configure Azure Policy to implement compliance requirements

URL : [Configure Azure Policy (5 of 31)](https://learn.microsoft.com/en-us/shows/on-demand-instructor-led-training-series/az-104-module-5)

*Key Points from Module 5*
- Purpose of Azure Policy
- Ensures resources comply with organizational or regulatory requirements.
- Helps enforce standards like allowed regions, required tags, or security configurations.
- Policy Definitions
- Written in JSON format.
- Define rules such as “Require a tag and its value” or “Restrict VM sizes.”
- Policy Assignment
- Policies are assigned to a scope (management group, subscription, resource group).
- Scope determines which resources are evaluated.
- Effects of Policies
- Deny: Blocks non-compliant deployments.
- Audit: Flags non-compliant resources but allows deployment.
- Append/Modify: Adds or changes resource settings.
- DeployIfNotExists: Automatically deploys required configurations.
- Initiatives
- Group multiple policies into a single assignment for broader compliance goals.
- Example: A “Security Baseline” initiative may include encryption, tagging, and region restrictions.
- Compliance Evaluation
- Azure Policy continuously evaluates resources.
- New resources are enforced immediately; existing ones are marked non-compliant unless remediation is applied.
- Remediation Tasks
- Allow policies to fix existing resources (e.g., add missing tags).
- Work with DeployIfNotExists or Modify effects.

🎯 Why It Matters for AZ-104
- As an Azure Administrator, you must ensure governance and compliance across all resources.
- This module prepares you to:
- Assign built-in policies.
- Create custom policies.
- Use initiatives for large-scale governance.
- Monitor compliance through the Azure Policy dashboard.

In short: Module 5 teaches you how to use Azure Policy to enforce rules, evaluate compliance, and remediate non-compliant resources — a core skill for passing AZ-104 and managing enterprise-grade Azure environments.

*Important Points*

-When a policy is assigned at a higher scope, such as a resource group, it is automatically inherited by all resources within that scope. However, if a policy is assigned directly to an individual resource, it applies only to that resource and does not cascade to other resources in the group

-When new Policy is created..Polocy will get applied to the resources tht are created post policy creation time.. existing resources will not get that policy applied.. to get that policy applied we need to do - Remediation Tasks
-When a new policy is created, it is automatically enforced on resources that are created or updated after the policy assignment. Existing resources are only evaluated for compliance and will not be modified by default. To bring those existing resources into compliance, remediation tasks must be used.
