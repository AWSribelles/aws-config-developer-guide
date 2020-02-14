# fms\-shield\-resource\-policy\-check<a name="fms-shield-resource-policy-check"></a>

Checks whether an Application Load Balancer, Amazon CloudFront distributions, Elastic Load Balancer or Elastic IP has AWS Shield protection\. This rule also checks if they have web ACL associated for Application Load Balancer and Amazon CloudFront distributions\. 

**Identifier:** FMS\_SHIELD\_RESOURCE\_POLICY\_CHECK

**Trigger type:** Configuration changes

**Parameters:**

 webACLId  
The `WebACLId` of the web ACL\. 

 resourceTags  
The resource tags associated with the rule \(for example, `{ "tagKey1" : ["tagValue1"], "tagKey2" : ["tagValue2", "tagValue3"] }"`\)\. 

 excludeResourceTags  
If true, exclude the resources that match the `resourceTags`\. If false, include all the resources that match the `resourceTags`\. 

 fmsManagedToken  
A token generated by AWS Firewall Manager when creating the rule in your account\. AWS Config ignores this parameter when you create this rule\. 

 fmsRemediationEnabled  
If true, AWS Firewall Manager will update NON\_COMPLIANT resources according to FMS policy\. AWS Config ignores this parameter when you create this rule\.

## AWS CloudFormation template<a name="w4aac13c29c17d161c13"></a>

To create AWS Config managed rules with AWS CloudFormation templates, see [Creating AWS Config Managed Rules With AWS CloudFormation Templates](aws-config-managed-rules-cloudformation-templates.md)\.