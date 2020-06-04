设置为可以实现 取代设备自带的Dialer、Message、Contacts
而实现这些，需要通过配置相应的AndroidManifest-intentfilter的文件
其中Dialer:
<activity >
	<intent-filter>
                <action android:name="android.intent.action.CALL_BUTTON" />
                <category android:name="android.intent.category.DEFAULT" />
            </intent-filter>
            <intent-filter>
                <action android:name="android.intent.action.VIEW" />
                <action android:name="android.intent.action.DIAL" />

                <category android:name="android.intent.category.DEFAULT" />
                <category android:name="android.intent.category.BROWSABLE" />
            </intent-filter>

</activity >

Message :
TODO 20200604 待完善

Contatcs :
TODO 20200604 待完善



