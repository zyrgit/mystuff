# edu.illinois.greendrive


# FusionSuiteSingleton

Sampler, GzipFileWriter, 

() requestSetMyLoc requestShiftMap requestZoomMap requestInitTraceMarkers mapRequestWrite

() initWriter closeWriter 

() initBTDevice initSensors initOBD initGPS 

() setFusionSuiteActivity getFusionSuiteActivity 

() preference set/get 

GPSlocationStr GPS_status trace_marker_initialized 

mainActivity.preference  android_id, bt_addr, obd_vid




# MainActivity

public class PreferencesData, preference

private class Mytask extends TimerTask, Force_quit

() onCreate mWakeLock timer "DATE", mydate appstarttime, HttpUploadThread http_type=3 check meta data, fragmentManager, turnOnBluetooth, checkSelfPermission initWriter  initSensors initOBD initGPS, HttpUploadThread HTTP_TYPE_Get disclaimer load info.

private class btOnClickListener onClick() swap frag

overwrite frag's interface map2activityStr() setting2activityStr()

() callMapJavascript main calls into js 

() changeSettingsTextview callMapReloadUrl() showInfoFragText() showUsageDisclaimer()

() onRequestPermissionsResult initWriter  initSensors initOBD initGPS,

extractLatLngFromStr() util



# Fragments

## MapFragment

public class WebAppInterface web2frag2write() singleton.mapRequestWrite(msg);

mWebView public WebAppInterface web2android; frag2activity

() onViewCreated mWebView.loadUrl reloadMapUrl onBackPressedInMap

() callJavascript 

private class MyWebViewClient extends WebViewClient, shouldOverrideUrlLoading()

private class MyWebChromeClient extends WebChromeClient, onGeolocationPermissionsShowPrompt

public interface FragToActivity map2activityStr()



## SettingFragment

frag2activity bt1user, bt2email, bt3addr, btspin, btcarExtra tv1,tv2,tv3 etuser, etemail, etaddr, etcar; MainActivity.PreferencesData myPreference;

public static String username, email, address, carmake,carmodel,caryear,carclass, carExtra;

spin setOnItemSelectedListener onItemSelected() myPreference.saveString 

() onClick, myPreference.saveString toast, save username, email, address... 

() getSpinIndex setTextview appendTextview



## InfoFragment

tvlist[POStv1]= tv1;  tvlist[POStv0]= tv0;  tvlist[POStv2]= tv2;

timer info_loaded 

() showUsageDisclaimer setTextview appendTextview 



## WebFragment

mWebView frag2activity singleton 

() onBackPressed reloadUrl 

public interface FragToActivity web2activityStr()

MyWebViewClient shouldOverrideUrlLoading() MyWebChromeClient 



## HttpUploadThread

this.file_name = strings[0];
this.user_id = strings[1];
this.http_type = strings[2];

() run_upload run_get doInBackground SharedPreferences delete onPostExecute usage disclaimer block downtime 



## FileUploadService

timer userid Upload_Service_Timeout Filewalker

() precheck file.lastModified() Upload_File_Time_Gap File_Size_Min sharedPrefs Wait_For_Upload

() walk Delete_None_Gz_File Wait_For_Upload HttpUploadThread

() stopAndClear Mysertask



