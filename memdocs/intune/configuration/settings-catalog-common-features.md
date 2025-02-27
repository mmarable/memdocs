---
# required metadata

title: Common tasks and features you can configure using settings catalog in Microsoft Intune
description: Use the settings catalog in Microsoft Intune and Endpoint Manager to configure common features. For example, you can create a Universal Print policy, configure Microsoft Edge and Google Chrome web browser, and use built in settings instead of plist files for macOS devices.
keywords:
author: MandiOhlinger
ms.author: mandia
manager: dougeby
ms.date: 06/21/2022
ms.topic: how-to
ms.service: microsoft-intune
ms.subservice: configuration
ms.localizationpriority: high
ms.technology:

# optional metadata

#ROBOTS:
#audience:

ms.reviewer: laarrizz, mikedano, beflamm
ms.suite: ems
search.appverid: MET150
#ms.tgt_pltfrm:
ms.custom: intune-azure
ms.collection: M365-identity-device-management
---

# Tasks you can complete using the Settings Catalog in Intune

Using the [settings catalog](settings-catalog.md) in the [Microsoft Endpoint Manager admin center](https://go.microsoft.com/fwlink/?linkid=2109431), you can access many settings that manage apps and features on your devices.

This article lists and describes some of the features you can configure in the settings catalog.

For more information on the settings catalog, and what it is, go to [Use the settings catalog to configure settings on Windows and macOS devices](settings-catalog.md). To see all the settings you can configure, create a settings catalog policy.

This feature applies to:

- iOS/iPadOS
- macOS
- Windows 11
- Windows 10

## Configure Microsoft Edge and Google Chrome

<!-- ms.reviewer: mikedano -->

This feature applies to:

- macOS
- Windows 11
- Windows 10

These web browser settings are built in, and can be configured & deployed to your managed devices. On Windows devices, you can also configure Google Chrome.

:::image type="content" source="./media/settings-catalog-common-features/google-chrome-settings.png" alt-text="In Settings Catalog, Google Chrome settings are built in to Microsoft Intune and Endpoint Manager admin center. Use these settings to create and configure a Google Chrome policy on Windows devices.":::

Previously, to configure Google Chrome settings on Windows devices, you created a custom OMA-URI device configuration policy.

## Add universal printers

<!-- ms.reviewer: laarrizz -->

This feature applies to:

- Windows 11

You can create a universal print policy, add printers, and then deploy this printer list to your managed users. When the policy is deployed, it automatically installs the printers you added. Users can see these printers, and select a printer from your list.

For more information, go to [Create a Universal Print policy in Microsoft Intune](settings-catalog-printer-provisioning.md).

Previously, to configure Universal Print settings, you used the [Universal Print printer provisioning tool](/universal-print/fundamentals/universal-print-intune-tool), which requires more manual steps, and has some limitations.

## Built-in macOS features replacing plist files

<!-- ms.reviewer: beflamm -->

This feature applies to:

- macOS

On macOS, you can use property list (plist) files to configure features and settings that aren't built in to Intune. Some of these feature settings are now available in the settings catalog:

- **Microsoft Edge version 77 and newer**: For a list of the settings you can configure, go to [Microsoft Edge - Policies](/DeployEdge/microsoft-edge-policies) (opens another Microsoft website).

  Previously, you had to [use a property list (plist) file to configure Microsoft Edge](/deployedge/configure-microsoft-edge-on-mac) (opens another Microsoft website).

- **Microsoft Defender for Endpoint**: For a list of the settings you can configure, go to [Set preferences for Microsoft Defender for Endpoint on macOS](/microsoft-365/security/defender-endpoint/mac-preferences) (opens another Microsoft website).

  Previously, you had to [use a property list (plist) file to configure Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/mac-install-with-intune) (opens another Microsoft website).

- **Microsoft Office and Microsoft Outlook**: For a list of the Microsoft Office and Outlook settings you can configure, go to:

  - [Use preferences to manage privacy controls for Office for Mac - Deploy Office](/deployoffice/privacy/mac-privacy-preferences)
  - [Set preferences for Outlook for Mac - Deploy Office](/deployoffice/mac/preferences-outlook)

  Previously, you had to [use a property list (plist) file to configure Office and Outlook for Mac](/deployoffice/mac/deploy-preferences-for-office-for-mac) (opens another Microsoft website).

Be sure macOS is listed as a supported platform. If some settings aren't available in the settings catalog, then it's recommended to continue using the [preference file](preference-file-settings-macos.md).

## Learn more

- [Use the settings catalog to configure settings on Windows and macOS devices](settings-catalog.md)
- [Create a Universal Print policy in Microsoft Intune](settings-catalog-printer-provisioning.md)
