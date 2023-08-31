# cordova-plugin-allow-notifications

To allow you to set add to Manifest.xml the uses-permission tag


So I totally biffed on the fact that edit-config is now supported in config.xml as well as plugin.xml so you don't need the above plugin. All you need to do is add an edit-config section to your config.xml file like this:

<platform name="android">
    <edit-config file="AndroidManifest.xml"
                 target="/manifest/application"
                 mode="merge">
        <application android:allowBackup="false"/>
    </edit-config>
</platform>

