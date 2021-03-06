# Actions, Resources, and Condition Keys for AWS Marketplace Procurement Systems Integration<a name="list_awsmarketplaceprocurementsystemsintegration"></a>

AWS Marketplace Procurement Systems Integration \(service prefix: `aws-marketplace`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/marketplace/latest/buyerguide/)\.
+ View a [list of the API operations available for this service](https://docs.aws.amazon.com/marketplace/latest/buyerguide/)\.
+ Learn how to protect this service and its resources by [using IAM](https://docs.aws.amazon.com/marketplace/latest/buyerguide/procurement-systems-integration.html) permission policies\.

**Topics**
+ [Actions Defined by AWS Marketplace Procurement Systems Integration](#awsmarketplaceprocurementsystemsintegration-actions-as-permissions)
+ [Resources Defined by AWS Marketplace Procurement Systems Integration](#awsmarketplaceprocurementsystemsintegration-resources-for-iam-policies)
+ [Condition Keys for AWS Marketplace Procurement Systems Integration](#awsmarketplaceprocurementsystemsintegration-policy-keys)

## Actions Defined by AWS Marketplace Procurement Systems Integration<a name="awsmarketplaceprocurementsystemsintegration-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  

| Actions | Description | Access Level | Resource Types \(\*required\) | Condition Keys | Dependent Actions | 
| --- | --- | --- | --- | --- | --- | 
|   [ DescribeProcurementSystemConfiguration ](https://docs.aws.amazon.com/marketplace/latest/buyerguide/procurement-systems-integration.html) \[permission only\] | Describes the Procurement System integration configuration \(e\.g\. Coupa\) for the individual account, or for the entire AWS Organization if one exists\. This action can only be performed by the master account if using an AWS Organization\. | Read |  |  |  | 
|   [ PutProcurementSystemConfiguration ](https://docs.aws.amazon.com/marketplace/latest/buyerguide/procurement-systems-integration.html) \[permission only\] | Creates or updates the Procurement System integration configuration \(e\.g\. Coupa\) for the individual account, or for the entire AWS Organization if one exists\. This action can only be performed by the master account if using an AWS Organization\. | Write |  |  |  | 

## Resources Defined by AWS Marketplace Procurement Systems Integration<a name="awsmarketplaceprocurementsystemsintegration-resources-for-iam-policies"></a>

AWS Marketplace Procurement Systems Integration has no service\-defined resources that can be used as the `Resource` element of an IAM policy statement\.

## Condition Keys for AWS Marketplace Procurement Systems Integration<a name="awsmarketplaceprocurementsystemsintegration-policy-keys"></a>

Marketplace Procurement Integration has no service\-specific context keys that can be used in the `Condition` element of policy statements\. For the list of the global context keys that are available to all services, see [Available Keys for Conditions](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.