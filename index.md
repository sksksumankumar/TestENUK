<html>
<body>
<script type="text/javascript">
(function () {
  function initEmbeddedMessaging() {
    try {
      var eb = window.embeddedservice_bootstrap;
      if (!eb) {
        console.error('embeddedservice_bootstrap is not available on window; cannot initialize Embedded Messaging.');
        return;
      }

      eb.settings = eb.settings || {};
      eb.settings.language = 'en_US';

      eb.init(
        '00DSu000004EBvl',
        'enUKTNC',
        'https://hertz--htzeinsbot.sandbox.my.site.com/ESWenUKTNC1765118177157',
        {
          scrt2URL: 'https://hertz--htzeinsbot.sandbox.my.salesforce-scrt.com'
        }
      );
    } catch (err) {
      console.error('Error loading Embedded Messaging: ', err);
    }
  }

  function loadBootstrapScript(src) {
    var s = document.createElement('script');
    s.type = 'text/javascript';
    s.src = src;
    s.async = true;
    s.onload = initEmbeddedMessaging;
    s.onerror = function (e) {
      console.error('Failed to load Embedded Messaging bootstrap script:', src, e);
    };
    (document.head || document.body || document.documentElement).appendChild(s);
  }

  var bootstrapUrl = 'https://hertz--htzeinsbot.sandbox.my.site.com/ESWenUKTNC1765118177157/assets/js/bootstrap.min.js';

  if (document.readyState === 'loading') {
    document.addEventListener('DOMContentLoaded', function () {
      loadBootstrapScript(bootstrapUrl);
    });
  } else {
    loadBootstrapScript(bootstrapUrl);
  }
})();
</script>
</body>
</html>
