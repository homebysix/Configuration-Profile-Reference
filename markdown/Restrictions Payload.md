# Restrictions Payload  

 [Configuration Profile Reference - Restrictions Payload](https://developer.apple.com/library/content/featuredarticles/iPhoneConfigurationProfileRef/Introduction/Introduction.html#//apple_ref/doc/uid/TP40010206-CH1-SW13)  

The Restrictions payload is designated by specifying `com.apple.applicationaccess` as the `PayloadType` value.  

A Restrictions payload allows the administrator to restrict the user from doing certain things with the device, such as using the camera.  


> **Note:** You can specify additional restrictions, including maximum allowed content ratings, by creating a profile using Apple Configurator 2 or Profile Manager.  
  

The Restrictions payload is supported in iOS; some keys are also supported in macOS, as noted below.  

In addition to the settings common to all payloads, this payload defines the following keys:  

|Key|Type|Value|
|-|-|-|
|`allowAccountModification`|Boolean|Optional. Supervised only. If set to `false`, account modification is disabled.</br>**Availability:** Available only in iOS 7.0 and later.|
|`allowAddingGameCenterFriends`|Boolean|Optional. When `false`, prohibits adding friends to Game Center. This key is deprecated on unsupervised devices.|
|`allowAirDrop`|Boolean|Optional. Supervised only. If set to `false`, AirDrop is disabled.</br>**Availability:** Available only in iOS 7.0 and later.|
|`allowAppCellularDataModification`|Boolean|Optional. Supervised only. If set to `false`, changes to cellular data usage for apps are disabled.</br>**Availability:** Available only in iOS 7.0 and later.|
|`allowAppInstallation`|Boolean|Optional. Supervised only. When `false`, the App Store is disabled and its icon is removed from the Home screen. Users are unable to install or update their applications. This key is deprecated on unsupervised devices.|
|`allowAppRemoval`|Boolean|Optional. When `false`, disables removal of apps from iOS device. This key is deprecated on unsupervised devices.|
|`allowAssistant`|Boolean|Optional. When `false`, disables Siri. Defaults to `true`.|
|`allowAssistantUserGeneratedContent`|Boolean|Optional. Supervised only. When `false`, prevents Siri from querying user-generated content from the web.</br>**Availability:** Available in iOS 7 and later.|
|`allowAssistantWhileLocked`|Boolean|Optional. When `false`, the user is unable to use Siri when the device is locked. Defaults to `true`. This restriction is ignored if the device does not have a passcode set.</br>**Availability:** Available only in iOS 5.1 and later.|
|`allowBookstore`|Boolean|Optional. Supervised only. If set to `false`, iBookstore will be disabled. This will default to `true`.</br>**Availability:** Available in iOS 6.0 and later.|
|`allowBookstoreErotica`|Boolean|Optional. Supervised only prior to iOS 6.1. If set to `false`, the user will not be able to download media from the iBookstore that has been tagged as erotica. This will default to `true`.</br>**Availability:** Available in iOS 6.0 and later.|
|`allowCamera`|Boolean|Optional. When `false`, the camera is completely disabled and its icon is removed from the Home screen. Users are unable to take photographs.</br>**Availability:** Available in iOS and in macOS 10.11 and later.|
|`allowChat`|Boolean|Optional. When `false`, disables the use of the Messages app with supervised devices.</br>**Availability:** Available in iOS 6.0 and later.|
|`allowCloudBackup`|Boolean|Optional. When `false`, disables backing up the device to iCloud.</br>**Availability:** Available in iOS 5.0 and later.|
|`allowCloudBTMM`|Boolean|Optional. When `false`, disallows macOS Back to My Mac iCloud service.</br>**Availability:** Available in macOS 10.12 and later.|
|`allowCloudFMM`|Boolean|Optional. When `false`, disallows macOS Find My Mac iCloud service.</br>**Availability:** Available in macOS 10.12 and later.|
|`allowCloudBookmarks`|Boolean|Optional. When `false`, disallows macOS iCloud Bookmark sync.</br>**Availability:** Available in macOS 10.12 and later.|
|`allowCloudMail`|Boolean|Optional. When `false`, disallows macOS Mail iCloud services.</br>**Availability:** Available in macOS 10.12 and later.|
|`allowCloudCalendar`|Boolean|Optional. When `false`, disallows macOS iCloud Calendar services.</br>**Availability:** Available in macOS 10.12 and later.|
|`allowCloudReminders`|Boolean|Optional. When `false`, disallows iCloud Reminder services.</br>**Availability:** Available in macOS 10.12 and later.|
|`allowCloudAddressBook`|Boolean|Optional. When `false`, disallows macOS iCloud Address Book services.</br>**Availability:** Available in macOS 10.12 and later.|
|`allowCloudNotes`|Boolean|Optional. When `false`, disallows macOS iCloud Notes services.</br>**Availability:** Available in macOS 10.12 and later.|
|`allowCloudDocumentSync`|Boolean|Optional. When `false`, disables document and  key-value syncing to iCloud. This key is deprecated on unsupervised devices.</br>**Availability:** Available in iOS 5.0 and later and in macOS 10.11 and later.|
|`allowCloudKeychainSync`|Boolean|Optional. If `false`, disables iCloud keychain synchronization. Default is `true`.</br>**Availability:** Available in iOS 7.0 and later and macOS 10.12 and later.|
|`allowDiagnosticSubmission`|Boolean|Optional. When `false`, this prevents the device from automatically submitting diagnostic reports to Apple. Defaults to `true`.</br>**Availability:** Available only in iOS 6.0 and later.|
|`allowExplicitContent`|Boolean|Optional. When `false`, explicit music or video content purchased from the iTunes Store is hidden. Explicit content is marked as such by content providers, such as record labels, when sold through the iTunes Store. This key is deprecated on unsupervised devices.|
|`allowFindMyFriendsModification`|Boolean|Optional. Supervised only. If set to `false`, changes to Find My Friends are disabled.</br>**Availability:** Available only in iOS 7.0 and later.|
|`allowFingerprintForUnlock`|Boolean|Optional. If `false`, prevents Touch ID from unlocking a device.</br>**Availability:** Available in iOS 7 and later.|
|`allowGameCenter`|Boolean|Optional. Supervised only. When `false`, Game Center is disabled and its icon is removed from the Home screen. Default is `true`.</br>**Availability:** Available only in iOS 6.0 and later.|
|`allowGlobalBackgroundFetchWhenRoaming`|Boolean|Optional. When `false`, disables global background fetch activity when an iOS phone is roaming.|
|`allowInAppPurchases`|Boolean|Optional. When `false`, prohibits in-app purchasing.|
|`allowLockScreenControlCenter`|Boolean|Optional. If `false`, prevents Control Center from appearing on the Lock screen.</br>**Availability:** Available in iOS 7 and later.|
|`allowHostPairing`|Boolean|Supervised only. If set to `false`, host pairing is disabled with the exception of the supervision host. If no supervision host certificate has been configured, all pairing is disabled. Host pairing lets the administrator control which devices an iOS 7 device can pair with.</br>**Availability:** Available only in iOS 7.0 and later.|
|`allowLockScreenNotificationsView`|Boolean|Optional. If set to `false`, the Notifications view in Notification Center on the lock screen is disabled and users can’t receive notifications when the screen is locked.</br>**Availability:** Available only in iOS 7.0 and later.|
|`allowLockScreenTodayView`|Boolean|Optional. If set to `false`, the Today view in Notification Center on the lock screen is disabled.</br>**Availability:** Available only in iOS 7.0 and later.|
|`allowMultiplayerGaming`|Boolean|Optional. When `false`, prohibits multiplayer gaming. This key is deprecated on unsupervised devices.|
|`allowOpenFromManagedToUnmanaged`|Boolean|Optional. If `false`, documents in managed apps and accounts only open in other managed apps and accounts. Default is `true`.</br>**Availability:** Available only in iOS 7.0 and later.|
|`allowOpenFromUnmanagedToManaged`|Boolean|Optional. If set to `false`, documents in unmanaged apps and accounts will only open in other unmanaged apps and accounts. Default is `true`.</br>**Availability:** Available only in iOS 7.0 and later.|
|`allowOTAPKIUpdates`|Boolean|Optional. If `false`, over-the-air PKI updates are disabled. Setting this restriction to false does not disable CRL and OCSP checks. Default is `true`.</br>**Availability:** Available only in iOS 7.0 and later.|
|`allowPassbookWhileLocked`|Boolean|Optional. If set to `false`, Passbook notifications will not be shown on the lock screen.This will default to `true`.</br>**Availability:** Available in iOS 6.0 and later.|
|`allowPhotoStream`|Boolean|Optional. When `false`, disables Photo Stream.</br>**Availability:** Available in iOS 5.0 and later.|
|`allowSafari`|Boolean|Optional. When `false`, the Safari web browser application is disabled and its icon removed from the Home screen. This also prevents users from opening web clips. This key is deprecated on unsupervised devices.|
|`safariAllowAutoFill`|Boolean|Optional. When `false`, Safari auto-fill is disabled. Defaults to true.|
|`safariForceFraudWarning`|Boolean|Optional. When `true`, Safari fraud warning is enabled. Defaults to false.|
|`safariAllowJavaScript`|Boolean|Optional. When `false`, Safari will not execute JavaScript. Defaults to true.|
|`safariAllowPopups`|Boolean|Optional. When `false`, Safari will not allow pop-up tabs. Defaults to true.|
|`safariAcceptCookies`|Integer|Optional. Determines conditions under which the device will accept cookies. Following are allowed values:</br></br>* 0:	 Never  </br></br>* 1:	 From visited sites only  </br></br>* 1.5: From websites I visit (enter `'&lt;real&gt;1.5&lt;/real&gt;'`)  </br></br>* 2:	 Always  </br></br></br>Defaults to 2.|
|`allowSharedStream`|Boolean|Optional. If set to `false`, Shared Photo Stream will be disabled. This will default to `true`.</br>**Availability:** Available in iOS 6.0 and later.|
|`allowUIConfigurationProfileInstallation`|Boolean|Optional. Supervised only. If set to `false`, the user is prohibited from installing configuration profiles and certificates interactively. This will default to `true`.</br>**Availability:** Available in iOS 6.0 and later.|
|`allowUntrustedTLSPrompt`|Boolean|Optional. When `false`, automatically rejects untrusted HTTPS certificates without prompting the user.</br>**Availability:** Available in iOS 5.0 and later.|
|`allowVideoConferencing`|Boolean|Optional. When `false`, disables video conferencing. This key is deprecated on unsupervised devices.|
|`allowVoiceDialing`|Boolean|Optional. When `false`, disables voice dialing if the device is locked with a passcode. Default is `true`.|
|`allowYouTube`|Boolean|Optional. When `false`, the YouTube application is disabled and its icon is removed from the Home screen.</br>This key is ignored in iOS 6 and later because the YouTube app is not provided.|
|`allowiTunes`|Boolean|Optional. When `false`, the iTunes Music Store is disabled and its icon is removed from the Home screen. Users cannot preview, purchase, or download content. This key is deprecated on unsupervised devices.|
|`autonomousSingleAppModePermittedAppIDs`|Array of strings|Optional. Supervised only. If present, allows apps identified by the bundle IDs listed in the array to autonomously enter Single App Mode.</br>**Availability:** Available only in iOS 7.0 and later.|
|`forceAssistantProfanityFilter`|Boolean|Optional. Supervised only. When `true`, forces the use of the profanity filter assistant.|
|`forceEncryptedBackup`|Boolean|Optional. When `true`, encrypts all backups.|
|`forceITunesStorePasswordEntry`|Boolean|Optional. When `true`, forces user to enter their iTunes password for each transaction.</br>**Availability:** Available in iOS 5.0 and later.|
|`forceLimitAdTracking`|Boolean|Optional. If `true`, limits ad tracking. Default is `false`.</br>**Availability:** Available only in iOS 7.0 and later.|
|`forceAirPlayOutgoingRequestsPairingPassword`|Boolean|Optional. If set to `true`, forces all devices receiving AirPlay requests from this device to use a pairing password. Default is `false`.</br>**Availability:** Available only in iOS 7.1 and later.|
|`forceAirPlayIncomingRequestsPairingPassword`|Boolean|Optional. If set to `true`, forces all devices sending AirPlay requests to this device to use a pairing password. Default is `false`.</br>**Availability:** Available only in Apple TV 6.1 and later.|
|`allowManagedAppsCloudSync`|Boolean|Optional. If set to `false`, prevents managed applications from using iCloud sync.|
|`allowEraseContentAndSettings`|Boolean|Supervised only. If set to `false`, disables the “Erase All Content And Settings” option in the Reset UI.|
|`allowSpotlightInternetResults`|Boolean|Supervised only. If set to `false`, Spotlight will not return Internet search results.</br>**Availability:** Available in iOS and in macOS 10.11 and later.|
|`allowEnablingRestrictions`|Boolean|Supervised only. If set to `false`, disables the "Enable Restrictions" option in the Restrictions UI in Settings.|
|`allowActivityContinuation`|Boolean|If set to `false`, Activity Continuation will be disabled. Defaults to `true`.|
|`allowEnterpriseBookBackup`|Boolean|If set to `false`, Enterprise books will not be backed up. Defaults to `true`.|
|`allowEnterpriseBookMetadataSync`|Boolean|If set to `false`, Enterprise books notes and highlights will not be synced. Defaults to `true`.|
|`allowPodcasts`|Boolean|Supervised only. If set to `false`, disables podcasts. Defaults to `true`.</br>**Availability:** Available in iOS 8.0 and later.|
|`allowDefinitionLookup`|Boolean|Supervised only. If set to `false`, disables definition lookup. Defaults to `true`.</br>**Availability:** Available in iOS 8.1.3 and later and in macOS 10.11.2 and later.|
|`allowPredictiveKeyboard`|Boolean|Supervised only. If set to `false`, disables predictive keyboards. Defaults to `true`.</br>**Availability:** Available in iOS 8.1.3 and later.|
|`allowAutoCorrection`|Boolean|Supervised only. If set to `false`, disables keyboard auto-correction. Defaults to `true`.</br>**Availability:** Available in iOS 8.1.3 and later.|
|`allowSpellCheck`|Boolean|Supervised only. If set to `false`, disables keyboard spell-check. Defaults to `true`.</br>**Availability:** Available in iOS 8.1.3 and later.|
|`forceWatchWristDetection`|Boolean|If set to `true`, a paired Apple Watch will be forced to use Wrist Detection. Defaults to `false`.</br>**Availability:** Available in iOS 8.2 and later.|
|`allowMusicService`|Boolean|Supervised only. If set to `false`, Music service is disabled and Music app reverts to classic mode. Defaults to `true`.</br>**Availability:** Available in iOS 9.3 and later and macOS 10.12 and later.|
|`allowCloudPhotoLibrary`|Boolean|If set to `false`, disables iCloud Photo Library. Any photos not fully downloaded from iCloud Photo Library to the device will be removed from local storage.</br>**Availability:** Available in iOS 9.0 and later.|
|`allowNews`|Boolean|Supervised only. If set to `false`, disables News. Defaults to `true`.</br>**Availability:** Available in iOS 9.0 and later.|
|`forceAirDropUnmanaged`|Boolean|Optional. If set to `true`, causes AirDrop to be considered an unmanaged drop target. Defaults to `false`.</br>**Availability:** Available in iOS 9.0 and later.|
|`allowUIAppInstallation`|Boolean|Supervised only. When `false`, the App Store is disabled and its icon is removed from the Home screen. However, users may continue to use Host apps (iTunes, Configurator) to install or update their apps. Defaults to `true`.</br>**Availability:** Available in iOS 9.0 and later.|
|`allowScreenShot`|Boolean|Optional. If set to `false`, users can’t save a screenshot of the display and are prevented from capturing a screen recording; it also prevents the Classroom app from observing remote screens. Defaults to `true`.</br>**Availability:** Updated in iOS 9.0 to include screen recordings.|
|`allowKeyboardShortcuts`|Boolean|Supervised only. If set to `false`, keyboard shortcuts cannot be used. Defaults to `true`.</br>**Availability:** Available in iOS 9.0 and later.|
|`allowPairedWatch`|Boolean|Supervised only. If set to `false`, disables pairing with an Apple Watch. Any currently paired Apple Watch is unpaired and erased. Defaults to `true`.</br>**Availability:** Available in iOS 9.0 and later.|
|`allowPasscodeModification`|Boolean|Supervised only. If set to `false`, prevents the device passcode from being added, changed, or removed. Defaults to `true`. This restriction is ignored by shared iPads.</br>**Availability:** Available in iOS 9.0 and later.|
|`allowDeviceNameModification`|Boolean|Supervised only. If set to `false`, prevents device name from being changed. Defaults to `true`.</br>**Availability:** Available in iOS 9.0 and later.|
|`allowWallpaperModification`|Boolean|Supervised only. If set to `false`, prevents wallpaper from being changed. Defaults to `true`.</br>**Availability:** Available in iOS 9.0 and later.|
|`allowAutomaticAppDownloads`|Boolean|Supervised only. If set to `false`, prevents automatic downloading of apps purchased on other devices. Does not affect updates to existing apps. Defaults to `true`.</br>**Availability:** Available in iOS 9.0 and later.|
|`allowEnterpriseAppTrust`|Boolean|If set to `false` removes the Trust Enterprise Developer button in Settings->General->Profiles & Device Management, preventing apps from being provisioned by universal provisioning profiles. This restriction applies to free developer accounts but it does not apply to enterprise app developers who are trusted because their apps were pushed via MDM, nor does it revoke previously granted trust. Defaults to `true`.</br>**Availability:** Available in iOS 9.0 and later.|
|`allowRadioService`|Boolean|Supervised only. If set to `false`, Apple Music Radio is disabled. Defaults to `true`.</br>**Availability:** Available in iOS 9.3 and later.|
|`blacklistedAppBundleIDs`|Array of strings|Supervised only. If present, prevents bundle IDs listed in the array from being shown or launchable.</br>**Availability:** Available in iOS 9.3 and later.|
|`whitelistedAppBundleIDs`|Array of strings|Supervised only. If present, allows only bundle IDs listed in the array from being shown or launchable.</br>**Availability:** Available in iOS 9.3 and later.|
|`allowNotificationsModification`|Boolean|Supervised only. If set to `false`, notification settings cannot be modified. Defaults to `true`.</br>**Availability:** Available in iOS 9.3 and later.|
|`allowRemoteScreenObservation`|Boolean|Supervised only. If set to `false`, remote screen observation by the Classroom app is disabled. Defaults to `true`.</br>This key should be nested beneath `allowScreenShot` as a sub-restriction. If `allowScreenShot` is set to false, it also prevents the Classroom app from observing remote screens.</br>**Availability:** Available in iOS 9.3 and later.|
|`allowDiagnosticSubmissionModification`|Boolean|Supervised only. If set to `false`, the diagnostic submission and app analytics settings in the Diagnostics & Usage pane in Settings cannot be modified. Defaults to `true`.</br>**Availability:** Available in iOS 9.3.2 and later.|
|`allowBluetoothModification`|Boolean|Supervised only. If set to `false`, prevents modification of Bluetooth settings. Defaults to `true`.</br>**Availability:** Available in iOS 10.0 and later.|
  