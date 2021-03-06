# Actions, Resources, and Condition Keys for Amazon Elastic Container Service<a name="list_amazonelasticcontainerservice"></a>

Amazon Elastic Container Service \(service prefix: `ecs`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/)\.
+ View a [list of the API operations available for this service](https://docs.aws.amazon.com/AmazonECS/latest/APIReference/)\.
+ Learn how to protect this service and its resources by [using IAM](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/IAM_policies.html) permission policies\.

**Topics**
+ [Actions Defined by Amazon Elastic Container Service](#amazonelasticcontainerservice-actions-as-permissions)
+ [Resources Defined by Amazon Elastic Container Service](#amazonelasticcontainerservice-resources-for-iam-policies)
+ [Condition Keys for Amazon Elastic Container Service](#amazonelasticcontainerservice-policy-keys)

## Actions Defined by Amazon Elastic Container Service<a name="amazonelasticcontainerservice-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  
[\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/IAM/latest/UserGuide/list_amazonelasticcontainerservice.html)

## Resources Defined by Amazon Elastic Container Service<a name="amazonelasticcontainerservice-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#amazonelasticcontainerservice-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ cluster ](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ECS_clusters.html)  |  arn:$\{Partition\}:ecs:$\{Region\}:$\{Account\}:cluster/$\{ClusterName\}  |   [ aws:ResourceTag/$\{TagKey\} ](#amazonelasticcontainerservice-aws_ResourceTag___TagKey_)   [ ecs:ResourceTag/$\{TagKey\} ](#amazonelasticcontainerservice-ecs_ResourceTag___TagKey_)   | 
|   [ container\-instance ](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ECS_instances.html)  |  arn:$\{Partition\}:ecs:$\{Region\}:$\{Account\}:container\-instance/$\{ContainerInstanceId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#amazonelasticcontainerservice-aws_ResourceTag___TagKey_)   [ ecs:ResourceTag/$\{TagKey\} ](#amazonelasticcontainerservice-ecs_ResourceTag___TagKey_)   | 
|   [ service ](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs_services.html)  |  arn:$\{Partition\}:ecs:$\{Region\}:$\{Account\}:service/$\{ServiceName\}  |   [ aws:ResourceTag/$\{TagKey\} ](#amazonelasticcontainerservice-aws_ResourceTag___TagKey_)   [ ecs:ResourceTag/$\{TagKey\} ](#amazonelasticcontainerservice-ecs_ResourceTag___TagKey_)   | 
|   [ task ](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/scheduling_tasks.html)  |  arn:$\{Partition\}:ecs:$\{Region\}:$\{Account\}:task/$\{TaskId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#amazonelasticcontainerservice-aws_ResourceTag___TagKey_)   [ ecs:ResourceTag/$\{TagKey\} ](#amazonelasticcontainerservice-ecs_ResourceTag___TagKey_)   | 
|   [ task\-definition ](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_definitions.html)  |  arn:$\{Partition\}:ecs:$\{Region\}:$\{Account\}:task\-definition/$\{TaskDefinitionFamilyName\}:$\{TaskDefinitionRevisionNumber\}  |   [ aws:ResourceTag/$\{TagKey\} ](#amazonelasticcontainerservice-aws_ResourceTag___TagKey_)   [ ecs:ResourceTag/$\{TagKey\} ](#amazonelasticcontainerservice-ecs_ResourceTag___TagKey_)   | 
|   [ task\-set ](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_sets.html)  |  arn:$\{Partition\}:ecs:$\{region\}:$\{Account\}:task\-set/$\{ClusterName\}/$\{ServiceName\}/$\{TaskSetId\}  |  | 

## Condition Keys for Amazon Elastic Container Service<a name="amazonelasticcontainerservice-policy-keys"></a>

Amazon Elastic Container Service defines the following condition keys that can be used in the `Condition` element of an IAM policy\. You can use these keys to further refine the conditions under which the policy statement applies\. For details about the columns in the following table, see [The Condition Keys Table](reference_policies_actions-resources-contextkeys.md#context_keys_table)\.

To view the global condition keys that are available to all services, see [Available Global Condition Keys](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.


****  

| Condition Keys | Description | Type | 
| --- | --- | --- | 
|   aws:RequestTag/$\{TagKey\}  |  | String | 
|   aws:ResourceTag/$\{TagKey\}  |  | String | 
|   aws:TagKeys  |  | String | 
|   ecs:ResourceTag/$\{TagKey\}  |  | String | 
|   [ ecs:cluster ](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/iam-policy-structure.html#amazon-ecs-keys)  | The ARN of an ECS cluster\. | ARN | 
|   [ ecs:container\-instances ](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/iam-policy-structure.html#amazon-ecs-keys)  | The ARN of an ECS container instance\. | ARN | 
|   [ ecs:service ](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/iam-policy-structure.html#amazon-ecs-keys)  | The ARN of an ECS service\. | ARN | 
|   [ ecs:task\-definition ](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/iam-policy-structure.html#amazon-ecs-keys)  | The ARN of an ECS task definition\. | ARN | 