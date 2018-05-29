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
