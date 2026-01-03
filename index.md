<html>
<body>
<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

			embeddedservice_bootstrap.init(
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
	};
</script>
<script type='text/javascript' src='https://hertz--htzeinsbot.sandbox.my.site.com/ESWenUKTNC1765118177157/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>

</body>
</html>
