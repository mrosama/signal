# websignal
chrome://settings/content
//for ssl
<link rel="manifest" href="/manifest.json" />
<script src="https://cdn.onesignal.com/sdks/OneSignalSDK.js" async=""></script>
<script>
  var OneSignal = window.OneSignal || [];
  //OneSignal.log.setLevel('trace');
  OneSignal.push(function() {
    
    OneSignal.SERVICE_WORKER_PARAM = { scope: '/' };
    OneSignal.init({
      appId: "9caa036f-8bac-48b3-bc31-f92b5a8112d2",
       path: '/mrosama/',
    });
  });


***************************mainCode

  var OneSignal = window.OneSignal || [];
  OneSignal.push(function() {
    OneSignal.init({
      appId: "9caa036f-8bac-48b3-bc31-f92b5a8112d2",
    });

      OneSignal.getUserId(function(userId) {
    console.log("OneSignal User ID:", userId);
    // (Output) OneSignal User ID: 270a35cd-4dda-4b3f-b04e-41d7463a2316    
  });
               
  OneSignal.getUserId().then(function(userId) {
    console.log("OneSignal User ID:", userId);
    // (Output) OneSignal User ID: 270a35cd-4dda-4b3f-b04e-41d7463a2316    
  });
  
  });


  **********************************************