---
title: "Update windows10GeneralConfiguration"
description: "Update the properties of a windows10GeneralConfiguration object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update windows10GeneralConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [windows10GeneralConfiguration](../resources/windows10generalconfiguration.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH ** Entity URI for microsoft.graph.windows10GeneralConfiguration not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [windows10GeneralConfiguration](../resources/windows10generalconfiguration.md) object.

The following table shows the properties that are required when you update the [windows10GeneralConfiguration](../resources/windows10generalconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/devicemanagementapplicabilityruledevicemode.md)|The device mode applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/devicemanagementapplicabilityruleosedition.md)|The OS edition applicability for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/devicemanagementapplicabilityruleosversion.md)|The OS version applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indicates whether or not the underlying Device Configuration supports the assignment of scope tags. Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users. This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal. This property is read-only. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|accountsBlockAddingNonMicrosoftAccountEmail|Boolean|Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.|
|activateAppsWithVoice|enablement|Specifies if Windows apps can be activated by voice. Possible values are: `notConfigured`, `enabled`, `disabled`.|
|antiTheftModeBlocked|Boolean|Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).|
|appManagementMSIAllowUserControlOverInstall|Boolean|This policy setting permits users to change installation options that typically are available only to system administrators.|
|appManagementMSIAlwaysInstallWithElevatedPrivileges|Boolean|This policy setting directs Windows Installer to use elevated permissions when it installs any program on the system.|
|appManagementPackageFamilyNamesToLaunchAfterLogOn|String collection|List of semi-colon delimited Package Family Names of Windows apps. Listed Windows apps are to be launched after logon.​|
|appsAllowTrustedAppsSideloading|stateManagementSetting|Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded. Possible values are: `notConfigured`, `blocked`, `allowed`.|
|appsBlockWindowsStoreOriginatedApps|Boolean|Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.|
|authenticationAllowSecondaryDevice|Boolean|Allows secondary authentication devices to work with Windows.|
|authenticationPreferredAzureADTenantDomainName|String|Specifies the preferred domain among available domains in the Azure AD tenant.|
|authenticationWebSignIn|enablement|Indicates whether or not Web Credential Provider will be enabled. Possible values are: `notConfigured`, `enabled`, `disabled`.|
|bluetoothAllowedServices|String collection|Specify a list of allowed Bluetooth services and profiles in hex formatted strings.|
|bluetoothBlockAdvertising|Boolean|Whether or not to Block the user from using bluetooth advertising.|
|bluetoothBlockDiscoverableMode|Boolean|Whether or not to Block the user from using bluetooth discoverable mode.|
|bluetoothBlocked|Boolean|Whether or not to Block the user from using bluetooth.|
|bluetoothBlockPrePairing|Boolean|Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.|
|bluetoothBlockPromptedProximalConnections|Boolean|Whether or not to block the users from using Swift Pair and other proximity based scenarios.|
|cameraBlocked|Boolean|Whether or not to Block the user from accessing the camera of the device.|
|cellularBlockDataWhenRoaming|Boolean|Whether or not to Block the user from using data over cellular while roaming.|
|cellularBlockVpn|Boolean|Whether or not to Block the user from using VPN over cellular.|
|cellularBlockVpnWhenRoaming|Boolean|Whether or not to Block the user from using VPN when roaming over cellular.|
|cellularData|configurationUsage|Whether or not to allow the cellular data channel on the device. If not configured, the cellular data channel is allowed and the user can turn it off. Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.|
|certificatesBlockManualRootCertificateInstallation|Boolean|Whether or not to Block the user from doing manual root certificate installation.|
|configureTimeZone|String|Specifies the time zone to be applied to the device. This is the standard Windows name for the target time zone.|
|connectedDevicesServiceBlocked|Boolean|Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.|
|copyPasteBlocked|Boolean|Whether or not to Block the user from using copy paste.|
|cortanaBlocked|Boolean|Whether or not to Block the user from using Cortana.|
|cryptographyAllowFipsAlgorithmPolicy|Boolean|Specify whether to allow or disallow the Federal Information Processing Standard (FIPS) policy.|
|dataProtectionBlockDirectMemoryAccess|Boolean|This policy setting allows you to block direct memory access (DMA) for all hot pluggable PCI downstream ports until a user logs into Windows.|
|defenderBlockEndUserAccess|Boolean|Whether or not to block end user access to Defender.|
|defenderBlockOnAccessProtection|Boolean|Allows or disallows Windows Defender On Access Protection functionality.|
|defenderCloudBlockLevel|defenderCloudBlockLevelType|Specifies the level of cloud-delivered protection. Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|defenderCloudExtendedTimeout|Int32|Timeout extension for file scanning by the cloud. Valid values 0 to 50|
|defenderCloudExtendedTimeoutInSeconds|Int32|Timeout extension for file scanning by the cloud. Valid values 0 to 50|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Number of days before deleting quarantined malware. Valid values 0 to 90|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/defenderdetectedmalwareactions.md)|Gets or sets Defender’s actions to take on detected Malware per threat level.|
|defenderDisableCatchupFullScan|Boolean|When blocked, catch-up scans for scheduled full scans will be turned off.|
|defenderDisableCatchupQuickScan|Boolean|When blocked, catch-up scans for scheduled quick scans will be turned off.|
|defenderFileExtensionsToExclude|String collection|File extensions to exclude from scans and real time protection.|
|defenderFilesAndFoldersToExclude|String collection|Files and folder to exclude from scans and real time protection.|
|defenderMonitorFileActivity|defenderMonitorFileActivity|Value for monitoring file activity. Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|defenderPotentiallyUnwantedAppAction|defenderPotentiallyUnwantedAppAction|Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself. Added in Windows 10 for desktop. Possible values are: `deviceDefault`, `block`, `audit`.|
|defenderPotentiallyUnwantedAppActionSetting|defenderProtectionType|Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself. Added in Windows 10 for desktop. Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.|
|defenderProcessesToExclude|String collection|Processes to exclude from scans and real time protection.|
|defenderPromptForSampleSubmission|defenderPromptForSampleSubmission|The configuration for how to prompt user for sample submission. Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.|
|defenderRequireBehaviorMonitoring|Boolean|Indicates whether or not to require behavior monitoring.|
|defenderRequireCloudProtection|Boolean|Indicates whether or not to require cloud protection.|
|defenderRequireNetworkInspectionSystem|Boolean|Indicates whether or not to require network inspection system.|
|defenderRequireRealTimeMonitoring|Boolean|Indicates whether or not to require real time monitoring.|
|defenderScanArchiveFiles|Boolean|Indicates whether or not to scan archive files.|
|defenderScanDownloads|Boolean|Indicates whether or not to scan downloads.|
|defenderScanIncomingMail|Boolean|Indicates whether or not to scan incoming mail messages.|
|defenderScanMappedNetworkDrivesDuringFullScan|Boolean|Indicates whether or not to scan mapped network drives during full scan.|
|defenderScanMaxCpu|Int32|Max CPU usage percentage during scan. Valid values 0 to 100|
|defenderScanNetworkFiles|Boolean|Indicates whether or not to scan files opened from a network folder.|
|defenderScanRemovableDrivesDuringFullScan|Boolean|Indicates whether or not to scan removable drives during full scan.|
|defenderScanScriptsLoadedInInternetExplorer|Boolean|Indicates whether or not to scan scripts loaded in Internet Explorer browser.|
|defenderScanType|defenderScanType|The defender system scan type. Possible values are: `userDefined`, `disabled`, `quick`, `full`.|
|defenderScheduledQuickScanTime|TimeOfDay|The time to perform a daily quick scan.|
|defenderScheduledScanTime|TimeOfDay|The defender time for the system scan.|
|defenderScheduleScanEnableLowCpuPriority|Boolean|When enabled, low CPU priority will be used during scheduled scans.|
|defenderSignatureUpdateIntervalInHours|Int32|The signature update interval in hours. Specify 0 not to check. Valid values 0 to 24|
|defenderSubmitSamplesConsentType|defenderSubmitSamplesConsentType|Checks for the user consent level in Windows Defender to send data. Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.|
|defenderSystemScanSchedule|weeklySchedule|Defender day of the week for the system scan. Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.|
|developerUnlockSetting|stateManagementSetting|Indicates whether or not to allow developer unlock. Possible values are: `notConfigured`, `blocked`, `allowed`.|
|deviceManagementBlockFactoryResetOnMobile|Boolean|Indicates whether or not to Block the user from resetting their phone.|
|deviceManagementBlockManualUnenroll|Boolean|Indicates whether or not to Block the user from doing manual un-enrollment from device management.|
|diagnosticsDataSubmissionMode|diagnosticDataSubmissionMode|Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson. Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.|
|displayAppListWithGdiDPIScalingTurnedOff|String collection|List of legacy applications that have GDI DPI Scaling turned off.|
|displayAppListWithGdiDPIScalingTurnedOn|String collection|List of legacy applications that have GDI DPI Scaling turned on.|
|edgeAllowStartPagesModification|Boolean|Allow users to change Start pages on Edge. Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.|
|edgeBlockAccessToAboutFlags|Boolean|Indicates whether or not to prevent access to about flags on Edge browser.|
|edgeBlockAddressBarDropdown|Boolean|Block the address bar dropdown functionality in Microsoft Edge. Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.|
|edgeBlockAutofill|Boolean|Indicates whether or not to block auto fill.|
|edgeBlockCompatibilityList|Boolean|Block Microsoft compatibility list in Microsoft Edge. This list from Microsoft helps Edge properly display sites with known compatibility issues.|
|edgeBlockDeveloperTools|Boolean|Indicates whether or not to block developer tools in the Edge browser.|
|edgeBlocked|Boolean|Indicates whether or not to Block the user from using the Edge browser.|
|edgeBlockEditFavorites|Boolean|Indicates whether or not to Block the user from making changes to Favorites.|
|edgeBlockExtensions|Boolean|Indicates whether or not to block extensions in the Edge browser.|
|edgeBlockFullScreenMode|Boolean|Allow or prevent Edge from entering the full screen mode.|
|edgeBlockInPrivateBrowsing|Boolean|Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.|
|edgeBlockJavaScript|Boolean|Indicates whether or not to Block the user from using JavaScript.|
|edgeBlockLiveTileDataCollection|Boolean|Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.|
|edgeBlockPasswordManager|Boolean|Indicates whether or not to Block password manager.|
|edgeBlockPopups|Boolean|Indicates whether or not to block popups.|
|edgeBlockPrelaunch|Boolean|Decide whether Microsoft Edge is prelaunched at Windows startup.|
|edgeBlockPrinting|Boolean|Configure Edge to allow or block printing.|
|edgeBlockSavingHistory|Boolean|Configure Edge to allow browsing history to be saved or to never save browsing history.|
|edgeBlockSearchEngineCustomization|Boolean|Indicates whether or not to block the user from adding new search engine or changing the default search engine.|
|edgeBlockSearchSuggestions|Boolean|Indicates whether or not to block the user from using the search suggestions in the address bar.|
|edgeBlockSendingDoNotTrackHeader|Boolean|Indicates whether or not to Block the user from sending the do not track header.|
|edgeBlockSendingIntranetTrafficToInternetExplorer|Boolean|Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer. Note: the name of this property is misleading; the property is obsolete, use EdgeSendIntranetTrafficToInternetExplorer instead.|
|edgeBlockSideloadingExtensions|Boolean|Indicates whether the user can sideload extensions.|
|edgeBlockTabPreloading|Boolean|Configure whether Edge preloads the new tab page at Windows startup.|
|edgeBlockWebContentOnNewTabPage|Boolean|Configure to load a blank page in Edge instead of the default New tab page and prevent users from changing it.|
|edgeClearBrowsingDataOnExit|Boolean|Clear browsing data on exiting Microsoft Edge.|
|edgeCookiePolicy|edgeCookiePolicy|Indicates which cookies to block in the Edge browser. Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.|
|edgeDisableFirstRunPage|Boolean|Block the Microsoft web page that opens on the first use of Microsoft Edge. This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.|
|edgeEnterpriseModeSiteListLocation|String|Indicates the enterprise mode site list location. Could be a local file, local network or http location.|
|edgeFavoritesBarVisibility|visibilitySetting|Get or set a value that specifies whether to set the favorites bar to always be visible or hidden on any page. Possible values are: `notConfigured`, `hide`, `show`.|
|edgeFavoritesListLocation|String|The location of the favorites list to provision. Could be a local file, local network or http location.|
|edgeFirstRunUrl|String|The first run URL for when Edge browser is opened for the first time.|
|edgeHomeButtonConfiguration|[edgeHomeButtonConfiguration](../resources/edgehomebuttonconfiguration.md)|Causes the Home button to either hide, load the default Start page, load a New tab page, or a custom URL|
|edgeHomeButtonConfigurationEnabled|Boolean|Enable the Home button configuration.|
|edgeHomepageUrls|String collection|The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.|
|edgeKioskModeRestriction|edgeKioskModeRestrictionType|Controls how the Microsoft Edge settings are restricted based on the configure kiosk mode. Possible values are: `notConfigured`, `digitalSignage`, `normalMode`, `publicBrowsingSingleApp`, `publicBrowsingMultiApp`.|
|edgeKioskResetAfterIdleTimeInMinutes|Int32|Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets. Valid values are 0-1440. The default is 5. 0 indicates no reset. Valid values 0 to 1440|
|edgeNewTabPageURL|String|Specify the page opened when new tabs are created.|
|edgeOpensWith|edgeOpenOptions|Specify what kind of pages are open at start. Possible values are: `notConfigured`, `startPage`, `newTabPage`, `previousPages`, `specificPages`.|
|edgePreventCertificateErrorOverride|Boolean|Allow or prevent users from overriding certificate errors.|
|edgeRequiredExtensionPackageFamilyNames|String collection|Specify the list of package family names of browser extensions that are required and cannot be turned off by the user.|
|edgeRequireSmartScreen|Boolean|Indicates whether or not to Require the user to use the smart screen filter.|
|edgeSearchEngine|[edgeSearchEngineBase](../resources/edgesearchenginebase.md)|Allows IT admins to set a default search engine for MDM-Controlled devices. Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.|
|edgeSendIntranetTrafficToInternetExplorer|Boolean|Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.|
|edgeShowMessageWhenOpeningInternetExplorerSites|internetExplorerMessageSetting|Controls the message displayed by Edge before switching to Internet Explorer. Possible values are: `notConfigured`, `disabled`, `enabled`, `keepGoing`.|
|edgeSyncFavoritesWithInternetExplorer|Boolean|Enable favorites sync between Internet Explorer and Microsoft Edge. Additions, deletions, modifications and order changes to favorites are shared between browsers.|
|edgeTelemetryForMicrosoft365Analytics|edgeTelemetryMode|Specifies what type of telemetry data (none, intranet, internet, both) is sent to Microsoft 365 Analytics. Possible values are: `notConfigured`, `intranet`, `internet`, `intranetAndInternet`.|
|enableAutomaticRedeployment|Boolean|Allow users with administrative rights to delete all user data and settings using CTRL + Win + R at the device lock screen so that the device can be automatically re-configured and re-enrolled into management.|
|energySaverOnBatteryThresholdPercentage|Int32|This setting allows you to specify battery charge level at which Energy Saver is turned on. While on battery, Energy Saver is automatically turned on at (and below) the specified battery charge level. Valid input range (0-100). Valid values 0 to 100|
|energySaverPluggedInThresholdPercentage|Int32|This setting allows you to specify battery charge level at which Energy Saver is turned on. While plugged in, Energy Saver is automatically turned on at (and below) the specified battery charge level. Valid input range (0-100). Valid values 0 to 100|
|enterpriseCloudPrintDiscoveryEndPoint|String|Endpoint for discovering cloud printers.|
|enterpriseCloudPrintDiscoveryMaxLimit|Int32|Maximum number of printers that should be queried from a discovery endpoint. This is a mobile only setting. Valid values 1 to 65535|
|enterpriseCloudPrintMopriaDiscoveryResourceIdentifier|String|OAuth resource URI for printer discovery service as configured in Azure portal.|
|enterpriseCloudPrintOAuthAuthority|String|Authentication endpoint for acquiring OAuth tokens.|
|enterpriseCloudPrintOAuthClientIdentifier|String|GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.|
|enterpriseCloudPrintResourceIdentifier|String|OAuth resource URI for print service as configured in the Azure portal.|
|experienceBlockDeviceDiscovery|Boolean|Indicates whether or not to enable device discovery UX.|
|experienceBlockErrorDialogWhenNoSIM|Boolean|Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.|
|experienceBlockTaskSwitcher|Boolean|Indicates whether or not to enable task switching on the device.|
|experienceDoNotSyncBrowserSettings|browserSyncSetting|Allow or prevent the syncing of Microsoft Edge Browser settings. Option for IT admins to prevent syncing across devices, but allow user override. Possible values are: `notConfigured`, `blockedWithUserOverride`, `blocked`.|
|findMyFiles|enablement|Controls if the user can configure search to Find My Files mode, which searches files in secondary hard drives and also outside of the user profile. Find My Files does not allow users to search files or locations to which they do not have access. Possible values are: `notConfigured`, `enabled`, `disabled`.|
|gameDvrBlocked|Boolean|Indicates whether or not to block DVR and broadcasting.|
|inkWorkspaceAccess|inkAccessSetting|Controls the user access to the ink workspace, from the desktop and from above the lock screen. Possible values are: `notConfigured`, `enabled`, `disabled`.|
|inkWorkspaceAccessState|stateManagementSetting|Controls the user access to the ink workspace, from the desktop and from above the lock screen. Possible values are: `notConfigured`, `blocked`, `allowed`.|
|inkWorkspaceBlockSuggestedApps|Boolean|Specify whether to show recommended app suggestions in the ink workspace.|
|internetSharingBlocked|Boolean|Indicates whether or not to Block the user from using internet sharing.|
|locationServicesBlocked|Boolean|Indicates whether or not to Block the user from location services.|
|lockScreenActivateAppsWithVoice|enablement|This policy setting specifies whether Windows apps can be activated by voice while the system is locked. Possible values are: `notConfigured`, `enabled`, `disabled`.|
|lockScreenAllowTimeoutConfiguration|Boolean|Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices. If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.|
|lockScreenBlockActionCenterNotifications|Boolean|Indicates whether or not to block action center notifications over lock screen.|
|lockScreenBlockCortana|Boolean|Indicates whether or not the user can interact with Cortana using speech while the system is locked.|
|lockScreenBlockToastNotifications|Boolean|Indicates whether to allow toast notifications above the device lock screen.|
|lockScreenTimeoutInSeconds|Int32|Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices. Supported values are 11-1800. Valid values 11 to 1800|
|logonBlockFastUserSwitching|Boolean|Disables the ability to quickly switch between users that are logged on simultaneously without logging off.|
|messagingBlockMMS|Boolean|Indicates whether or not to block the MMS send/receive functionality on the device.|
|messagingBlockRichCommunicationServices|Boolean|Indicates whether or not to block the RCS send/receive functionality on the device.|
|messagingBlockSync|Boolean|Indicates whether or not to block text message back up and restore and Messaging Everywhere.|
|microsoftAccountBlocked|Boolean|Indicates whether or not to Block a Microsoft account.|
|microsoftAccountBlockSettingsSync|Boolean|Indicates whether or not to Block Microsoft account settings sync.|
|microsoftAccountSignInAssistantSettings|signInAssistantOptions|Controls the Microsoft Account Sign-In Assistant (wlidsvc) NT service. Possible values are: `notConfigured`, `disabled`.|
|networkProxyApplySettingsDeviceWide|Boolean|If set, proxy settings will be applied to all processes and accounts in the device. Otherwise, it will be applied to the user account that’s enrolled into MDM.|
|networkProxyAutomaticConfigurationUrl|String|Address to the proxy auto-config (PAC) script you want to use.|
|networkProxyDisableAutoDetect|Boolean|Disable automatic detection of settings. If enabled, the system will try to find the path to a proxy auto-config (PAC) script.|
|networkProxyServer|[windows10NetworkProxyServer](../resources/windows10networkproxyserver.md)|Specifies manual proxy server settings.|
|nfcBlocked|Boolean|Indicates whether or not to Block the user from using near field communication.|
|oneDriveDisableFileSync|Boolean|Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.|
|passwordBlockSimple|Boolean|Specify whether PINs or passwords suc ktops, it also controls the use of picture passwords.|
|passwordExpirationDays|Int32|The password expiration in days. Valid values 0 to 730|
|passwordMinimumAgeInDays|Int32|This security setting determines the period of time (in days) that a password must be used before the user can change it. Valid values 0 to 998|
|passwordMinimumCharacterSetCount|Int32|The number of character sets required in the password.|
|passwordMinimumLength|Int32|The minimum password length. Valid values 4 to 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|The minutes of inactivity before the screen times out.|
|passwordPreviousPasswordBlockCount|Int32|The number of previous passwords to prevent reuse of. Valid values 0 to 50|
|passwordRequired|Boolean|Indicates whether or not to require the user to have a password.|
|passwordRequiredType|requiredPasswordType|The required password type. Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordRequireWhenResumeFromIdleState|Boolean|Indicates whether or not to require a password upon resuming from an idle state.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|The number of sign in failures before factory reset. Valid values 0 to 999|
|personalizationDesktopImageUrl|String|A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.|
|personalizationLockScreenImageUrl|String|A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.|
|powerButtonActionOnBattery|powerActionType|This setting specifies the action that Windows takes when a user presses the Power button while on battery. Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerButtonActionPluggedIn|powerActionType|This setting specifies the action that Windows takes when a user presses the Power button while plugged in. Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerHybridSleepOnBattery|enablement|This setting allows you to turn off hybrid sleep while on battery. If you set this setting to disable, a hiberfile is not generated when the system transitions to sleep (Stand By). If you set this setting to enable or do not configure this policy setting, users control this setting. Possible values are: `notConfigured`, `enabled`, `disabled`.|
|powerHybridSleepPluggedIn|enablement|This setting allows you to turn off hybrid sleep while plugged in. If you set this setting to disable, a hiberfile is not generated when the system transitions to sleep (Stand By). If you set this setting to enable or do not configure this policy setting, users control this setting. Possible values are: `notConfigured`, `enabled`, `disabled`.|
|powerLidCloseActionOnBattery|powerActionType|This setting specifies the action that Windows takes when a user closes the lid on a mobile PC while on battery. Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerLidCloseActionPluggedIn|powerActionType|This setting specifies the action that Windows takes when a user closes the lid on a mobile PC while plugged in. Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerSleepButtonActionOnBattery|powerActionType|This setting specifies the action that Windows takes when a user presses the Sleep button while on battery. Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|powerSleepButtonActionPluggedIn|powerActionType|This setting specifies the action that Windows takes when a user presses the Sleep button while plugged in. Possible values are: `notConfigured`, `noAction`, `sleep`, `hibernate`, `shutdown`.|
|printerBlockAddition|Boolean|Prevent user installation of additional printers from printers settings.|
|printerDefaultName|String|Name (network host name) of an installed printer.|
|printerNames|String collection|Automatically provision printers based on their names (network host names).|
|privacyAdvertisingId|stateManagementSetting|Enables or disables the use of advertising ID. Added in Windows 10, version 1607. Possible values are: `notConfigured`, `blocked`, `allowed`.|
|privacyAutoAcceptPairingAndConsentPrompts|Boolean|Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.|
|privacyBlockActivityFeed|Boolean|Blocks the usage of cloud based speech services for Cortana, Dictation, or Store applications.|
|privacyBlockInputPersonalization|Boolean|Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.|
|privacyBlockPublishUserActivities|Boolean|Blocks the shared experiences/discovery of recently used resources in task switcher etc.|
|privacyDisableLaunchExperience|Boolean|This policy prevents the privacy experience from launching during user logon for new and upgraded users.​|
|resetProtectionModeBlocked|Boolean|Indicates whether or not to Block the user from reset protection mode.|
|safeSearchFilter|safeSearchFilterType|Specifies what filter level of safe search is required. Possible values are: `userDefined`, `strict`, `moderate`.|
|screenCaptureBlocked|Boolean|Indicates whether or not to Block the user from taking Screenshots.|
|searchBlockDiacritics|Boolean|Specifies if search can use diacritics.|
|searchBlockWebResults|Boolean|Indicates whether or not to block the web search.|
|searchDisableAutoLanguageDetection|Boolean|Specifies whether to use automatic language detection when indexing content and properties.|
|searchDisableIndexerBackoff|Boolean|Indicates whether or not to disable the search indexer backoff feature.|
|searchDisableIndexingEncryptedItems|Boolean|Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.|
|searchDisableIndexingRemovableDrive|Boolean|Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.|
|searchDisableLocation|Boolean|Specifies if search can use location information.|
|searchDisableUseLocation|Boolean|Specifies if search can use location information.|
|searchEnableAutomaticIndexSizeManangement|Boolean|Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.|
|searchEnableRemoteQueries|Boolean|Indicates whether or not to block remote queries of this computer’s index.|
|securityBlockAzureADJoinedDevicesAutoEncryption|Boolean|Specify whether to allow automatic device encryption during OOBE when the device is Azure AD joined (desktop only).|
|settingsBlockAccountsPage|Boolean|Indicates whether or not to block access to Accounts in Settings app.|
|settingsBlockAddProvisioningPackage|Boolean|Indicates whether or not to block the user from installing provisioning packages.|
|settingsBlockAppsPage|Boolean|Indicates whether or not to block access to Apps in Settings app.|
|settingsBlockChangeLanguage|Boolean|Indicates whether or not to block the user from changing the language settings.|
|settingsBlockChangePowerSleep|Boolean|Indicates whether or not to block the user from changing power and sleep settings.|
|settingsBlockChangeRegion|Boolean|Indicates whether or not to block the user from changing the region settings.|
|settingsBlockChangeSystemTime|Boolean|Indicates whether or not to block the user from changing date and time settings.|
|settingsBlockDevicesPage|Boolean|Indicates whether or not to block access to Devices in Settings app.|
|settingsBlockEaseOfAccessPage|Boolean|Indicates whether or not to block access to Ease of Access in Settings app.|
|settingsBlockEditDeviceName|Boolean|Indicates whether or not to block the user from editing the device name.|
|settingsBlockGamingPage|Boolean|Indicates whether or not to block access to Gaming in Settings app.|
|settingsBlockNetworkInternetPage|Boolean|Indicates whether or not to block access to Network and Internet in Settings app.|
|settingsBlockPersonalizationPage|Boolean|Indicates whether or not to block access to Personalization in Settings app.|
|settingsBlockPrivacyPage|Boolean|Indicates whether or not to block access to Privacy in Settings app.|
|settingsBlockRemoveProvisioningPackage|Boolean|Indicates whether or not to block the runtime configuration agent from removing provisioning packages.|
|settingsBlockSettingsApp|Boolean|Indicates whether or not to block access to Settings app.|
|settingsBlockSystemPage|Boolean|Indicates whether or not to block access to System in Settings app.|
|settingsBlockTimeLanguagePage|Boolean|Indicates whether or not to block access to Time and Language in Settings app.|
|settingsBlockUpdateSecurityPage|Boolean|Indicates whether or not to block access to Update and Security in Settings app.|
|sharedUserAppDataAllowed|Boolean|Indicates whether or not to block multiple users of the same app to share data.|
|smartScreenAppInstallControl|appInstallControlType|Added in Windows 10, version 1703. Allows IT Admins to control whether users are allowed to install apps from places other than the Store. Possible values are: `notConfigured`, `anywhere`, `storeOnly`, `recommendations`, `preferStore`.|
|smartScreenBlockPromptOverride|Boolean|Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.|
|smartScreenBlockPromptOverrideForFiles|Boolean|Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files|
|smartScreenEnableAppInstallControl|Boolean|This property will be deprecated in July 2019 and will be replaced by property SmartScreenAppInstallControl. Allows IT Admins to control whether users are allowed to install apps from places other than the Store.|
|startBlockUnpinningAppsFromTaskbar|Boolean|Indicates whether or not to block the user from unpinning apps from taskbar.|
|startMenuAppListVisibility|windowsStartMenuAppListVisibilityType|Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app. Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.|
|startMenuHideChangeAccountSettings|Boolean|Enabling this policy hides the change account setting from appearing in the user tile in the start menu.|
|startMenuHideFrequentlyUsedApps|Boolean|Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.|
|startMenuHideHibernate|Boolean|Enabling this policy hides hibernate from appearing in the power button in the start menu.|
|startMenuHideLock|Boolean|Enabling this policy hides lock from appearing in the user tile in the start menu.|
|startMenuHidePowerButton|Boolean|Enabling this policy hides the power button from appearing in the start menu.|
|startMenuHideRecentJumpLists|Boolean|Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.|
|startMenuHideRecentlyAddedApps|Boolean|Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.|
|startMenuHideRestartOptions|Boolean|Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.|
|startMenuHideShutDown|Boolean|Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.|
|startMenuHideSignOut|Boolean|Enabling this policy hides sign out from appearing in the user tile in the start menu.|
|startMenuHideSleep|Boolean|Enabling this policy hides sleep from appearing in the power button in the start menu.|
|startMenuHideSwitchAccount|Boolean|Enabling this policy hides switch account from appearing in the user tile in the start menu.|
|startMenuHideUserTile|Boolean|Enabling this policy hides the user tile from appearing in the start menu.|
|startMenuLayoutEdgeAssetsXml|Binary|This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy. Start layout can contain secondary tile from Edge app which looks for Edge local asset file. Edge local asset would not exist and cause Edge secondary tile to appear empty in this case. This policy only gets applied when startMenuLayoutXml policy is modified. The value should be a UTF-8 Base64 encoded byte array.|
|startMenuLayoutXml|Binary|Allows admins to override the default Start menu layout and prevents the user from changing it. The layout is modified by specifying an XML file based on a layout modification schema. XML needs to be in a UTF8 encoded byte array format.|
|startMenuMode|windowsStartMenuModeType|Allows admins to decide how the Start menu is displayed. Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.|
|startMenuPinnedFolderDocuments|visibilitySetting|Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderDownloads|visibilitySetting|Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderFileExplorer|visibilitySetting|Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderHomeGroup|visibilitySetting|Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderMusic|visibilitySetting|Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderNetwork|visibilitySetting|Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPersonalFolder|visibilitySetting|Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderPictures|visibilitySetting|Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderSettings|visibilitySetting|Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|startMenuPinnedFolderVideos|visibilitySetting|Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu. Possible values are: `notConfigured`, `hide`, `show`.|
|storageBlockRemovableStorage|Boolean|Indicates whether or not to Block the user from using removable storage.|
|storageRequireMobileDeviceEncryption|Boolean|Indicating whether or not to require encryption on a mobile device.|
|storageRestrictAppDataToSystemVolume|Boolean|Indicates whether application data is restricted to the system drive.|
|storageRestrictAppInstallToSystemVolume|Boolean|Indicates whether the installation of applications is restricted to the system drive.|
|systemTelemetryProxyServer|String|Gets or sets the fully qualified domain name (FQDN) or IP address of a proxy server to forward Connected User Experiences and Telemetry requests.|
|taskManagerBlockEndTask|Boolean|Specify whether non-administrators can use Task Manager to end tasks.|
|tenantLockdownRequireNetworkDuringOutOfBoxExperience|Boolean|Whether the device is required to connect to the network.|
|uninstallBuiltInApps|Boolean|Indicates whether or not to uninstall a fixed list of built-in Windows apps.|
|usbBlocked|Boolean|Indicates whether or not to Block the user from USB connection.|
|voiceRecordingBlocked|Boolean|Indicates whether or not to Block the user from voice recording.|
|webRtcBlockLocalhostIpAddress|Boolean|Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC|
|wiFiBlockAutomaticConnectHotspots|Boolean|Indicating whether or not to block automatically connecting to Wi-Fi hotspots. Has no impact if Wi-Fi is blocked.|
|wiFiBlocked|Boolean|Indicates whether or not to Block the user from using Wi-Fi.|
|wiFiBlockManualConfiguration|Boolean|Indicates whether or not to Block the user from using Wi-Fi manual configuration.|
|wiFiScanInterval|Int32|Specify how often devices scan for Wi-Fi networks. Supported values are 1-500, where 100 = default, and 500 = low frequency. Valid values 1 to 500|
|windows10AppsForceUpdateSchedule|[windows10AppsForceUpdateSchedule](../resources/windows10appsforceupdateschedule.md)|Windows 10 force update schedule for Apps.|
|windowsSpotlightBlockConsumerSpecificFeatures|Boolean|Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.|
|windowsSpotlightBlocked|Boolean|Allows IT admins to turn off all Windows Spotlight features|
|windowsSpotlightBlockOnActionCenter|Boolean|Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed|
|windowsSpotlightBlockTailoredExperiences|Boolean|Block personalized content in Windows spotlight based on user’s device usage.|
|windowsSpotlightBlockThirdPartyNotifications|Boolean|Block third party content delivered via Windows Spotlight|
|windowsSpotlightBlockWelcomeExperience|Boolean|Block Windows Spotlight Windows welcome experience|
|windowsSpotlightBlockWindowsTips|Boolean|Allows IT admins to turn off the popup of Windows Tips.|
|windowsSpotlightConfigureOnLockScreen|windowsSpotlightEnablementSettings|Specifies the type of Spotlight. Possible values are: `notConfigured`, `disabled`, `enabled`.|
|windowsStoreBlockAutoUpdate|Boolean|Indicates whether or not to block automatic update of apps from Windows Store.|
|windowsStoreBlocked|Boolean|Indicates whether or not to Block the user from using the Windows store.|
|windowsStoreEnablePrivateStoreOnly|Boolean|Indicates whether or not to enable Private Store Only.|
|wirelessDisplayBlockProjectionToThisDevice|Boolean|Indicates whether or not to allow other devices from discovering this PC for projection.|
|wirelessDisplayBlockUserInputFromReceiver|Boolean|Indicates whether or not to allow user input from wireless display receiver.|
|wirelessDisplayRequirePinForPairing|Boolean|Indicates whether or not to require a PIN for new devices to initiate pairing.|



