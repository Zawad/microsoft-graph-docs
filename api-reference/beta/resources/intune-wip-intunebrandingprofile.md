---
title: "intuneBrandingProfile resource type"
description: "This entity contains data which is used in customizing the tenant level appearance of the Company Portal applications as well as the end user web portal."
author: "rolyon"
localization_priority: Normal
ms.prod: "Intune"
doc_type: resourcePageType
---

# intuneBrandingProfile resource type

> **Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.

> **Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.

This entity contains data which is used in customizing the tenant level appearance of the Company Portal applications as well as the end user web portal.

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List intuneBrandingProfiles](../api/intune-wip-intunebrandingprofile-list.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) collection|List properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects.|
|[Get intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Read properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.|
|[Create intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.|
|[Delete intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-delete.md)|None|Deletes a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).|
|[Update intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.|
|[assign action](../api/intune-wip-intunebrandingprofile-assign.md)|None|Not yet documented|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Profile Key|
|profileName|String|Name of the profile|
|profileDescription|String|Description of the profile|
|isDefaultProfile|Boolean|Boolean that represents whether the profile is used as default or not|
|createdDateTime|DateTimeOffset|Time when the BrandingProfile was created|
|lastModifiedDateTime|DateTimeOffset|Time when the BrandingProfile was last modified|
|displayName|String|Company/organization name that is displayed to end users|
|contactITName|String|Name of the person/organization responsible for IT support|
|contactITPhoneNumber|String|Phone number of the person/organization responsible for IT support|
|contactITEmailAddress|String|E-mail address of the person/organization responsible for IT support|
|contactITNotes|String|Text comments regarding the person/organization responsible for IT support|
|privacyUrl|String|URL to the company/organization’s privacy policy|
|onlineSupportSiteUrl|String|URL to the company/organization’s IT helpdesk site|
|onlineSupportSiteName|String|Display name of the company/organization’s IT helpdesk site|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Primary theme color used in the Company Portal applications and web portal|
|showLogo|Boolean|Boolean that represents whether the administrator-supplied logo images are shown or not|
|showDisplayNameNextToLogo|Boolean|Boolean that represents whether the administrator-supplied display name will be shown next to the logo image or not|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Logo image displayed in Company Portal apps which have a theme color background behind the logo|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Logo image displayed in Company Portal apps which have a light background behind the logo|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Customized image displayed in Company Portal apps landing page|
|customPrivacyMessage|String|Text comments regarding what the admin has access to on the device|
|isRemoveDeviceDisabled|Boolean|Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.|
|isFactoryResetDisabled|Boolean|Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) collection|The list of group assignments for the branding profile|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.intuneBrandingProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "String (identifier)",
  "profileName": "String",
  "profileDescription": "String",
  "isDefaultProfile": true,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "privacyUrl": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "customPrivacyMessage": "String",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true
}
```



