---
title: "Configure your Yammer network"
ms.author: v-irpast
author: IrenePasternack
manager: pamgreen
ms.date: 11/6/2018
ms.audience: Admin
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.custom: Adm_Yammer
ms.service: yammer
search.appverid:
- MET150
- MOE150
- YAE150
ms.assetid: f886e916-fe64-41de-be52-38d458250fa5
description: "Use the Yammer admin tools to set up your Yammer network. Covers options for configuration, design, admins, usage policy, external networks, and activity stream keys."
---

# Configure your Yammer network

Do these basic network configuration tasks in the Yammer admin center before you invite users to use Yammer Enterprise so that all users get a consistent experience. 
  
As you're getting started with Yammer, review the links in [Yammer admin help](../yammer-landing-page.md) for other tasks you might want to do, such as [customizing the look of your Yammer network](customize-the-look-of-yammer.md), [reviewing security and compliance settings](../manage-security-and-compliance/security-and-compliance.md), and making sure your [email system is configured properly](configure-email-and-yammer.md).
  
To access the Yammer network configuration tools:
  
- In Office 365, go to **Admin** \> **Yammer** \> **Configuration**.
    
- Or, in Yammer, click the Yammer settings icon ![Yammer settings icon](../media/9704ce70-56ce-43f7-96c6-f253b0413d40.png) and go to **Network Admin** \> **Configuration**. 
    
## Set the Yammer network name
<a name="NetworkName"> </a>

> [!IMPORTANT] 
> In Office 365 Yammer networks, the name in the Office 365 company profile overrides the **Network name** setting in Yammer. To change the Office 365 company profile settings, see [Change your organization's address, technical contact, and more](https://support.office.com/en-us/article/Change-your-organization-s-address-technical-contact-and-more-a36e5a52-4df2-479e-bb97-9e67b8483e10)

- On the **Configuration** page, in the **Basics** section, specify the following: 
    
  - **Network name:** This is the friendly name of your network that is used in the Yammer header. Note that this name is overwritten by the name used in the Office 365 company profile.
    
  - **Message prompt:** This prompt is visible at the top of each Yammer group page, under **Update**. 
    
## Review domains set up to work with your Yammer network
<a name="ReviewDomains"> </a>

- On the **Configuration** page, in the **Network Domains** section, select **Click here** to verify that the correct domains are listed. These are the domains that have been set up in Office 365. For more information, see [Add a domain to Office 365](https://support.office.com/article/17f4aa9b-5ece-4af8-8be4-a5e8ff8367f2).
    
## Require users to confirm email messages posted via email before posting
<a name="ConfirmEmailPosts"> </a>

- On the **Configuration** page, in the **Email Settings** section, select whether to require users to confirm messages posted via email before posting. 
    
    For more information about email and Yammer, see [Configure email and Yammer](configure-email-and-yammer.md).
    
## Restrict who can upload files and limit file formats
<a name="RestrictFiles"> </a>

1. On the **Configuration** page, in the **File Upload Permissions** section, set which types of files can be uploaded. 
    
2. To allow unlimited file types, select **Allow people to upload and attach files in any format**. 
    
    Any number of files, images, or both can be attached to any message or reply, with each file size limited to 5 GB. By default, file attachments are enabled. 
    
    > [!NOTE]
    > Users will get an error message if they try to upload an image that is wider than 7680 pixels or taller than 4320 pixels. 
  
3. To restrict who can upload files, clear the **Allow people to upload and attach files in any format** checkbox. You'll then see three options: 
    
      - **Allow people to upload and attach files in any format**
    
      - **Only allow people to upload and attach image or video files**: Limits attachments to images and videos. Yammer determines file type by extension. 
    
         Yammer uses Azure Media Services to make videos viewable within the network. For more information, see [Azure Media Services](https://go.microsoft.com/fwlink/?LinkId=698736).
    
      - **Don't allow anyone to upload or attach files**: This prevents people from uploading and attaching new files; however, existing attachments are not be affected.
    
> [!NOTE]
> When files are stored in Yammer, there is no virus check. An admin can export the files and perform an offline virus scan on them, and this process can be automated with custom scripting.<br><br>For Office 365 connected Yammer groups that store files in SharePoint, virus checking is done as the file is uploaded. For more information, see [Virus detection in SharePoint Online](https://docs.microsoft.com/office365/securitycompliance/virus-detection-in-spo).

> [!TIP]
> Any admin can delete any file, and group admins can delete files posted to the groups that they manage.<br><br>To delete files, a network admin can click the Yammer **Settings** icon and then click **Files**. This brings up the **Files** directory for the entire network. Group admins can delete files posted to a group by going to the **Files** tab within the group they administer. 
  
## Enable or restrict the use of third-party apps
<a name="RestrictApps"> </a>

The growing network of partners and developers in Yammer continue to build third-party applications using the Yammer API. To find the list of current apps, including integrations with Microsoft SharePoint, Microsoft Flow, Microsoft Dynamics, and many more business applications, click **App Directory** on your main Yammer page or go directly to the [App Directory](https://go.microsoft.com/fwlink/?LinkId=524143).
  
- On the **Configuration** page, in the **Enabled Features** section, specify whether to allow 3rd party applications 
    
    > [!CAUTION]
    > Clearing this setting prevents users from adding or accessing these applications. Note that all users, including verified admins, will lose access to apps that were added prior to clearing this setting. 
  
## Allow users to view an org chart in Yammer
<a name="RestrictApps"> </a>

The org chart was deprecated for Office 365 Yammer networks in May 2018. Office charts are available in Skype for Business and Delve. For more information, see [Find info from a contact card in Skype for Business](https://support.office.com/en-us/article/Find-info-from-a-contact-card-in-Skype-for-Business-d797905c-66f0-4248-b473-c49e3c9a0767) and [How can I find people and information in Office Delve?](https://support.office.com/en-us/article/How-can-I-find-people-and-information-in-Office-Delve-5b8bffdd-a50a-430a-8570-09b39481887c)
  
    
## Allow message translation
<a name="RestrictApps"> </a>

This feature gives users the option to translate messages from [any language supported by Microsoft Translator](https://www.microsoft.com/en-us/translator/languages.aspx) into the network's default language. To enable this feature, the network admin must accept a Terms and Services agreement in order to use Microsoft's proprietary translation technology. This feature is disabled by default. 
  
- On the **Configuration** page, in the **Enabled Features** section, select whether to allow **Message Translation**.
