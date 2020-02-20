# Role Name:
- ansible-role-compliance-windows-windows-components-policy-2019

# Description:
This Windows Components Policy Role was based off the CIS specs for 2019
servers.   This role covers the "Windows Components" CIS section only. The
checks and remediation commands are for local settings only. Group Policy
settings may override these settings. When the "remediate" variable is set
to "YES", the role will try to remediate the server's setting(s) according
to the CIS standards.  The defaults/main.yml file can be used to disable
specific CIS items (i.e. execute_###) from executing. The default value in
the defaults/main.yml for these CIS item variables (i.e. execute_###) is "YES".   
The value "YES" means that CIS item will execute at run time. Set the value to
"NO" if you want to skip this CIS item in question from executing.

# Requirements:
Windows Ansible related pre-requisites

# Role Variables:
# defaults file - ansible-role-compliance-windows-windows-components-policy-2019
Parameter | Choices/Defaults|Comments
----------|-----------------|--------
__remediate__ |"NO"| to determine whether or not to remediate settings.
__AllowSharedLocalAppData_cis__ |"0"| CIS Value.
__MSAOptional_cis__ |"1"| CIS value.
__BlockHostedAppAccessWinRT_cis__ |"1"| CIS Value.
__NoAutoplayfornonVolume_cis__ |"1"| CIS Value.
__NoAutorun_cis__ |"1"| CIS Value.
__NoDriveTypeAutoRun_cis__ |"255"| CIS Value.
__EnhancedAntiSpoofing_cis__ |"1"| CIS Value.
__AllowCamera_cis__ |"0"| CIS Value.
__DisableWindowsConsumerFeatures_cis__ |"1"| CIS Value.
__RequirePinForPairing_cis__ |"1"| CIS Value.
__DisablePasswordReveal_cis__ |"1"| CIS Value.
__EnumerateAdministrators_cis__ |"0"| CIS Value.
__AllowTelemetry_cis__ |"0"| CIS Value.
__EnableConfigFlighting_cis__ |"0"| CIS Value.
__DoNotShowFeedbackNotifications_cis__ |"1"| CIS Value.
__AllowBuildPreview_cis__ |"0"| CIS Value.
__Retention_cis__ |"0"| CIS Value.
__MaxSize_cis__ |32768| CIS Value.
__Retention2_cis__ |"0"| CIS Value.
__MaxSize2_cis__ |196608| CIS Value.
__Retention3_cis__ |"0"| CIS Value.
__MaxSize3_cis__ |32768| CIS Value.
__Retention4_cis__ |"0"| CIS Value.
__MaxSize4_cis__ |32768| CIS Value.
__EnableSmartScreen_cis__ |"0"| CIS Value.
__NoDataExecutionPrevention_cis__ |"0"| CIS Value.
__NoHeapTerminationOnCorruption_cis__ |"0"| CIS Value.
__PreXPSP2ShellProtocolBehavior_cis__ |"0"| CIS Value.
__DisableLocation_cis__ |"1"| CIS Value.
__ExtensionsEnabled_cis__ |"0"| CIS Value.
__AllowInPrivate_cis__ |"0"| CIS Value.
__Cookies_cis__ |"1"| CIS Value.
__FormSuggest_Passwords_cis__ |"no"| CIS Value.
__AllowPopups_cis__ |"1"| CIS Value.
__ShowSearchSuggestionsGlobal_cis__ |"0"| CIS Value.
__EnabledV9_cis__ |"1"| CIS Value.
__PreventAccessToAboutFlagsInMicrosoftEdge_cis__ |"0"| CIS Value.
__PreventOverrideAppRepUnknown_cis__ |"1"| CIS Value.
__PreventOverride_cis__ |"1"| CIS Value.
__HideLocalHostIP_cis__ |"1"| CIS Value.
__DisableFileSyncNGSC_cis__ |"1"| CIS Value.
__DisablePasswordSaving_cis__ |"1"| CIS Value.
__fSingleSessionPerUser_cis__ |"1"| CIS Value.
__fDisableCcm_cis__ |"1"| CIS Value.
__fDisableCdm_cis__ |"1"| CIS Value.
__fDisableLPT_cis__ |"1"| CIS Value.
__fDisablePNPRedir_cis__ |"1"| CIS Value.
__fPromptForPassword_cis__ |"1"| CIS Value.
__fEncryptRPCTraffic_cis__ |"1"| CIS Value.
__MinEncryptionLevel_cis__ |"3"| CIS Value.
__MaxIdleTime_cis__ |900000| CIS Value.
__MaxDisconnectionTime_cis__ |"60000"| CIS Value.
__DeleteTempDirsOnExit_cis__ |"1"| CIS Value.
__PerSessionTempDir_cis__ |"1"| CIS Value.
__DisableEnclosureDownload_cis__ |"1"| CIS Value.
__AllowCortana_cis__ |"0"| CIS Value.
__AllowCortanaAboveLock_cis__ |"0"| CIS Value.
__AllowIndexingEncryptedStoresOrItems_cis__ |"0"| CIS Value.
__AllowSearchToUseLocation_cis__ |"0"| CIS Value.
__NoGenTicket_cis__ |"1"| CIS Value.
__DisableStoreApps_cis__ |"0"| CIS Value.
__AutoDownload_cis__ |"2"| CIS Value.
__DisableOSUpgrade_cis__ |"1"| CIS Value.
__RemoveWindowsStore_cis__ |"1"| CIS Value.
__SpyNetReporting_cis__ |"0"| CIS Value.
__DisableGenericReports_cis__ |"1"| CIS Value.
__AllowSuggestedAppsInWindowsInkWorkspace_cis__ |"0"| CIS Value.
__AllowWindowsInkWorkspace_cis__ |"1"| CIS Value.
__EnableUserControl_cis__ |"0"| CIS Value.
__AlwaysInstallElevated_cis__ |"0"| CIS Value.
__SafeForScripting_cis__ |"0"| CIS Value.
__DisableAutomaticRestartSignOn_cis__ |"1"| CIS Value.
__EnableScriptBlockLogging_cis__ |"1"| CIS Value.
__EnableTranscripting_cis__ |"0"| CIS Value.
__AllowBasic_cis__ |"0"| CIS Value.
__AllowUnencryptedTraffic_cis__ |"0"| CIS Value.
__AllowDigest_cis__ |"0"| CIS Value.
__AllowBasic2_cis__ |"0"| CIS Value.
__AllowAutoConfig_cis__ |"1"| CIS Value.
__AllowUnencryptedTraffic2_cis__ |"0"| CIS Value.
__DisableRunAs_cis__ |"1"| CIS Value.
__AllowRemoteShellAccess_cis__ |"1"| CIS Value.
__NoAutoUpdate_cis__ |"1"| CIS Value.
__ScheduledInstallDay_cis__ |"0"| CIS Value.
__NoAutoRebootWithLoggedOnUsers_cis__ |"0"| CIS Value.
__SaveZoneInformation_cis__ |"2"| CIS Value.
__ScanWithAntiVirus_cis__ |"3"| CIS Value.
__ConfigureWindowsSpotlight_cis__ |"2"| CIS Value.
__DisableThirdPartySuggestions_cis__ |"1"| CIS Value.
__DisableWindowsSpotlightFeatures_cis__ |"1"| CIS Value.
__NoInPlaceSharing_cis__ |"1"| CIS Value.| CIS Value.
__AlwaysInstallElevated2_cis__ |"0"| CIS Value.
__PreventCodecDownload_cis__ |"1"| CIS Value.
__LetAppsAccessAccountInfo_cis__ |"2"| CIS Value.
__LetAppsAccessCalendar_cis__ |"2"| CIS Value.
__LetAppsAccessCallHistory_cis__ |"2"| CIS Value.
__LetAppsAccessCamera_cis__ |"2"| CIS Value.
__LetAppsAccessContacts_cis__ |"2"| CIS Value.
__LetAppsAccessEmail_cis__ |"2"| CIS Value.
__LetAppsAccessLocation_cis__ |"2"| CIS Value.
__LetAppsAccessMessaging_cis__ |"2"| CIS Value.
__LetAppsAccessMicrophone_cis__ |"2"| CIS Value.
__LetAppsAccessMotion_cis__ |"2"| CIS Value.
__LetAppsAccessRadios_cis__ |"2"| CIS Value.
__LetAppsAccessTrustedDevices_cis__ |"2"| CIS Value.
__LetAppsSyncWithDevices_cis__ |"2"| CIS Value.
__LetAppsAccessPhone_cis__ |"2"| CIS Value.
__LetAppsAccessNotifications_cis__ |"2"| CIS Value.
__DeferFeatureUpdates_cis__ |"1"| CIS Value.
__BranchReadinessLevel_cis__ |"2"| CIS Value.
__DeferFeatureUpdatesPeriodInDays_cis__ |"180"| CIS Value.
__DeferQualityUpdates_cis__ |"1"| CIS Value.
__DeferQualityUpdatesPeriodInDays_cis__ |"0"| CIS Value.


# Example Playbook:
---
 - hosts: [win]
   roles:
   - ansible-role-compliance-windows-windows-components-policy-2019


# Author Information:
Richard M. Williams

rmwill@us.ibm.com
