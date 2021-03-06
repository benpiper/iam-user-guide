# Using Multi\-Factor Authentication \(MFA\) in AWS<a name="id_credentials_mfa"></a>

For increased security, we recommend that you configure multi\-factor authentication \(MFA\) to help protect your AWS resources\.

**Topics**
+ [What Is MFA?](#id_credentials_mfa-what-is-mfa)
+ [Enabling MFA Devices](id_credentials_mfa_enable.md)
+ [Checking MFA Status](id_credentials_mfa_checking-status.md)
+ [Resynchronizing Virtual and Hardware MFA Devices](id_credentials_mfa_sync.md)
+ [Deactivating MFA Devices](id_credentials_mfa_disable.md)
+ [What If an MFA Device Is Lost or Stops Working?](id_credentials_mfa_lost-or-broken.md)
+ [Configuring MFA\-Protected API Access](id_credentials_mfa_configure-api-require.md)
+ [Sample Code: Requesting Credentials with Multi\-factor Authentication](id_credentials_mfa_sample-code.md)

## What Is MFA?<a name="id_credentials_mfa-what-is-mfa"></a>

MFA adds extra security because it requires users to provide unique authentication from an AWS supported MFA mechanism in addition to their regular sign\-in credentials when they access AWS websites or services: 
+ **Virtual MFA devices**\. A software app that runs on a phone or other mobile device and emulates a physical device\. The device generates a six\-digit numeric code based upon a time\-synchronized one\-time password algorithm\. The user must type a valid code from the device on a second webpage during sign\-in\. Each virtual MFA device assigned to a user must be unique\. A user cannot type a code from another user's virtual MFA device to authenticate\. For a list of a few supported apps that you can use as virtual MFA devices, see [Multi\-Factor Authentication](http://aws.amazon.com/iam/details/mfa/)\. For instructions on setting up a virtual MFA device with AWS, see [Enabling a Virtual Multi\-factor Authentication \(MFA\) Device \(Console\)](id_credentials_mfa_enable_virtual.md)\.
+ **U2F security key**\. A device that you plug into a USB port on your computer\. U2F is an open authentication standard hosted by the [FIDO Alliance](https://fidoalliance.org)\. When you enable a U2F security key, you sign in by entering your credentials and then tapping the device instead of manually entering a code\. For information on supported AWS U2F security keys, see [Multi\-Factor Authentication](http://aws.amazon.com/iam/details/mfa/)\. For instructions on setting up a U2F security key with AWS, see [Enabling a U2F Security Key \(Console\)](id_credentials_mfa_enable_u2f.md)\. 
+ **Hardware MFA device**\. A hardware device that generates a six\-digit numeric code based upon a time\-synchronized one\-time password algorithm\. The user must type a valid code from the device on a second webpage during sign\-in\. Each MFA device assigned to a user must be unique\. A user cannot type a code from another user's device to be authenticated\. For information on supported hardware MFA devices, see [Multi\-Factor Authentication](http://aws.amazon.com/iam/details/mfa/)\. For instructions on setting up a hardware MFA device with AWS, see [Enabling a Hardware MFA Device \(Console\)](id_credentials_mfa_enable_physical.md)\.
+ **SMS text message\-based MFA**\. A type of MFA in which the IAM user settings include the phone number of the user's SMS\-compatible mobile device\. When the user signs in, AWS sends a six\-digit numeric code by SMS text message to the user's mobile device\. The user is required to type that code on a second webpage during sign\-in\. Note that SMS\-based MFA is available only for IAM users\. You cannot use this type of MFA with the AWS account root user\. For more information about enabling SMS text messaging\-based MFA, see [PREVIEW – Enabling SMS Text Message MFA Devices](id_credentials_mfa_enable_sms.md)\.
**Note**  
AWS will soon end support for SMS multi\-factor authentication \(MFA\)\. We are not allowing new customers to preview this feature\. We recommend that existing customers switch to one of the following alternative methods of MFA: [virtual \(software\-based\) MFA device](id_credentials_mfa_enable_virtual.md), [U2F security key](id_credentials_mfa_enable_u2f.md), or [hardware MFA device](id_credentials_mfa_enable_physical.md)\.
**Tip**  
You can view users in your account with an assigned SMS MFA device\. To do so, go to the IAM console, choose **Users** from the navigation pane, and look for users with **SMS** in the **MFA** column of the table\.

**Note**  
When you enable MFA for the AWS account root user, it affects only the root user credentials\. IAM users in the account are distinct identities with their own credentials, and each identity has its own MFA configuration\.

For answers to commonly asked questions about AWS MFA, go to the [AWS Multi\-Factor Authentication FAQs](http://aws.amazon.com/iam/faqs/#MFA_FAQs)\. 