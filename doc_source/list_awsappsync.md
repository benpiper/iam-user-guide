# Actions, Resources, and Condition Keys for AWS AppSync<a name="list_awsappsync"></a>

AWS AppSync \(service prefix: `appsync`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/appsync/latest/devguide/)\.
+ View a [list of the API operations available for this service](https://docs.aws.amazon.com/appsync/latest/APIReference/)\.
+ Learn how to protect this service and its resources by [using IAM](https://docs.aws.amazon.com/appsync/latest/devguide/security.html) permission policies\.

**Topics**
+ [Actions Defined by AWS AppSync](#awsappsync-actions-as-permissions)
+ [Resources Defined by AWS AppSync](#awsappsync-resources-for-iam-policies)
+ [Condition Keys for AWS AppSync](#awsappsync-policy-keys)

## Actions Defined by AWS AppSync<a name="awsappsync-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  
[\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/IAM/latest/UserGuide/list_awsappsync.html)

## Resources Defined by AWS AppSync<a name="awsappsync-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#awsappsync-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ datasource ](https://docs.aws.amazon.com/appsync/latest/devguide/attaching-a-data-source.html)  |  arn:$\{Partition\}:appsync:$\{Region\}:$\{Account\}:apis/$\{GraphQLAPIId\}/datasources/$\{DatasourceName\}  |  | 
|   [ graphqlapi ](https://docs.aws.amazon.com/appsync/latest/devguide/designing-a-graphql-api.html)  |  arn:$\{Partition\}:appsync:$\{Region\}:$\{Account\}:apis/$\{GraphQLAPIId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#awsappsync-aws_ResourceTag___TagKey_)   | 
|   [ field ](https://docs.aws.amazon.com/appsync/latest/devguide/configuring-resolvers.html)  |  arn:$\{Partition\}:appsync:$\{Region\}:$\{Account\}:apis/$\{GraphQLAPIId\}/types/$\{TypeName\}/fields/$\{FieldName\}  |  | 
|   [ type ](https://docs.aws.amazon.com/appsync/latest/devguide/designing-your-schema.html#adding-a-root-query-type)  |  arn:$\{Partition\}:appsync:$\{Region\}:$\{Account\}:apis/$\{GraphQLAPIId\}/types/$\{TypeName\}  |  | 
|   [ function ](https://docs.aws.amazon.com/appsync/latest/devguide/pipeline-resolvers.html)  |  arn:$\{Partition\}:appsync:$\{Region\}:$\{Account\}:apis/$\{GraphQLAPIId\}/functions/$\{FunctionId\}  |  | 

## Condition Keys for AWS AppSync<a name="awsappsync-policy-keys"></a>

AWS AppSync defines the following condition keys that can be used in the `Condition` element of an IAM policy\. You can use these keys to further refine the conditions under which the policy statement applies\. For details about the columns in the following table, see [The Condition Keys Table](reference_policies_actions-resources-contextkeys.md#context_keys_table)\.

To view the global condition keys that are available to all services, see [Available Global Condition Keys](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.


****  

| Condition Keys | Description | Type | 
| --- | --- | --- | 
|   [ aws:RequestTag/$\{TagKey\} ](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_condition-keys.html#condition-keys-requesttag)  | Filters actions based on the presence of tag key\-value pairs in the request | String | 
|   [ aws:ResourceTag/$\{TagKey\} ](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_condition-keys.html#condition-keys-resourcetag)  | Filters actions based on tag key\-value pairs attached to the resource | String | 
|   [ aws:TagKeys ](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_condition-keys.html#condition-keys-tagkeys)  | Filters actions based on the presence of tag keys in the request | String | 