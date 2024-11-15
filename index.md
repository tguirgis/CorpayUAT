
<html>
<body>

<meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1">

<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

      window.addEventListener("onEmbeddedMessagingReady", e => {
						  embeddedservice_bootstrap.prechatAPI.setVisiblePrechatFields({
						    // List the pre-chat field names with the value and whether
						    // it's editable in the pre-chat form.
						    	"Account_Code": {
						      	"value": "AA123",
						      	"isEditableByEndUser": true
						    	},
		 					"_email": {
						      	"value": "tguirgis@testemail.com.invalid",
						      	"isEditableByEndUser": true
						    	},
							"_firstName": {
						      	"value": "Tony",
						      	"isEditableByEndUser": true
						    	},
		 					"_lastName": {
						      	"value": "Guirgis",
						      	"isEditableByEndUser": true
						    	}
		 				  });
						});

			embeddedservice_bootstrap.init(
				'00DDk00000096DG',
				'NAT_Chat_Web',
				'https://fleetcorna--uat.sandbox.my.site.com/ESWNATChatWeb1730393482019',
				{
					scrt2URL: 'https://fleetcorna--uat.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://fleetcorna--uat.sandbox.my.site.com/ESWNATChatWeb1730393482019/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>


</body>
</html> 
