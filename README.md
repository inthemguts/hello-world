Dictionary manifest


<manifest xmlns:android="http://schemas.android.com/apk/res/android" android:versionCode="305" android:versionName="7.5.40" android:installLocation="1" android:compileSdkVersion="29" android:compileSdkVersionCodename="10" package="com.dictionary" platformBuildVersionCode="29" platformBuildVersionName="10">
	<uses-sdk android:minSdkVersion="16" android:targetSdkVersion="29" />
	<uses-permission android:name="android.permission.INTERNET" />
	<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
	<uses-permission android:name="com.android.vending.BILLING" />
	<uses-permission android:name="com.android.vending.CHECK_LICENSE" />
	<uses-permission android:name="android.permission.ACCESS_WIFI_STATE" />
	<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
	<uses-permission android:name="android.permission.WAKE_LOCK" />
	<uses-permission android:name="android.permission.VIBRATE" />
	<uses-permission android:name="android.permission.MODIFY_AUDIO_SETTINGS" />
	<uses-permission android:name="android.permission.FOREGROUND_SERVICE" />
	<uses-permission android:name="android.permission.READ_PHONE_STATE" />
	<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
	<uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" />
	<uses-permission android:name="android.permission.RECEIVE_BOOT_COMPLETED" />
	<uses-permission android:name="com.google.android.finsky.permission.BIND_GET_INSTALL_REFERRER_SERVICE" />
	<uses-permission android:name="com.google.android.c2dm.permission.RECEIVE" />
	<application android:theme="@com.dictionary:style/AppTheme" android:label="@com.dictionary:string/app_name" android:icon="@com.dictionary:drawable/icon" android:name="com.dictionary.util.DailyApplication" android:allowClearUserData="true" android:enabled="true" android:allowBackup="true" android:largeHeap="true" android:supportsRtl="true" android:fullBackupContent="@com.dictionary:xml/backup_descriptor" android:networkSecurityConfig="@com.dictionary:xml/network_security_config" android:roundIcon="@com.dictionary:mipmap/ic_launcher_round" android:appComponentFactory="androidx.core.app.CoreComponentFactory" android:isSplitRequired="true">
		<meta-data android:name="asset_statements" android:resource="@com.dictionary:string/asset_statements" />
		<activity android:theme="@android:style/Theme.NoDisplay" android:name="com.dictionary.deeplink.DeepLinkActivity">
			<intent-filter android:label="Thesaurus" android:autoVerify="true">
				<action android:name="android.intent.action.VIEW" />
				<category android:name="android.intent.category.DEFAULT" />
				<category android:name="android.intent.category.BROWSABLE" />
				<data android:scheme="https" android:host="www.thesaurus.com" />
			</intent-filter>
			<intent-filter android:autoVerify="true">
				<action android:name="android.intent.action.VIEW" />
				<category android:name="android.intent.category.DEFAULT" />
				<category android:name="android.intent.category.BROWSABLE" />
				<data android:scheme="https" android:host="www.dictionary.com" />
			</intent-filter>
		</activity>
		<activity android:theme="@com.dictionary:style/HomeAppTheme" android:name="com.dictionary.activity.HomeActivity" android:launchMode="2" android:screenOrientation="1">
			<intent-filter>
				<action android:name="android.intent.action.VIEW" />
				<category android:name="android.intent.category.DEFAULT" />
				<category android:name="android.intent.category.BROWSABLE" />
				<data android:scheme="https" android:host="15708.measurementapi.com" android:pathPrefix="/serve" />
			</intent-filter>
			<intent-filter>
				<action android:name="android.intent.action.VIEW" />
				<category android:name="android.intent.category.DEFAULT" />
				<category android:name="android.intent.category.BROWSABLE" />
				<data android:scheme="https" android:host="16472.measurementapi.com" android:pathPrefix="/serve" />
			</intent-filter>
			<intent-filter>
				<action android:name="android.intent.action.VIEW" />
				<category android:name="android.intent.category.DEFAULT" />
				<category android:name="android.intent.category.BROWSABLE" />
				<data android:scheme="https" android:host="311809.measurementapi.com" android:pathPrefix="/serve" />
			</intent-filter>
			<intent-filter>
				<action android:name="android.intent.action.VIEW" />
				<category android:name="android.intent.category.DEFAULT" />
				<category android:name="android.intent.category.BROWSABLE" />
				<data android:scheme="https" android:host="311819.measurementapi.com" android:pathPrefix="/serve" />
			</intent-filter>
			<intent-filter>
				<action android:name="android.intent.action.VIEW" />
				<category android:name="android.intent.category.DEFAULT" />
				<category android:name="android.intent.category.BROWSABLE" />
				<data android:scheme="https" android:host="71612.api-01.com" android:pathPrefix="/serve" />
			</intent-filter>
			<intent-filter>
				<action android:name="android.intent.action.VIEW" />
				<category android:name="android.intent.category.DEFAULT" />
				<category android:name="android.intent.category.BROWSABLE" />
				<data android:scheme="https" android:host="53638.api-03.com" android:path="/serve" />
			</intent-filter>
			<intent-filter>
				<action android:name="android.intent.action.VIEW" />
				<category android:name="android.intent.category.DEFAULT" />
				<category android:name="android.intent.category.BROWSABLE" />
				<data android:scheme="https" android:host="131328.api-04.com" android:pathPrefix="/serve" />
			</intent-filter>
			<intent-filter>
				<action android:name="android.intent.action.VIEW" />
				<category android:name="android.intent.category.DEFAULT" />
				<category android:name="android.intent.category.BROWSABLE" />
				<data android:scheme="https" android:host="309017.measurementapi.com" android:pathPrefix="/serve" />
			</intent-filter>
		</activity>
		<activity android:name="com.dictionary.activity.TranslateActivity" android:screenOrientation="1" android:windowSoftInputMode="0x20" android:parentActivityName="com.dictionary.activity.HomeActivity" />
		<activity android:label="@com.dictionary:string/app_name" android:name="com.dictionary.AddOnsActivity" android:launchMode="2" android:screenOrientation="1" />
		<activity android:name="com.dictionary.BlogActivity" android:launchMode="2" android:screenOrientation="1" />
		<activity android:name="com.dictionary.BlogDetailActivity" android:screenOrientation="1" android:configChanges="0x4a0" />
		<activity android:name="com.dictionary.WordOfTheDayDetailActivity" android:screenOrientation="1" android:configChanges="0x20" android:parentActivityName="com.dictionary.activity.HomeActivity" />
		<activity android:name="com.dictionary.WordOfTheDayArchivesActivity" android:screenOrientation="1" />
		<activity android:name="com.dictionary.SettingsActivity" android:launchMode="2" android:screenOrientation="1" android:configChanges="0x580" />
		<activity android:name="com.dictionary.PushSettingsActivity" android:launchMode="2" android:screenOrientation="1" android:configChanges="0x580" />
		<activity android:name="com.dictionary.FavoritesActivity" android:launchMode="2" android:screenOrientation="1" android:configChanges="0x580" android:windowSoftInputMode="0x10" />
		<activity android:name="com.dictionary.RecentsActivity" android:launchMode="2" android:screenOrientation="1" android:configChanges="0x580" android:windowSoftInputMode="0x10" />
		<activity android:name="com.dictionary.About" android:launchMode="2" android:screenOrientation="1" android:configChanges="0x580" />
		<activity android:label="@com.dictionary:string/app_name" android:name="com.dictionary.activity.SearchActivity" android:screenOrientation="1" />
		<activity android:name="com.dictionary.activity.QuizActivity" android:screenOrientation="1" android:configChanges="0x580" />
		<activity android:name="com.dictionary.activity.QuizListActivity" android:screenOrientation="1" android:configChanges="0x580" />
		<activity android:label="WidgetVoice" android:name="com.dictionary.widget.VoiceHandler" android:taskAffinity="com.dictionary.task.widget" android:clearTaskOnLaunch="true" android:excludeFromRecents="true" android:launchMode="2" />
		<activity android:name="com.dictionary.activity.BundlesDetailActivity" android:screenOrientation="1" />
		<activity android:theme="@com.dictionary:style/UpgradeDialogActivityTheme" android:label="@com.dictionary:string/app_name" android:name="com.dictionary.activity.UpgradeDialogActivity" android:launchMode="2" />
		<activity android:name="com.dictionary.WebViewActivity" android:launchMode="2" android:screenOrientation="1" />
		<activity android:theme="@android:style/Theme.Translucent" android:name="com.google.android.gms.ads.AdActivity" android:exported="false" android:configChanges="0xfb0" />
		<activity android:theme="@com.dictionary:style/AppTheme.SplashTheme" android:name="com.dictionary.Splash" android:screenOrientation="1" android:configChanges="0x580">
			<intent-filter>
				<action android:name="android.intent.action.MAIN" />
				<category android:name="android.intent.category.LAUNCHER" />
			</intent-filter>
		</activity>
		<activity android:name="com.mopub.mobileads.MoPubActivity" android:configChanges="0x4a0" />
		<activity android:name="com.mopub.mobileads.MraidActivity" android:configChanges="0x4a0" />
		<activity android:name="com.mopub.common.MoPubBrowser" android:configChanges="0x4a0" />
		<activity android:name="com.mopub.mobileads.MraidVideoPlayerActivity" android:configChanges="0x4a0" />
		<activity android:name="com.mopub.mobileads.RewardedMraidActivity" android:configChanges="0x4a0" />
		<activity android:name="com.dictionary.activity.ClickActionHandlerActivity">
			<intent-filter android:label="clickAction">
				<action android:name="android.intent.action.VIEW" />
				<category android:name="android.intent.category.DEFAULT" />
				<category android:name="android.intent.category.BROWSABLE" />
				<data android:scheme="com.dictionary" android:host="clickAction" android:pathPrefix="/" />
			</intent-filter>
		</activity>
		<activity android:label="Define" android:name="com.dictionary.SerpTabbedActivity" android:screenOrientation="1">
			<intent-filter>
				<action android:name="android.intent.action.PROCESS_TEXT" />
				<category android:name="android.intent.category.DEFAULT" />
				<data android:mimeType="text/plain" />
			</intent-filter>
		</activity>
		<activity android:name="net.hockeyapp.android.UpdateActivity" />
		<activity android:name="com.amazon.device.ads.DTBActivity" android:exported="false">
			<intent-filter>
				<action android:name="android.intent.action.VIEW" />
				<category android:name="android.intent.category.DEFAULT" />
				<category android:name="android.intent.category.BROWSABLE" />
				<data android:scheme="amazonmobile" android:host="intent" />
			</intent-filter>
		</activity>
		<meta-data android:name="com.google.android.geo.API_KEY" android:value="@com.dictionary:string/google_maps_api_key" />
		<meta-data android:name="NEXAGE_MEDIATION_URL" android:value="http://bos.ads0.nexage.com" />
		<meta-data android:name="NEXAGE_DCN" android:value="8a809417014848e5cfccf01d124d0014" />
		<meta-data android:name="com.google.android.gms.version" android:value="@com.dictionary:integer/google_play_services_version" />
		<meta-data android:name="io.fabric.ApiKey" android:value="34f8b2041128ab6909f2e638684b2294cc6af226" />
		<meta-data android:name="com.google.firebase.messaging.default_notification_icon" android:resource="@com.dictionary:drawable/notification_icon" />
		<meta-data android:name="com.google.firebase.messaging.default_notification_color" android:resource="@android:color/transparent" />
		<meta-data android:name="com.google.firebase.messaging.default_notification_channel_id" android:value="@com.dictionary:string/default_notification_channel_id" />
		<meta-data android:name="com.google.android.gms.ads.APPLICATION_ID" android:value="ca-app-pub-5966256865708729~2744469193" />
		<provider android:name="androidx.core.content.FileProvider" android:exported="false" android:authorities="com.dictionary.myfileprovider" android:grantUriPermissions="true">
			<meta-data android:name="android.support.FILE_PROVIDER_PATHS" android:resource="@com.dictionary:xml/file_provider_paths" />
		</provider>
		<provider android:name="com.millennialmedia.internal.utils.MediaContentProvider" android:exported="false" android:authorities="com.dictionary.MediaContentProvider" android:grantUriPermissions="true" />
		<receiver android:label="@com.dictionary:string/widget_name" android:name="com.dictionary.WordWidget">
			<intent-filter>
				<action android:name="android.appwidget.action.APPWIDGET_UPDATE" />
				<action android:name="com.dictionary.action.APPWIDGET_UPDATE" />
			</intent-filter>
			<meta-data android:name="android.appwidget.provider" android:resource="@com.dictionary:xml/widget_word" />
		</receiver>
		<receiver android:name="com.google.android.gms.analytics.AnalyticsReceiver" android:enabled="true" android:exported="false">
			<intent-filter>
				<action android:name="com.google.android.gms.analytics.ANALYTICS_DISPATCH" />
			</intent-filter>
		</receiver>
		<receiver android:name="com.dictionary.util.CustomReferralReceiver" android:exported="true">
			<intent-filter>
				<action android:name="com.android.vending.INSTALL_REFERRER" />
			</intent-filter>
		</receiver>
		<service android:name="com.dictionary.widget.UpdateService" />
		<service android:name="com.google.android.gms.analytics.AnalyticsService" android:enabled="true" android:exported="false" />
		<service android:name="com.google.android.gms.analytics.CampaignTrackingService" />
		<service android:name="com.dictionary.firebase.CustomFirebaseMessagingService">
			<intent-filter>
				<action android:name="com.google.firebase.MESSAGING_EVENT" />
			</intent-filter>
		</service>
		<uses-library android:name="org.apache.http.legacy" android:required="false" />
		<service android:name="com.google.android.gms.analytics.AnalyticsJobService" android:permission="android.permission.BIND_JOB_SERVICE" android:enabled="true" android:exported="false" />
		<activity android:theme="@android:style/Theme.Translucent.NoTitleBar" android:name="com.google.android.gms.auth.api.signin.internal.SignInHubActivity" android:exported="false" android:excludeFromRecents="true" />
		<service android:name="com.google.android.gms.auth.api.signin.RevocationBoundService" android:permission="com.google.android.gms.auth.api.signin.permission.REVOCATION_NOTIFICATION" android:exported="true" />
		<service android:name="com.google.firebase.components.ComponentDiscoveryService" android:exported="false" android:directBootAware="true">
			<meta-data android:name="com.google.firebase.components:com.google.firebase.remoteconfig.RemoteConfigRegistrar" android:value="com.google.firebase.components.ComponentRegistrar" />
			<meta-data android:name="com.google.firebase.components:com.google.firebase.storage.StorageRegistrar" android:value="com.google.firebase.components.ComponentRegistrar" />
			<meta-data android:name="com.google.firebase.components:com.google.firebase.analytics.connector.internal.AnalyticsConnectorRegistrar" android:value="com.google.firebase.components.ComponentRegistrar" />
			<meta-data android:name="com.google.firebase.components:com.google.firebase.iid.Registrar" android:value="com.google.firebase.components.ComponentRegistrar" />
			<meta-data android:name="com.google.firebase.components:com.google.firebase.abt.component.AbtRegistrar" android:value="com.google.firebase.components.ComponentRegistrar" />
		</service>
		<service android:name="com.google.android.gms.tagmanager.TagManagerService" android:enabled="true" android:exported="false" />
		<activity android:name="com.google.android.gms.tagmanager.TagManagerPreviewActivity" android:exported="true" android:noHistory="true">
			<intent-filter>
				<data android:scheme="tagmanager.c.com.dictionary" />
				<action android:name="android.intent.action.VIEW" />
				<category android:name="android.intent.category.DEFAULT" />
				<category android:name="android.intent.category.BROWSABLE" />
			</intent-filter>
		</activity>
		<service android:name="com.google.firebase.messaging.FirebaseMessagingService" android:exported="false">
			<intent-filter android:priority="-500">
				<action android:name="com.google.firebase.MESSAGING_EVENT" />
			</intent-filter>
		</service>
		<activity android:theme="@com.dictionary:style/Theme.MMTransparent" android:label="@com.dictionary:string/mmadsdk_app_name" android:name="com.millennialmedia.internal.MMActivity" android:configChanges="0x2004" />
		<activity android:label="sdk" android:name="com.millennialmedia.internal.MMIntentWrapperActivity" android:configChanges="0x2004" />
		<receiver android:name="com.quantcast.measurement.service.QCReferrerReceiver" android:exported="true">
			<intent-filter>
				<action android:name="com.android.vending.INSTALL_REFERRER" />
			</intent-filter>
		</receiver>
		<activity android:label="OtherName" android:name="com.quantcast.measurement.service.AboutQuantcastScreen" />
		<provider android:name="com.crashlytics.android.CrashlyticsInitProvider" android:exported="false" android:authorities="com.dictionary.crashlyticsinitprovider" android:initOrder="90" />
		<service android:name="com.liulishuo.filedownloader.services.FileDownloadService$SharedMainProcessService" />
		<service android:name="com.liulishuo.filedownloader.services.FileDownloadService$SeparateProcessService" android:process=":filedownloader" />
		<activity android:theme="@com.dictionary:style/OT.AppTheme.Transparent" android:name="com.onetrust.otpublisherssdk.OTPublishersSDKActivity" android:configChanges="0x580" />
		<provider android:name="androidx.work.impl.WorkManagerInitializer" android:exported="false" android:multiprocess="true" android:authorities="com.dictionary.workmanager-init" android:directBootAware="false" />
		<service android:name="androidx.work.impl.background.systemalarm.SystemAlarmService" android:enabled="@com.dictionary:bool/enable_system_alarm_service_default" android:exported="false" android:directBootAware="false" />
		<service android:name="androidx.work.impl.background.systemjob.SystemJobService" android:permission="android.permission.BIND_JOB_SERVICE" android:enabled="@com.dictionary:bool/enable_system_job_service_default" android:exported="true" android:directBootAware="false" />
		<service android:name="androidx.work.impl.foreground.SystemForegroundService" android:enabled="@com.dictionary:bool/enable_system_foreground_service_default" android:exported="false" android:directBootAware="false" />
		<receiver android:name="androidx.work.impl.utils.ForceStopRunnable$BroadcastReceiver" android:enabled="true" android:exported="false" android:directBootAware="false" />
		<receiver android:name="androidx.work.impl.background.systemalarm.ConstraintProxy$BatteryChargingProxy" android:enabled="false" android:exported="false" android:directBootAware="false">
			<intent-filter>
				<action android:name="android.intent.action.ACTION_POWER_CONNECTED" />
				<action android:name="android.intent.action.ACTION_POWER_DISCONNECTED" />
			</intent-filter>
		</receiver>
		<receiver android:name="androidx.work.impl.background.systemalarm.ConstraintProxy$BatteryNotLowProxy" android:enabled="false" android:exported="false" android:directBootAware="false">
			<intent-filter>
				<action android:name="android.intent.action.BATTERY_OKAY" />
				<action android:name="android.intent.action.BATTERY_LOW" />
			</intent-filter>
		</receiver>
		<receiver android:name="androidx.work.impl.background.systemalarm.ConstraintProxy$StorageNotLowProxy" android:enabled="false" android:exported="false" android:directBootAware="false">
			<intent-filter>
				<action android:name="android.intent.action.DEVICE_STORAGE_LOW" />
				<action android:name="android.intent.action.DEVICE_STORAGE_OK" />
			</intent-filter>
		</receiver>
		<receiver android:name="androidx.work.impl.background.systemalarm.ConstraintProxy$NetworkStateProxy" android:enabled="false" android:exported="false" android:directBootAware="false">
			<intent-filter>
				<action android:name="android.net.conn.CONNECTIVITY_CHANGE" />
			</intent-filter>
		</receiver>
		<receiver android:name="androidx.work.impl.background.systemalarm.RescheduleReceiver" android:enabled="false" android:exported="false" android:directBootAware="false">
			<intent-filter>
				<action android:name="android.intent.action.BOOT_COMPLETED" />
				<action android:name="android.intent.action.TIME_SET" />
				<action android:name="android.intent.action.TIMEZONE_CHANGED" />
			</intent-filter>
		</receiver>
		<receiver android:name="androidx.work.impl.background.systemalarm.ConstraintProxyUpdateReceiver" android:enabled="@com.dictionary:bool/enable_system_alarm_service_default" android:exported="false" android:directBootAware="false">
			<intent-filter>
				<action android:name="androidx.work.impl.background.systemalarm.UpdateProxies" />
			</intent-filter>
		</receiver>
		<provider android:name="com.google.android.gms.ads.MobileAdsInitProvider" android:exported="false" android:authorities="com.dictionary.mobileadsinitprovider" android:initOrder="100" />
		<receiver android:name="com.google.android.gms.measurement.AppMeasurementReceiver" android:enabled="true" android:exported="false" />
		<receiver android:name="com.google.android.gms.measurement.AppMeasurementInstallReferrerReceiver" android:permission="android.permission.INSTALL_PACKAGES" android:enabled="true" android:exported="true">
			<intent-filter>
				<action android:name="com.android.vending.INSTALL_REFERRER" />
			</intent-filter>
		</receiver>
		<service android:name="com.google.android.gms.measurement.AppMeasurementService" android:enabled="true" android:exported="false" />
		<service android:name="com.google.android.gms.measurement.AppMeasurementJobService" android:permission="android.permission.BIND_JOB_SERVICE" android:enabled="true" android:exported="false" />
		<receiver android:name="com.google.firebase.iid.FirebaseInstanceIdReceiver" android:permission="com.google.android.c2dm.permission.SEND" android:exported="true">
			<intent-filter>
				<action android:name="com.google.android.c2dm.intent.RECEIVE" />
			</intent-filter>
		</receiver>
		<activity android:theme="@android:style/Theme.Translucent.NoTitleBar" android:name="com.google.android.gms.common.api.GoogleApiActivity" android:exported="false" />
		<provider android:name="com.google.firebase.provider.FirebaseInitProvider" android:exported="false" android:authorities="com.dictionary.firebaseinitprovider" android:initOrder="100" />
		<service android:name="androidx.room.MultiInstanceInvalidationService" android:exported="false" />
		<meta-data android:name="com.android.vending.splits.required" android:value="true" />
		<meta-data android:name="com.android.vending.splits" android:value="@com.dictionary:xml/splits0" />
		<meta-data android:name="com.android.vending.derived.apk.id" android:value="8" />
	</application>
</manifest>