## Response

If successful, this method returns a `200 OK` response code and an updated [windows10GeneralConfiguration](../resources/windows10generalconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_windows10generalconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta** Entity URI for microsoft.graph.windows10GeneralConfiguration not found
Content-Type: application/json
Content-length: 14199

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "description": "String",
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode"
  },
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
  },
  "displayName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": "Boolean",
  "version": "Integer",
  "accountsBlockAddingNonMicrosoftAccountEmail": "Boolean",
  "activateAppsWithVoice": "String",
  "antiTheftModeBlocked": "Boolean",
  "appManagementMSIAllowUserControlOverInstall": "Boolean",
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": "Boolean",
  "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
    "String"
  ],
  "appsAllowTrustedAppsSideloading": "String",
  "appsBlockWindowsStoreOriginatedApps": "Boolean",
  "authenticationAllowSecondaryDevice": "Boolean",
  "authenticationPreferredAzureADTenantDomainName": "String",
  "authenticationWebSignIn": "String",
  "bluetoothAllowedServices": [
    "String"
  ],
  "bluetoothBlockAdvertising": "Boolean",
  "bluetoothBlockDiscoverableMode": "Boolean",
  "bluetoothBlocked": "Boolean",
  "bluetoothBlockPrePairing": "Boolean",
  "bluetoothBlockPromptedProximalConnections": "Boolean",
  "cameraBlocked": "Boolean",
  "cellularBlockDataWhenRoaming": "Boolean",
  "cellularBlockVpn": "Boolean",
  "cellularBlockVpnWhenRoaming": "Boolean",
  "cellularData": "String",
  "certificatesBlockManualRootCertificateInstallation": "Boolean",
  "configureTimeZone": "String",
  "connectedDevicesServiceBlocked": "Boolean",
  "copyPasteBlocked": "Boolean",
  "cortanaBlocked": "Boolean",
  "cryptographyAllowFipsAlgorithmPolicy": "Boolean",
  "dataProtectionBlockDirectMemoryAccess": "Boolean",
  "defenderBlockEndUserAccess": "Boolean",
  "defenderBlockOnAccessProtection": "Boolean",
  "defenderCloudBlockLevel": "String",
  "defenderCloudExtendedTimeout": "Integer",
  "defenderCloudExtendedTimeoutInSeconds": "Integer",
  "defenderDaysBeforeDeletingQuarantinedMalware": "Integer",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions"
  },
  "defenderDisableCatchupFullScan": "Boolean",
  "defenderDisableCatchupQuickScan": "Boolean",
  "defenderFileExtensionsToExclude": [
    "String"
  ],
  "defenderFilesAndFoldersToExclude": [
    "String"
  ],
  "defenderMonitorFileActivity": "String",
  "defenderPotentiallyUnwantedAppAction": "String",
  "defenderPotentiallyUnwantedAppActionSetting": "String",
  "defenderProcessesToExclude": [
    "String"
  ],
  "defenderPromptForSampleSubmission": "String",
  "defenderRequireBehaviorMonitoring": "Boolean",
  "defenderRequireCloudProtection": "Boolean",
  "defenderRequireNetworkInspectionSystem": "Boolean",
  "defenderRequireRealTimeMonitoring": "Boolean",
  "defenderScanArchiveFiles": "Boolean",
  "defenderScanDownloads": "Boolean",
  "defenderScanIncomingMail": "Boolean",
  "defenderScanMappedNetworkDrivesDuringFullScan": "Boolean",
  "defenderScanMaxCpu": "Integer",
  "defenderScanNetworkFiles": "Boolean",
  "defenderScanRemovableDrivesDuringFullScan": "Boolean",
  "defenderScanScriptsLoadedInInternetExplorer": "Boolean",
  "defenderScanType": "String",
  "defenderScheduledQuickScanTime": "String (time of day)",
  "defenderScheduledScanTime": "String (time of day)",
  "defenderScheduleScanEnableLowCpuPriority": "Boolean",
  "defenderSignatureUpdateIntervalInHours": "Integer",
  "defenderSubmitSamplesConsentType": "String",
  "defenderSystemScanSchedule": "String",
  "developerUnlockSetting": "String",
  "deviceManagementBlockFactoryResetOnMobile": "Boolean",
  "deviceManagementBlockManualUnenroll": "Boolean",
  "diagnosticsDataSubmissionMode": "String",
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "String"
  ],
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "String"
  ],
  "edgeAllowStartPagesModification": "Boolean",
  "edgeBlockAccessToAboutFlags": "Boolean",
  "edgeBlockAddressBarDropdown": "Boolean",
  "edgeBlockAutofill": "Boolean",
  "edgeBlockCompatibilityList": "Boolean",
  "edgeBlockDeveloperTools": "Boolean",
  "edgeBlocked": "Boolean",
  "edgeBlockEditFavorites": "Boolean",
  "edgeBlockExtensions": "Boolean",
  "edgeBlockFullScreenMode": "Boolean",
  "edgeBlockInPrivateBrowsing": "Boolean",
  "edgeBlockJavaScript": "Boolean",
  "edgeBlockLiveTileDataCollection": "Boolean",
  "edgeBlockPasswordManager": "Boolean",
  "edgeBlockPopups": "Boolean",
  "edgeBlockPrelaunch": "Boolean",
  "edgeBlockPrinting": "Boolean",
  "edgeBlockSavingHistory": "Boolean",
  "edgeBlockSearchEngineCustomization": "Boolean",
  "edgeBlockSearchSuggestions": "Boolean",
  "edgeBlockSendingDoNotTrackHeader": "Boolean",
  "edgeBlockSendingIntranetTrafficToInternetExplorer": "Boolean",
  "edgeBlockSideloadingExtensions": "Boolean",
  "edgeBlockTabPreloading": "Boolean",
  "edgeBlockWebContentOnNewTabPage": "Boolean",
  "edgeClearBrowsingDataOnExit": "Boolean",
  "edgeCookiePolicy": "String",
  "edgeDisableFirstRunPage": "Boolean",
  "edgeEnterpriseModeSiteListLocation": "String",
  "edgeFavoritesBarVisibility": "String",
  "edgeFavoritesListLocation": "String",
  "edgeFirstRunUrl": "String",
  "edgeHomeButtonConfiguration": {
    "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
  },
  "edgeHomeButtonConfigurationEnabled": "Boolean",
  "edgeHomepageUrls": [
    "String"
  ],
  "edgeKioskModeRestriction": "String",
  "edgeKioskResetAfterIdleTimeInMinutes": "Integer",
  "edgeNewTabPageURL": "String",
  "edgeOpensWith": "String",
  "edgePreventCertificateErrorOverride": "Boolean",
  "edgeRequiredExtensionPackageFamilyNames": [
    "String"
  ],
  "edgeRequireSmartScreen": "Boolean",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeSendIntranetTrafficToInternetExplorer": "Boolean",
  "edgeShowMessageWhenOpeningInternetExplorerSites": "String",
  "edgeSyncFavoritesWithInternetExplorer": "Boolean",
  "edgeTelemetryForMicrosoft365Analytics": "String",
  "enableAutomaticRedeployment": "Boolean",
  "energySaverOnBatteryThresholdPercentage": "Integer",
  "energySaverPluggedInThresholdPercentage": "Integer",
  "enterpriseCloudPrintDiscoveryEndPoint": "String",
  "enterpriseCloudPrintDiscoveryMaxLimit": "Integer",
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "String",
  "enterpriseCloudPrintOAuthAuthority": "String",
  "enterpriseCloudPrintOAuthClientIdentifier": "String",
  "enterpriseCloudPrintResourceIdentifier": "String",
  "experienceBlockDeviceDiscovery": "Boolean",
  "experienceBlockErrorDialogWhenNoSIM": "Boolean",
  "experienceBlockTaskSwitcher": "Boolean",
  "experienceDoNotSyncBrowserSettings": "String",
  "findMyFiles": "String",
  "gameDvrBlocked": "Boolean",
  "inkWorkspaceAccess": "String",
  "inkWorkspaceAccessState": "String",
  "inkWorkspaceBlockSuggestedApps": "Boolean",
  "internetSharingBlocked": "Boolean",
  "locationServicesBlocked": "Boolean",
  "lockScreenActivateAppsWithVoice": "String",
  "lockScreenAllowTimeoutConfiguration": "Boolean",
  "lockScreenBlockActionCenterNotifications": "Boolean",
  "lockScreenBlockCortana": "Boolean",
  "lockScreenBlockToastNotifications": "Boolean",
  "lockScreenTimeoutInSeconds": "Integer",
  "logonBlockFastUserSwitching": "Boolean",
  "messagingBlockMMS": "Boolean",
  "messagingBlockRichCommunicationServices": "Boolean",
  "messagingBlockSync": "Boolean",
  "microsoftAccountBlocked": "Boolean",
  "microsoftAccountBlockSettingsSync": "Boolean",
  "microsoftAccountSignInAssistantSettings": "String",
  "networkProxyApplySettingsDeviceWide": "Boolean",
  "networkProxyAutomaticConfigurationUrl": "String",
  "networkProxyDisableAutoDetect": "Boolean",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
  },
  "nfcBlocked": "Boolean",
  "oneDriveDisableFileSync": "Boolean",
  "passwordBlockSimple": "Boolean",
  "passwordExpirationDays": "Integer",
  "passwordMinimumAgeInDays": "Integer",
  "passwordMinimumCharacterSetCount": "Integer",
  "passwordMinimumLength": "Integer",
  "passwordMinutesOfInactivityBeforeScreenTimeout": "Integer",
  "passwordPreviousPasswordBlockCount": "Integer",
  "passwordRequired": "Boolean",
  "passwordRequiredType": "String",
  "passwordRequireWhenResumeFromIdleState": "Boolean",
  "passwordSignInFailureCountBeforeFactoryReset": "Integer",
  "personalizationDesktopImageUrl": "String",
  "personalizationLockScreenImageUrl": "String",
  "powerButtonActionOnBattery": "String",
  "powerButtonActionPluggedIn": "String",
  "powerHybridSleepOnBattery": "String",
  "powerHybridSleepPluggedIn": "String",
  "powerLidCloseActionOnBattery": "String",
  "powerLidCloseActionPluggedIn": "String",
  "powerSleepButtonActionOnBattery": "String",
  "powerSleepButtonActionPluggedIn": "String",
  "printerBlockAddition": "Boolean",
  "printerDefaultName": "String",
  "printerNames": [
    "String"
  ],
  "privacyAdvertisingId": "String",
  "privacyAutoAcceptPairingAndConsentPrompts": "Boolean",
  "privacyBlockActivityFeed": "Boolean",
  "privacyBlockInputPersonalization": "Boolean",
  "privacyBlockPublishUserActivities": "Boolean",
  "privacyDisableLaunchExperience": "Boolean",
  "resetProtectionModeBlocked": "Boolean",
  "safeSearchFilter": "String",
  "screenCaptureBlocked": "Boolean",
  "searchBlockDiacritics": "Boolean",
  "searchBlockWebResults": "Boolean",
  "searchDisableAutoLanguageDetection": "Boolean",
  "searchDisableIndexerBackoff": "Boolean",
  "searchDisableIndexingEncryptedItems": "Boolean",
  "searchDisableIndexingRemovableDrive": "Boolean",
  "searchDisableLocation": "Boolean",
  "searchDisableUseLocation": "Boolean",
  "searchEnableAutomaticIndexSizeManangement": "Boolean",
  "searchEnableRemoteQueries": "Boolean",
  "securityBlockAzureADJoinedDevicesAutoEncryption": "Boolean",
  "settingsBlockAccountsPage": "Boolean",
  "settingsBlockAddProvisioningPackage": "Boolean",
  "settingsBlockAppsPage": "Boolean",
  "settingsBlockChangeLanguage": "Boolean",
  "settingsBlockChangePowerSleep": "Boolean",
  "settingsBlockChangeRegion": "Boolean",
  "settingsBlockChangeSystemTime": "Boolean",
  "settingsBlockDevicesPage": "Boolean",
  "settingsBlockEaseOfAccessPage": "Boolean",
  "settingsBlockEditDeviceName": "Boolean",
  "settingsBlockGamingPage": "Boolean",
  "settingsBlockNetworkInternetPage": "Boolean",
  "settingsBlockPersonalizationPage": "Boolean",
  "settingsBlockPrivacyPage": "Boolean",
  "settingsBlockRemoveProvisioningPackage": "Boolean",
  "settingsBlockSettingsApp": "Boolean",
  "settingsBlockSystemPage": "Boolean",
  "settingsBlockTimeLanguagePage": "Boolean",
  "settingsBlockUpdateSecurityPage": "Boolean",
  "sharedUserAppDataAllowed": "Boolean",
  "smartScreenAppInstallControl": "String",
  "smartScreenBlockPromptOverride": "Boolean",
  "smartScreenBlockPromptOverrideForFiles": "Boolean",
  "smartScreenEnableAppInstallControl": "Boolean",
  "startBlockUnpinningAppsFromTaskbar": "Boolean",
  "startMenuAppListVisibility": "String",
  "startMenuHideChangeAccountSettings": "Boolean",
  "startMenuHideFrequentlyUsedApps": "Boolean",
  "startMenuHideHibernate": "Boolean",
  "startMenuHideLock": "Boolean",
  "startMenuHidePowerButton": "Boolean",
  "startMenuHideRecentJumpLists": "Boolean",
  "startMenuHideRecentlyAddedApps": "Boolean",
  "startMenuHideRestartOptions": "Boolean",
  "startMenuHideShutDown": "Boolean",
  "startMenuHideSignOut": "Boolean",
  "startMenuHideSleep": "Boolean",
  "startMenuHideSwitchAccount": "Boolean",
  "startMenuHideUserTile": "Boolean",
  "startMenuLayoutEdgeAssetsXml": "Binary",
  "startMenuLayoutXml": "Binary",
  "startMenuMode": "String",
  "startMenuPinnedFolderDocuments": "String",
  "startMenuPinnedFolderDownloads": "String",
  "startMenuPinnedFolderFileExplorer": "String",
  "startMenuPinnedFolderHomeGroup": "String",
  "startMenuPinnedFolderMusic": "String",
  "startMenuPinnedFolderNetwork": "String",
  "startMenuPinnedFolderPersonalFolder": "String",
  "startMenuPinnedFolderPictures": "String",
  "startMenuPinnedFolderSettings": "String",
  "startMenuPinnedFolderVideos": "String",
  "storageBlockRemovableStorage": "Boolean",
  "storageRequireMobileDeviceEncryption": "Boolean",
  "storageRestrictAppDataToSystemVolume": "Boolean",
  "storageRestrictAppInstallToSystemVolume": "Boolean",
  "systemTelemetryProxyServer": "String",
  "taskManagerBlockEndTask": "Boolean",
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": "Boolean",
  "uninstallBuiltInApps": "Boolean",
  "usbBlocked": "Boolean",
  "voiceRecordingBlocked": "Boolean",
  "webRtcBlockLocalhostIpAddress": "Boolean",
  "wiFiBlockAutomaticConnectHotspots": "Boolean",
  "wiFiBlocked": "Boolean",
  "wiFiBlockManualConfiguration": "Boolean",
  "wiFiScanInterval": "Integer",
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule"
  },
  "windowsSpotlightBlockConsumerSpecificFeatures": "Boolean",
  "windowsSpotlightBlocked": "Boolean",
  "windowsSpotlightBlockOnActionCenter": "Boolean",
  "windowsSpotlightBlockTailoredExperiences": "Boolean",
  "windowsSpotlightBlockThirdPartyNotifications": "Boolean",
  "windowsSpotlightBlockWelcomeExperience": "Boolean",
  "windowsSpotlightBlockWindowsTips": "Boolean",
  "windowsSpotlightConfigureOnLockScreen": "String",
  "windowsStoreBlockAutoUpdate": "Boolean",
  "windowsStoreBlocked": "Boolean",
  "windowsStoreEnablePrivateStoreOnly": "Boolean",
  "wirelessDisplayBlockProjectionToThisDevice": "Boolean",
  "wirelessDisplayBlockUserInputFromReceiver": "Boolean",
  "wirelessDisplayRequirePinForPairing": "Boolean"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a63f677b-677b-a63f-7b67-3fa67b673fa6",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode"
  },
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
  },
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": "Boolean",
  "version": "Integer",
  "accountsBlockAddingNonMicrosoftAccountEmail": "Boolean",
  "activateAppsWithVoice": "String",
  "antiTheftModeBlocked": "Boolean",
  "appManagementMSIAllowUserControlOverInstall": "Boolean",
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": "Boolean",
  "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
    "String"
  ],
  "appsAllowTrustedAppsSideloading": "String",
  "appsBlockWindowsStoreOriginatedApps": "Boolean",
  "authenticationAllowSecondaryDevice": "Boolean",
  "authenticationPreferredAzureADTenantDomainName": "String",
  "authenticationWebSignIn": "String",
  "bluetoothAllowedServices": [
    "String"
  ],
  "bluetoothBlockAdvertising": "Boolean",
  "bluetoothBlockDiscoverableMode": "Boolean",
  "bluetoothBlocked": "Boolean",
  "bluetoothBlockPrePairing": "Boolean",
  "bluetoothBlockPromptedProximalConnections": "Boolean",
  "cameraBlocked": "Boolean",
  "cellularBlockDataWhenRoaming": "Boolean",
  "cellularBlockVpn": "Boolean",
  "cellularBlockVpnWhenRoaming": "Boolean",
  "cellularData": "String",
  "certificatesBlockManualRootCertificateInstallation": "Boolean",
  "configureTimeZone": "String",
  "connectedDevicesServiceBlocked": "Boolean",
  "copyPasteBlocked": "Boolean",
  "cortanaBlocked": "Boolean",
  "cryptographyAllowFipsAlgorithmPolicy": "Boolean",
  "dataProtectionBlockDirectMemoryAccess": "Boolean",
  "defenderBlockEndUserAccess": "Boolean",
  "defenderBlockOnAccessProtection": "Boolean",
  "defenderCloudBlockLevel": "String",
  "defenderCloudExtendedTimeout": "Integer",
  "defenderCloudExtendedTimeoutInSeconds": "Integer",
  "defenderDaysBeforeDeletingQuarantinedMalware": "Integer",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions"
  },
  "defenderDisableCatchupFullScan": "Boolean",
  "defenderDisableCatchupQuickScan": "Boolean",
  "defenderFileExtensionsToExclude": [
    "String"
  ],
  "defenderFilesAndFoldersToExclude": [
    "String"
  ],
  "defenderMonitorFileActivity": "String",
  "defenderPotentiallyUnwantedAppAction": "String",
  "defenderPotentiallyUnwantedAppActionSetting": "String",
  "defenderProcessesToExclude": [
    "String"
  ],
  "defenderPromptForSampleSubmission": "String",
  "defenderRequireBehaviorMonitoring": "Boolean",
  "defenderRequireCloudProtection": "Boolean",
  "defenderRequireNetworkInspectionSystem": "Boolean",
  "defenderRequireRealTimeMonitoring": "Boolean",
  "defenderScanArchiveFiles": "Boolean",
  "defenderScanDownloads": "Boolean",
  "defenderScanIncomingMail": "Boolean",
  "defenderScanMappedNetworkDrivesDuringFullScan": "Boolean",
  "defenderScanMaxCpu": "Integer",
  "defenderScanNetworkFiles": "Boolean",
  "defenderScanRemovableDrivesDuringFullScan": "Boolean",
  "defenderScanScriptsLoadedInInternetExplorer": "Boolean",
  "defenderScanType": "String",
  "defenderScheduledQuickScanTime": "String (time of day)",
  "defenderScheduledScanTime": "String (time of day)",
  "defenderScheduleScanEnableLowCpuPriority": "Boolean",
  "defenderSignatureUpdateIntervalInHours": "Integer",
  "defenderSubmitSamplesConsentType": "String",
  "defenderSystemScanSchedule": "String",
  "developerUnlockSetting": "String",
  "deviceManagementBlockFactoryResetOnMobile": "Boolean",
  "deviceManagementBlockManualUnenroll": "Boolean",
  "diagnosticsDataSubmissionMode": "String",
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "String"
  ],
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "String"
  ],
  "edgeAllowStartPagesModification": "Boolean",
  "edgeBlockAccessToAboutFlags": "Boolean",
  "edgeBlockAddressBarDropdown": "Boolean",
  "edgeBlockAutofill": "Boolean",
  "edgeBlockCompatibilityList": "Boolean",
  "edgeBlockDeveloperTools": "Boolean",
  "edgeBlocked": "Boolean",
  "edgeBlockEditFavorites": "Boolean",
  "edgeBlockExtensions": "Boolean",
  "edgeBlockFullScreenMode": "Boolean",
  "edgeBlockInPrivateBrowsing": "Boolean",
  "edgeBlockJavaScript": "Boolean",
  "edgeBlockLiveTileDataCollection": "Boolean",
  "edgeBlockPasswordManager": "Boolean",
  "edgeBlockPopups": "Boolean",
  "edgeBlockPrelaunch": "Boolean",
  "edgeBlockPrinting": "Boolean",
  "edgeBlockSavingHistory": "Boolean",
  "edgeBlockSearchEngineCustomization": "Boolean",
  "edgeBlockSearchSuggestions": "Boolean",
  "edgeBlockSendingDoNotTrackHeader": "Boolean",
  "edgeBlockSendingIntranetTrafficToInternetExplorer": "Boolean",
  "edgeBlockSideloadingExtensions": "Boolean",
  "edgeBlockTabPreloading": "Boolean",
  "edgeBlockWebContentOnNewTabPage": "Boolean",
  "edgeClearBrowsingDataOnExit": "Boolean",
  "edgeCookiePolicy": "String",
  "edgeDisableFirstRunPage": "Boolean",
  "edgeEnterpriseModeSiteListLocation": "String",
  "edgeFavoritesBarVisibility": "String",
  "edgeFavoritesListLocation": "String",
  "edgeFirstRunUrl": "String",
  "edgeHomeButtonConfiguration": {
    "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
  },
  "edgeHomeButtonConfigurationEnabled": "Boolean",
  "edgeHomepageUrls": [
    "String"
  ],
  "edgeKioskModeRestriction": "String",
  "edgeKioskResetAfterIdleTimeInMinutes": "Integer",
  "edgeNewTabPageURL": "String",
  "edgeOpensWith": "String",
  "edgePreventCertificateErrorOverride": "Boolean",
  "edgeRequiredExtensionPackageFamilyNames": [
    "String"
  ],
  "edgeRequireSmartScreen": "Boolean",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeSendIntranetTrafficToInternetExplorer": "Boolean",
  "edgeShowMessageWhenOpeningInternetExplorerSites": "String",
  "edgeSyncFavoritesWithInternetExplorer": "Boolean",
  "edgeTelemetryForMicrosoft365Analytics": "String",
  "enableAutomaticRedeployment": "Boolean",
  "energySaverOnBatteryThresholdPercentage": "Integer",
  "energySaverPluggedInThresholdPercentage": "Integer",
  "enterpriseCloudPrintDiscoveryEndPoint": "String",
  "enterpriseCloudPrintDiscoveryMaxLimit": "Integer",
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "String",
  "enterpriseCloudPrintOAuthAuthority": "String",
  "enterpriseCloudPrintOAuthClientIdentifier": "String",
  "enterpriseCloudPrintResourceIdentifier": "String",
  "experienceBlockDeviceDiscovery": "Boolean",
  "experienceBlockErrorDialogWhenNoSIM": "Boolean",
  "experienceBlockTaskSwitcher": "Boolean",
  "experienceDoNotSyncBrowserSettings": "String",
  "findMyFiles": "String",
  "gameDvrBlocked": "Boolean",
  "inkWorkspaceAccess": "String",
  "inkWorkspaceAccessState": "String",
  "inkWorkspaceBlockSuggestedApps": "Boolean",
  "internetSharingBlocked": "Boolean",
  "locationServicesBlocked": "Boolean",
  "lockScreenActivateAppsWithVoice": "String",
  "lockScreenAllowTimeoutConfiguration": "Boolean",
  "lockScreenBlockActionCenterNotifications": "Boolean",
  "lockScreenBlockCortana": "Boolean",
  "lockScreenBlockToastNotifications": "Boolean",
  "lockScreenTimeoutInSeconds": "Integer",
  "logonBlockFastUserSwitching": "Boolean",
  "messagingBlockMMS": "Boolean",
  "messagingBlockRichCommunicationServices": "Boolean",
  "messagingBlockSync": "Boolean",
  "microsoftAccountBlocked": "Boolean",
  "microsoftAccountBlockSettingsSync": "Boolean",
  "microsoftAccountSignInAssistantSettings": "String",
  "networkProxyApplySettingsDeviceWide": "Boolean",
  "networkProxyAutomaticConfigurationUrl": "String",
  "networkProxyDisableAutoDetect": "Boolean",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
  },
  "nfcBlocked": "Boolean",
  "oneDriveDisableFileSync": "Boolean",
  "passwordBlockSimple": "Boolean",
  "passwordExpirationDays": "Integer",
  "passwordMinimumAgeInDays": "Integer",
  "passwordMinimumCharacterSetCount": "Integer",
  "passwordMinimumLength": "Integer",
  "passwordMinutesOfInactivityBeforeScreenTimeout": "Integer",
  "passwordPreviousPasswordBlockCount": "Integer",
  "passwordRequired": "Boolean",
  "passwordRequiredType": "String",
  "passwordRequireWhenResumeFromIdleState": "Boolean",
  "passwordSignInFailureCountBeforeFactoryReset": "Integer",
  "personalizationDesktopImageUrl": "String",
  "personalizationLockScreenImageUrl": "String",
  "powerButtonActionOnBattery": "String",
  "powerButtonActionPluggedIn": "String",
  "powerHybridSleepOnBattery": "String",
  "powerHybridSleepPluggedIn": "String",
  "powerLidCloseActionOnBattery": "String",
  "powerLidCloseActionPluggedIn": "String",
  "powerSleepButtonActionOnBattery": "String",
  "powerSleepButtonActionPluggedIn": "String",
  "printerBlockAddition": "Boolean",
  "printerDefaultName": "String",
  "printerNames": [
    "String"
  ],
  "privacyAdvertisingId": "String",
  "privacyAutoAcceptPairingAndConsentPrompts": "Boolean",
  "privacyBlockActivityFeed": "Boolean",
  "privacyBlockInputPersonalization": "Boolean",
  "privacyBlockPublishUserActivities": "Boolean",
  "privacyDisableLaunchExperience": "Boolean",
  "resetProtectionModeBlocked": "Boolean",
  "safeSearchFilter": "String",
  "screenCaptureBlocked": "Boolean",
  "searchBlockDiacritics": "Boolean",
  "searchBlockWebResults": "Boolean",
  "searchDisableAutoLanguageDetection": "Boolean",
  "searchDisableIndexerBackoff": "Boolean",
  "searchDisableIndexingEncryptedItems": "Boolean",
  "searchDisableIndexingRemovableDrive": "Boolean",
  "searchDisableLocation": "Boolean",
  "searchDisableUseLocation": "Boolean",
  "searchEnableAutomaticIndexSizeManangement": "Boolean",
  "searchEnableRemoteQueries": "Boolean",
  "securityBlockAzureADJoinedDevicesAutoEncryption": "Boolean",
  "settingsBlockAccountsPage": "Boolean",
  "settingsBlockAddProvisioningPackage": "Boolean",
  "settingsBlockAppsPage": "Boolean",
  "settingsBlockChangeLanguage": "Boolean",
  "settingsBlockChangePowerSleep": "Boolean",
  "settingsBlockChangeRegion": "Boolean",
  "settingsBlockChangeSystemTime": "Boolean",
  "settingsBlockDevicesPage": "Boolean",
  "settingsBlockEaseOfAccessPage": "Boolean",
  "settingsBlockEditDeviceName": "Boolean",
  "settingsBlockGamingPage": "Boolean",
  "settingsBlockNetworkInternetPage": "Boolean",
  "settingsBlockPersonalizationPage": "Boolean",
  "settingsBlockPrivacyPage": "Boolean",
  "settingsBlockRemoveProvisioningPackage": "Boolean",
  "settingsBlockSettingsApp": "Boolean",
  "settingsBlockSystemPage": "Boolean",
  "settingsBlockTimeLanguagePage": "Boolean",
  "settingsBlockUpdateSecurityPage": "Boolean",
  "sharedUserAppDataAllowed": "Boolean",
  "smartScreenAppInstallControl": "String",
  "smartScreenBlockPromptOverride": "Boolean",
  "smartScreenBlockPromptOverrideForFiles": "Boolean",
  "smartScreenEnableAppInstallControl": "Boolean",
  "startBlockUnpinningAppsFromTaskbar": "Boolean",
  "startMenuAppListVisibility": "String",
  "startMenuHideChangeAccountSettings": "Boolean",
  "startMenuHideFrequentlyUsedApps": "Boolean",
  "startMenuHideHibernate": "Boolean",
  "startMenuHideLock": "Boolean",
  "startMenuHidePowerButton": "Boolean",
  "startMenuHideRecentJumpLists": "Boolean",
  "startMenuHideRecentlyAddedApps": "Boolean",
  "startMenuHideRestartOptions": "Boolean",
  "startMenuHideShutDown": "Boolean",
  "startMenuHideSignOut": "Boolean",
  "startMenuHideSleep": "Boolean",
  "startMenuHideSwitchAccount": "Boolean",
  "startMenuHideUserTile": "Boolean",
  "startMenuLayoutEdgeAssetsXml": "Binary",
  "startMenuLayoutXml": "Binary",
  "startMenuMode": "String",
  "startMenuPinnedFolderDocuments": "String",
  "startMenuPinnedFolderDownloads": "String",
  "startMenuPinnedFolderFileExplorer": "String",
  "startMenuPinnedFolderHomeGroup": "String",
  "startMenuPinnedFolderMusic": "String",
  "startMenuPinnedFolderNetwork": "String",
  "startMenuPinnedFolderPersonalFolder": "String",
  "startMenuPinnedFolderPictures": "String",
  "startMenuPinnedFolderSettings": "String",
  "startMenuPinnedFolderVideos": "String",
  "storageBlockRemovableStorage": "Boolean",
  "storageRequireMobileDeviceEncryption": "Boolean",
  "storageRestrictAppDataToSystemVolume": "Boolean",
  "storageRestrictAppInstallToSystemVolume": "Boolean",
  "systemTelemetryProxyServer": "String",
  "taskManagerBlockEndTask": "Boolean",
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": "Boolean",
  "uninstallBuiltInApps": "Boolean",
  "usbBlocked": "Boolean",
  "voiceRecordingBlocked": "Boolean",
  "webRtcBlockLocalhostIpAddress": "Boolean",
  "wiFiBlockAutomaticConnectHotspots": "Boolean",
  "wiFiBlocked": "Boolean",
  "wiFiBlockManualConfiguration": "Boolean",
  "wiFiScanInterval": "Integer",
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule"
  },
  "windowsSpotlightBlockConsumerSpecificFeatures": "Boolean",
  "windowsSpotlightBlocked": "Boolean",
  "windowsSpotlightBlockOnActionCenter": "Boolean",
  "windowsSpotlightBlockTailoredExperiences": "Boolean",
  "windowsSpotlightBlockThirdPartyNotifications": "Boolean",
  "windowsSpotlightBlockWelcomeExperience": "Boolean",
  "windowsSpotlightBlockWindowsTips": "Boolean",
  "windowsSpotlightConfigureOnLockScreen": "String",
  "windowsStoreBlockAutoUpdate": "Boolean",
  "windowsStoreBlocked": "Boolean",
  "windowsStoreEnablePrivateStoreOnly": "Boolean",
  "wirelessDisplayBlockProjectionToThisDevice": "Boolean",
  "wirelessDisplayBlockUserInputFromReceiver": "Boolean",
  "wirelessDisplayRequirePinForPairing": "Boolean"
}
```

