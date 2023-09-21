
## No Error Code Unable to launch camera in android mobile using the provided React-js code snippet

| **Area** | **Scenario** | **Resolution** |
| -------- | --------- | ----------------|
| Device capabilities | The developer is trying to launch the camera and gallery on both android and iPhone using a React-js code snippet in a Microsoft Teams app. The camera does not open on Android, only the gallery opens without multiple selection, while it works fine on iPhone. | Ensure that the necessary camera and storage permissions are granted on the Android device. Check the app's permission settings and make sure the camera and storage permissions are enabled. If the issue persists, consider debugging the code to identify any potential issues specific to Android. |

## Bad Request - Error in query syntax. The error occurred while trying to get detailed user information using GetUserProfile() in Microsoft Power Virtual Agents Flow Template

| **Area** | **Scenario** | **Resolution** |
| -------- | --------- | ----------------|
| Bots | The developer was trying to get detailed user information using Microsoft Power Virtual Agents in Microsoft Teams. The error occurred when the developer tried to use GetUserProfile() function with the input as 'first(outputs('Search_for_users_(V2)')?['body/value'])?['UserPrincipalName']'. | Ensure that the necessary camera and storage permissions are granted on the Android device. Check the app's permission settings and make sure the camera and storage permissions are enabled. If the issue persists, consider debugging the code to identify any potential issues specific to Android. |


##  Message: Manifest Error   Manifest is invalid due to missing 'name.short' and 'name.full' properties in the localization file

| **Area** | **Scenario** | **Resolution** |
| -------- | --------- | ----------------|
| Developer Portal | The developer was trying to upload the manifest for a Teams app with localization. The Teams app started throwing an error stating that the manifest is invalid due to missing 'name.short' and 'name.full' properties in the localization file. | Add 'name.short' and 'name.full' properties to the localization file. Even if the name of the application is not localizable, these fields are required in the localization file. |



## Area: Device Capabilities
### Error Message: No Error Code   Unable to launch camera in android mobile using the provided React-js code snippet.
### Scenario: The developer is trying to launch the camera and gallery on both android and iPhone using a React-js code snippet in a Microsoft Teams app. The camera does not open on Android, only the gallery opens without multiple selection, while it works fine on iPhone.
### Remediation: Ensure that the necessary camera and storage permissions are granted on the Android device. Check the app's permission settings and make sure the camera and storage permissions are enabled. If the issue persists, consider debugging the code to identify any potential issues specific to Android.

## Area: Bots
### Error Message: Bad Request - Error in query syntax   The error occurred while trying to get detailed user information using GetUserProfile() in Microsoft Power Virtual Agents Flow Template.
### Scenario: The developer was trying to get detailed user information using Microsoft Power Virtual Agents in Microsoft Teams. The error occurred when the developer tried to use GetUserProfile() function with the input as 'first(outputs('Search_for_users_(V2)')?['body/value'])?['UserPrincipalName']'.
### Remediation: Instead of passing in display name, pass in UserID. This way, the call to SearchForUsers() is not needed. Correcting the input to GetUserProfile() function should resolve the issue.


## Area: Developer Portal
### Error Message: Manifest Error   Manifest is invalid due to missing 'name.short' and 'name.full' properties in the localization file.
### Scenario: The developer was trying to upload the manifest for a Teams app with localization. The Teams app started throwing an error stating that the manifest is invalid due to missing 'name.short' and 'name.full' properties in the localization file.
### Remediation: Add 'name.short' and 'name.full' properties to the localization file. Even if the name of the application is not localizable, these fields are required in the localization file.



## Area: Bots
### Error Message: ServiceError   Could not find Connection Setting with name teamsAuth
### Scenario: The developer was trying to add SSO for a notification bot using Teams Toolkit. Despite following the documentation and adding the OAuth connection in the bot, the developer was encountering an error stating that the connection setting 'teamsAuth' could not be found.
### Remediation: Ensure that the OAuth connection name is correctly added to the .env file as mentioned in the documentation. If the issue persists, try using the TeamsBotSSOPrompt function by registering an AAD App for bot authentication. If the problem still persists, consider filing an issue in the TeamsFx repo for further assistance.



## Area: Bots
### Error Message: BadArgument   Unknown attachment type
### Scenario: The developer is trying to attach a PDF file to a Microsoft Teams bot and encounters an error.
### Remediation: The developer should check the sample code for file sharing on MS Teams provided by Microsoft. Additionally, the 'supportsFiles' option needs to be enabled in the manifest for the bot to support file attachments.



## Area: Webhook and Connectors
### Error Message: Error encountered when trying to mention @webhook name in teams.
### Scenario: The developer is trying to invoke Azure functions from Outgoing webhooks in Microsoft Teams. They have created Outgoing webhooks in teams and added their Azure function URL in the callback URL. They have also copied their secret key from webhooks to Azure configuration. However, when they try to mention @webhook name in teams, they encounter an error.
### Remediation: The developer needs to create an HttpTrigger Azure function instead of just an HttpRequest function. They can refer to the provided code for creating an Azure HttpTrigger function. They can also refer to the provided document for more information on Azure functions and bindings.



## Area: Bots
### Error Message: BadArgument   Failed to decrypt pairwise id
### Scenario: The error occurred when attempting to create a conversation between a bot and a user in Teams using the POST request to the https://smba.trafficmanager.net/amer/v3/conversations endpoint.
### Remediation: Verify the values of each parameter in the request, especially the ID given for the member parameter. If the error persists, try executing the request at a different time as it may be a temporary issue.



## Area: Microsoft Graph
### Error Message: PreconditionFailed   PreconditionFailed-ETag mismatch for thread store resource.
### Scenario: The error occurred while trying to create a group chat using the $batch API from MS Team Graph API.
### Remediation: Ensure that you are using the correct POST query while creating the group chat. After creating the group chat, try adding members to the chat using batch operation.



## Area: Apps in Meetings
### Error Message: No specific error code   Session ID changes every time the page is reloaded in the custom app on MS Teams Desktop App.
### Scenario: A custom app in Microsoft Teams Desktop App, which uses Cookies and a session id to keep track of temporary settings for tasks, is experiencing an issue where the session ID changes every time the page is reloaded.
### Remediation: Avoid using cookies in Teams apps as they can cause issues when switching between Desktop and Web or different devices. Instead, store state server-side in a database or other store, keyed on the user's AadObject Id (their unique Azure Active Directory user guid), which remains consistent across all platforms.



## Area: Developer Portal
### Error Message: File not found   The file could not be found in the app package.
### Scenario: The developer is trying to import the 'Hello World' app package to the Developer Portal in Microsoft Teams. However, the import fails with an error message stating that the file could not be found in the app package. The developer has tried both generating the app package using the 'gulp' command and manually creating the app package, but the error persists.
### Remediation: The developer should manually update the color and outline icon file names in the manifest file and check if it works. If the issue persists, the developer should manually create a zip package of color, outline, and manifest file which is in the appPackage folder and check if it works. If the issue still persists, the developer should check the PR #525 for the updated changes.



## Area: Microsoft Graph
### Error Message: No authorization information present   No authorization information present on the request.
### Scenario: The developer is trying to call a simple Graph API from the explorer but is encountering an error even though all required permissions have been granted.
### Remediation: Ensure that there is an admin grant for the required permissions. You can also decode your token at https://jwt.ms/ and check in scopes whether the required permissions are available.



## Area: Bots
### Error Message: The deep link does not save the subEntityId param when clicked in Microsoft Teams chat.
### Scenario: A developer is trying to use a deep link in Microsoft Teams chat, but the subEntityId param is not being saved when the link is clicked.
### Remediation: Ensure that the 'context' is not web encoded. Try using the following format: https://teams.microsoft.com/l/entity/c38259cb-cd15-4797-b634-098bcea43f9a/index1?webUrl=https://google.com/&label=Google&context={"subEntityId":39138959}



## Area: Bots
### Error Message: 412   The server crashes when trying to send a 412 response in the `onInvokeActivity` in the `server/bots/botActivityHandler.js`.
### Scenario: The developer is using Node 16 and npm 8 in the sample app-sso and encounters a server crash when the botAdaptivity attempts to return a 412 response. The bot-builder does not catch and process this exception, causing the app to crash.
### Remediation: Ensure that all required permissions are added and the configuration is correct. Check if admin consent has been granted for your graph API's. Also, consider adding exception handling in the server or elsewhere to catch and process this exception. An issue has been submitted to botbuilder-js and they have added this problem to their backlog.



## Area: Webhook and Connectors
### Error Message: 403   Forbidden error when trying to do an HttpPOST request via a message card, delivered via a Custom Connector.
### Scenario: The developer is trying to create a custom connector for their application in Teams. They are able to post message cards using PostMan, but when they try to post a message card with an Action (HttpPOST) and execute it on the click of a button, they receive a 'Failed to send' message. Further inspection reveals that an API called Execute Action is returning a 403 forbidden error.
### Remediation: Check the permissions for the webhook.site URL. Make sure it is added as an Action URL in the connector developer dashboard and as a valid domain in the connector manifest.json. If the issue persists, try using a different webhook.site as suggested by the Microsoft Teams support.



## Area: Adaptive Card
### Error Message: Unable to render dynamic data inside the AdaptiveCard template for user mentions in Teams.
### Scenario: The developer is trying to create a dynamic AdaptiveCard to mention users in Teams. They are facing an issue with rendering dynamic data inside the template. They have tried to serialize a JSON with the same $data structure with the name of the user mentioned but it doesn't render anything.
### Remediation: Currently, there is no support for sending a dynamic array to the entity property in Microsoft Teams. For mentioning a user, you need to repeat the entity block, not the text block. Refer to the documentation for more details: https://learn.microsoft.com/en-us/adaptive-cards/templating/language



## Area: Microsoft Graph
### Error Message: PS>TerminatingError(Import-Module)   Could not load file or assembly 'System.Management.Automation, Version=7.2.0.0, Culture=neutral, PublicKeyToken=31bf3856ad364e35' or one of its dependencies. The system cannot find the file specified.
### Scenario: The error occurred when a PowerShell script was executed via Intune on devices other than the developer's own. The script was intended to deploy corporate images to each user's workstation for use as Microsoft Teams backgrounds. The script worked fine when executed locally or on the developer's machine, but failed on other laptops when executed through Intune.
### Remediation: 1. Downgrade the PnP Powershell to version 1.12.0 using the commands: 'Uninstall-Module PnP.Powershell' and 'Install-Module -Name PnP.PowerShell -RequiredVersion 1.12.0'. 2. If the script is being run in an Azure DevOps release pipeline, force the PowerShell task to run with PowerShell Core instead of the default V5. This can be done by updating the task settings under Advanced. 3. If the script is being run via Intune, check if there is an option to enforce using PowerShell Core. 4. Alternatively, host the image files on an accessible website and use 'Invoke-WebRequest' to remove the need for interaction with PnP.Powershell.



## Area: Authentication
### Error Message: 403   Google auth on Microsoft Teams mobile app returns 403: disallowed_useragent
### Scenario: The developer is trying to authenticate a Teams app using Google authentication on Android. The authentication process opens a popup but it redirects to an error page.
### Remediation: Ensure that the 'isExternal' parameter and two placeholder values in the existing url parameter are added to the authenticate() API to support external OAuth providers as suggested by Nivedipa-MSFT. If the issue persists, escalate it using the provided link.



## Area: Microsoft Graph
### Error Message: Forbidden   UnknownError
### Scenario: The developer is trying to retrieve messages from a public Microsoft Teams channel that they are not a part of, using Microsoft Graph APIs.
### Remediation: Ensure that the access token has at least ChannelMessage.Read.All permission. If not, add the required permission and try again. Check the functionality in the Graph Explorer first. Note that only team members, owners, or admins can access GET /teams/team-id/ and even admins cannot pull messages from channels they are not part of. This is by design.



## Area: Sideloading
### Error Message: Error while importing the Teams custom app after unzipping, zipping, and re-importing.
### Scenario: The developer is trying to import a Teams custom app. The import works fine if the zip is exported and immediately re-imported. However, if the zip is exported, unzipped on a Mac or Windows computer, then re-zipped and re-imported, it fails.
### Remediation: Ensure that when zipping the files, only the three necessary files (manifest file, color and outline icon file) are selected and zipped. Do not zip the entire folder containing these files as it results in the files being buried in a folder which the dev portal is not expecting.



## Area: Bots
### Error Message: invalid_grant   Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access.
### Scenario: The developer is trying to create a MS Teams chatbot using Python and is having difficulty obtaining the correct access token to read the user's group chat and interact with it. The user has multi-factor authentication enabled.
### Remediation: The developer needs to use interactive flows where user sign in is required. They should modify their code to use 'acquire_token_interactive' instead of 'acquire_token_by_username_password'. Also, they should add a redirect URI as 'http://localhost' in their application.



## Area: Developer Portal
### Error Message: Error converting value "{{variable-name}}" to type 'System.Nullable`1[System.Guid]'. Path 'botId', line 1, position 31.   Cannot use environment variable as Bot ID in Teams App Developer Portal.
### Scenario: The developer is trying to use an environment variable as a bot ID while creating a Teams App manifest using the Developer Portal.
### Remediation: Environment variables are not designed to be used in the GUID field. The developer should directly use the GUID value instead of the environment variable in the bot ID field.



## Area: Authentication
### Error Message: AuthFailed   Failure to get the renewal token from microsoftTeams.authentication.getAuthToken({ }) on app load or for renewal when it expires.
### Scenario: The developer is trying to get the auth token for a personal app using microsoftTeams.authentication.getAuthToken({ }) method. The method is failing often and taking time to get the token. The token is only obtained on browser refresh/retry.
### Remediation: The developer is advised to set 'showLoadingIndicator' to 'false' and remove 'notifySuccess' and 'notifyFailure' calls. This is to simplify the process and avoid confusion between SSO in a tab and the way the 'loading' indicator works.



## Area: Sideloading
### Error Message: 403   Failed to create an app in Azure Active Directory due to insufficient privileges.
### Scenario: A user is trying to upload a custom app through Teams but is encountering an error due to insufficient privileges.
### Remediation: Check if the E3 license includes Microsoft Teams. Ensure the user has either the Application Administrator or Application Developer role assigned. If not, assign one of these roles to the user. There might be a delay after assigning the role, so try again after some time. If the error persists, login with a Microsoft 365 Developer Account. If you don’t have one, consider joining the Microsoft 365 Developer Program.



## Area: Bots
### Error Message: Manifest.json validation errors and meeting join events not getting delivered.
### Scenario: The developer is trying to run a Microsoft Teams bot for meeting events but is encountering validation errors with the manifest.json file. Additionally, the bot is not receiving meeting join events, although chat messages are arriving.
### Remediation: 1. Ensure that the manifest.json file is correctly formatted and adheres to the schema. 2. Check the bot's permissions and scopes to ensure it has the necessary access to receive meeting join events. 3. Refer to the sample provided by Microsoft at https://github.com/OfficeDev/Microsoft-Teams-Samples/tree/main/samples/meetings-events/csharp for guidance. 4. If the issue persists, reach out to Microsoft support for further assistance.



## Area: Developer Portal
### Error Message: 400   App failed to update
### Scenario: The developer is trying to update a bot in the Developer Portal but forgot to identify the bot by selecting an existing bot in the dropdown. When trying to save the changes, an error occurs.
### Remediation: The developer should delete the existing instances and redo the process. This is because the Developer Portal creates a unique app ID and locks the ID for the registered Teams app, preventing duplicate app IDs for multiple apps. In this case, since the existing bot was not selected, the manifest did not update with the commands, causing the error.



## Area: Cards
### Error Message: iOS Teams app not showing card if the card contains a hyperlink with an ampersand.
### Scenario: The developer is trying to display a card in the iOS Teams app that contains a hyperlink with an ampersand. Instead of displaying the card, the app only shows the message 'Sent a card'.
### Remediation: Ensure that the iOS and Teams versions are up to date. If the issue persists, share the card JSON for further investigation. It might be an issue with the way the hyperlink is parsed when it contains an ampersand. As a workaround, try encoding the ampersand in the URL.



## Area: Apps in Meetings
### Error Message: OnTeamsMeetingStartAsync() and OnTeamsMeetingEndAsync() methods are not being called in a specific tenant, but work in a local demo tenant.
### Scenario: The developer is trying to use OnTeamsMeetingStartAsync() and OnTeamsMeetingEndAsync() methods in a specific tenant, but they are not being called. However, these methods work in a local demo tenant.
### Remediation: 1. Confirm that the feature is available in public developer preview. 2. Ensure that 'OnlineMeeting.ReadBasic.Chat' permission is added. 3. Check the configuration of group owner consent settings for RSC in a team using the Azure AD portal. 4. Use Graph explorer to check whether the correct RSC permission is associated with the bot.



## Area: Device Capabilities
### Error Message: 10000 / SIZE_EXCEEDED   The error occurs when users select more than a certain number of images using the microsoftTeams.media.selectMedia function, exceeding the total file size limit of ~30 MB.
### Scenario: The issue arises when users of the custom message extension, particularly on modern Android devices, select more than five images at once. Each image can be over 6MB, causing the function to fail due to the total file size limit.
### Remediation: The platform's size boundaries seem to be limited. You can change the `maxMediaCount` value as mentioned in the code. However, the exact limit may vary depending on the device and the size of the images. The engineering team is investigating ways to counter the platform size limit.



## Area: Developer Portal
### Error Message: Option to disable developer preview no longer exists in the stated menu.
### Scenario: A user enabled the developer preview in Microsoft Teams and later found that the option to disable it no longer exists in the menu. The user was unable to disable the developer preview for a year.
### Remediation: The user should update the Teams version and check again. If the issue persists, the user should connect with the tenant admin to disable the policy. If the issue still persists, the user should reach out to Microsoft 365 Product Support.



## Area: Bots
### Error Message: This action can't be performed since the app does not exist or has been uninstalled.
### Scenario: The developer is creating a Microsoft Teams messaging bot that requires authentication/sign-in. The bot sends a non-reply message to the user that includes a hero card with a sign-in button. When the user receives the hero card and clicks the sign-in button, an error message is displayed.
### Remediation: 1. Ensure that 'token.botframework.com' and 'login.microsoftonline.com' are added in the valid domain section of your app manifest. 2. If you are sideloading the app, be aware that installing/uninstalling the app can be buggy. Try closing and reopening your MS Teams client.



## Area: Developer Portal
### Error Message: 514   SDK Initialization Failed - Please provide instrumentation key
### Scenario: The developer is trying to initialize the Teams SDK in web teams on Chrome browser but it's failing due to missing instrumentation key.
### Remediation: Ensure that you have provided a valid instrumentation key while initializing the SDK. The instrumentation key is required for telemetry data. If you don't have one, you can create it in Azure portal.



## Area: Bots
### Error Message: Error finding key for token   The system is unable to find the key for the token while testing the command bot app.
### Scenario: The developer was testing a command bot app in Microsoft Teams. When they used @mention to send a 'helloWorld' command to the bot, they received no response and encountered an error message in the VSCode terminal stating 'Error finding key for token'.
### Remediation: 1. Ensure that the bot is properly configured and the token is correctly generated. 2. Check if the RSA public key is correctly set up and matches with the token. 3. Make sure all prerequisites and steps are correctly followed as per the given document. 4. Try to reproduce the issue in a different environment or setup to isolate the issue. 5. If the issue persists, consider reaching out to Microsoft Teams Developer Community or escalating the issue via the provided link.



## Area: Bots
### Error Message: 400   Bot is not responding when using app service url as messaging endpoint.
### Scenario: The developer is trying to use a bot with a deployed service url in Microsoft Teams. The bot works fine with ngrok but fails to respond when using the app service url.
### Remediation: Check if any policy is blocking the request from Teams to App service. If so, modify the policy to allow the request. Also, ensure that the domain where your app is deployed is added under the 'validDomains' section of the manifest. If not using SSO, enter a dummy string value in the 'resource' field of the 'webApplicationInfo' section of your app manifest.



## Area: Bots
### Error Message: DEP0005, DEP0018   The bot stopped responding due to deprecation of Buffer() and unhandled promise rejections.
### Scenario: A bot built with Microsoft Bot Framework Node.JS SDK, deployed on a windows server, stopped responding after working well for over a year.
### Remediation: Replace the deprecated Buffer() methods with the new Buffer.alloc(), Buffer.allocUnsafe(), or Buffer.from() methods in your code. Also, handle promise rejections properly in your code to avoid termination of the Node.js process.



## Area: Apps in Meetings
### Error Message: Upload failed File size too large   The file size limit for Adobe eSign feature is 10MB.
### Scenario: The error occurred when trying to attach files over 10MB using the Teams 'Approvals' App for eSignature and Approvals of documents.
### Remediation: Ensure that the file size does not exceed the limit set by Adobe eSign feature, which is 10MB. If larger files need to be attached, consider compressing the files or using a different method to send them.



## Area: Developer Portal
### Error Message: Duplicate file error   Duplicate readme.md files found in different sample paths.
### Scenario: While ingesting sample files, duplicate readme.md files were found under different 'parent' sample paths.
### Remediation: Review the files and determine if they are needed. If not, delete the duplicate files. A PR has been raised to delete the second readme file residing in the /Images/ path. After the changes are pushed to the main branch, check and confirm the changes.



## Area: Bots
### Error Message: Invalid URL   Invoking a Teams chat via DeepLink to external contacts does not work on iOS.
### Scenario: The developer is trying to invoke a Teams chat with external contacts using DeepLink on iOS. The same operation works fine on other platforms like desktop but fails on iOS, returning an 'Invalid URL' error.
### Remediation: Ensure that the URL being used to invoke the chat is correctly formatted and valid. Test the URL on different platforms to verify its functionality. If the issue persists, escalate it using the provided link in the Microsoft Teams Developer Community.



## Area: Adaptive Card
### Error Message: URL with double quotes in Adaptive Card action is not opening in Microsoft Teams on iOS.
### Scenario: A developer is using Logic Apps to generate Actions in an Adaptive Card and pass a URL with double quotes. When the Adaptive Card is sent to Microsoft Teams and the action button is clicked, the URL does not open.
### Remediation: Verify the URL and try with a different URL. Ensure that the URL is properly encoded to handle special characters like double quotes. Test the behavior on different platforms (Teams web, desktop, and iOS) to isolate the issue. If the problem persists, report the issue with all the relevant details for further investigation.



## Area: Authentication
### Error Message: getAuthToken() method returns empty SSO token in success callback.
### Scenario: The developer is trying to fetch the SSO token using TeamsFx React SDK in a SSO Tab app. The token is fetched successfully when running the app using Teams Toolkit or when previewing/publishing the app from the Developer Portal. However, when the app is deployed in Ring0, the SSO token is returned as an empty string.
### Remediation: Check the implementation of the getAuthToken() method. Ensure that the correct ClientId is being used across all environments. Verify the app manifest and app definition in Ring0. If the issue persists, escalate to the engineering team for further investigation.



## Area: Adaptive Card
### Error Message: Adaptive Cards are not fully occupying width in MS Teams Group Channel despite setting the 'width: full' property.
### Scenario: The developer is trying to render Adaptive Cards in MS Teams Group Channel with full width. Despite setting the 'width: full' property, the Adaptive Cards are not occupying the full width.
### Remediation: The issue was fixed by the engineering team and the fix was rolled out to the organization's tenant. The developer should ensure they are using the latest version of MS Teams Desktop and Web version in channel scope.



## Area: Authentication
### Error Message: Manifest Error   Manifest does not contain the RSC permission to allow in-app purchases.
### Scenario: The developer is trying to implement in-app purchases in Microsoft Teams app. The app works fine on a test tenant but shows an error on a normal tenant. The error also occurs on a second account where the in-app purchase popup does not appear.
### Remediation: 1. Validate the manifest using Teams store app validation in the Developer Portal. 2. Follow the v1 implementation guide strictly, remove the planInfo parameter and put a callback function inside instead. 3. Ensure that the in-app purchase is implemented in personal scope as it is currently not supported in channel scope.



## Area: Task Module
### Error Message: Task Module is empty when opened in Teams desktop or web app, but works fine in Teams mobile app.
### Scenario: A chat bot was created to send adaptive cards with buttons that start task modules. However, when these task modules are opened in Teams desktop or web app, they appear empty. The issue does not occur in Teams mobile app.
### Remediation: Check if 'showLoadingIndicator' is set to true in your manifest. If it is, ensure that you have implemented the corresponding protocol for showing the loading indicator as per Microsoft's documentation. If the issue persists, consider debugging your code to identify any potential issues with the task module's implementation.



## Area: Task Module
### Error Message: X-Frame-Options set to 'deny'   The application proxy doesn't work in Teams Desktop Task Module due to login.microsoftonline.com authentication.
### Scenario: The developer is trying to update an app to allow users to open their on-premises sites in the Teams task window using AAD, Enterprise application, Application Proxy and assigned users. The app works fine on mobile and browser but fails on the Desktop application with an error related to 'X-Frame-Options'.
### Remediation: Ensure that the website used is iFramable and is included in the valid domains of the Manifest. Set the Content-Security-Policy header to 'frame-ancestors teams.microsoft.com *.teams.microsoft.com *.skype.com'. For Internet Explorer 11 compatibility, set X-Content-Security-Policy. Alternatively, set the X-Frame-Options header to 'ALLOW-FROM https://teams.microsoft.com/'. Refer to the documentation for tab requirements in Microsoft Teams.



## Area: Bots
### Error Message: Bot is not receiving all channel messages despite having the ChannelMessage.Read.Group RSC permission.
### Scenario: The developer is trying to make a bot receive all channel messages even when not mentioned, as per the documentation. However, the bot is not receiving all messages unless explicitly mentioned. The developer is also facing issues with the structure of 'webApplicationInfo' in Manifest.json and receiving an error when uploading the manifest.json.
### Remediation: 1. Ensure that the manifest version is v1.12 or above. 2. Add 'token.botframework.com' in valid domains. 3. Remove 'orgWide': [], from the authorization section. 4. The bot-id should be given in the 'webapplicationInfo' section. 5. Refer to the sample provided in the link: https://github.com/OfficeDev/Microsoft-Teams-Samples/tree/main/samples/bot-receive-channel-messages-withRSC/csharp and follow the steps.



## Area: Bots
### Error Message: BotNotInConversationRoster   Automatic installation of bot is not working while invoking from message extension.
### Scenario: The developer is trying to automatically install a bot when invoked from a message extension. Despite following the documentation and using an adaptive card with an install button, the bot does not get installed.
### Remediation: 1. Ensure that the bot is correctly configured in the manifest.json file. 2. Check the messaging extension invoke handler in TeamsBot. 3. Verify that the adaptive card is correctly formatted and includes the 'justInTimeInstall' property. 4. Try uploading the app via the Teams admin center instead of sideloading. 5. Test the setup with a different sample to see if the issue persists.



## Area: Bots
### Error Message: Permissions Denied   Permission denied. Ask your IT admin to add this app for you.
### Scenario: The developer is trying to add a transcript bot to a chat or a meeting in Microsoft Teams but is encountering a permissions error.
### Remediation: Check if there is any custom policy set up in admin center for this app which is not allowing it to be added in chat/meeting. Ensure that the options for adding apps to meetings and chats are enabled in the Teams admin center. If all settings are correct, it may take up to 28 days for apps to be fully provisioned. In this case, a manual sync performed by Microsoft support solved the issue.



## Area: Bots
### Error Message: Invalid user identity in provided tenant   The bot encountered an error while sending Adaptive Cards to users outside the host's tenant/organization.
### Scenario: The developer is trying to send an Adaptive Card to each member of a meeting using a notification bot. The bot is able to send the card to the meeting creator but throws an error when trying to send to other members.
### Remediation: The bot can only send Adaptive Cards to users within the host's tenant/organization. Add a condition to check if the member's tenantId matches the conversation's tenantId before sending the Adaptive Card. This will prevent the bot from attempting to send cards to users outside the host's tenant, thus avoiding the error.



## Area: Microsoft Graph
### Error Message: Batch request against /education/user/{userId} endpoint in Microsoft Graph API is not returning a 'value' property.
### Scenario: The developer is running a batch request against the /education/user/{userId} endpoint in Microsoft Graph API and is not receiving a 'value' property in the response.
### Remediation: This is not a bug but a feature of the Microsoft Graph API. When calling endpoints that return a collection, the batch response contains a 'value' property with a collection of objects. However, when calling endpoints that return a single object, like /education/users/{id}, the batch response directly contains the object. No 'value' property is returned in this case.



## Area: Developer Portal
### Error Message: SyntaxError   Cannot use import statement outside a module
### Scenario: The developer is trying to run the Microsoft Teams sample app 'app-hello-world' locally using npm start, but encounters a syntax error related to the import statement.
### Remediation: Add "type": "module", in the package.json file. If the issue persists, follow the steps mentioned in the 'app-hello-world' GitHub sample and refer to the 'Common Issues' section.



## Area: Authentication
### Error Message: unknownAuthError   The error occurs when the `authentication.getAuthToken()` function is called, returning `Error: unknownAuthError`.
### Scenario: The developer is trying to get tokens from the current user logged in on Teams Desktop App using the `authentication.getAuthToken()` function in the Teams SDK. The error occurs when testing on Teams Desktop client (both Windows and MacOS).
### Remediation: There are several possible resolutions. First, proactively check for token expiration and ask the user to login again if the ID token is not valid. Second, catch the error in a callback passed into the acquiretoken ADAL JS function and ask the user to login again if the error occurs. Third, whitelist the login.microsoftonline.com endpoint in your browser extension or re-enable third party cookies in your browser if they are disabled. Lastly, add two client applications to `Authorized client applications` in Azure Portal for the Teams desktop/mobile clients and the web client: `5e3ce6c0-2b1f-4285-8d4b-75ee78787346` and `1fec8e78-bce4-4aaf-ab1b-5451cc387264`.



## Area: Bots
### Error Message: Bot is not responding to command messages in Teams channel without an assigned owner.
### Scenario: The issue occurs when a command message is posted in a Teams channel that was created using the Graph API and does not have an assigned owner. The bot installed in the channel does not respond to the command message.
### Remediation: Ensure that the Teams channel has an assigned owner. This can be done by checking the channel's settings. If the issue persists, it may be due to an intermittent issue with the Graph API. Monitor the situation and report if the issue reoccurs.



## Area: Bots
### Error Message: context.adapter.getSignInLink is not a function   The function 'getSignInLink' is not recognized as a function of 'context.adapter'.
### Scenario: The developer is following a tutorial to implement adaptive cards in a Microsoft Teams bot. The error occurs when trying to use the 'getSignInLink' function with the 'CloudAdapter' class, which is not recognized as a valid function.
### Remediation: The developer should refer to the provided NodeJS sample where the 'CloudAdapter' class is used. If the issue persists, the developer should ensure they are using the latest version of the repository and consider seeking further examples or documentation on how to use the 'getSignInLink' function with the 'CloudAdapter' class.



## Area: Device Capabilities
### Error Message: DOMException: Permission denied   Unable to get audio record in meeting side panel.
### Scenario: The developer is trying to get audio record in the meeting side panel using TeamsFx-Samples and Recorder.js. The code works in meetingChatTab but fails in meetingSidePanel, with no console error but a DOMException: Permission denied in meetingChatTab (web version).
### Remediation: The developer should ensure that they have manually granted permission at a per app level in the web browser as per the instructions in the Microsoft Teams documentation. However, it should be noted that device permissions in the meetings side panel are not yet supported in the General/Public ring.



## Area: Adaptive Card
### Error Message: ReplyToId is coming null when user performs any action on the adaptive card in the emulator.
### Scenario: Developer is testing an adaptive card with yes/no action items in the emulator. When a user clicks on yes/no, the developer wants to update the card with a thank you message. However, the ReplyToId, which is needed for the update, is coming as null.
### Remediation: 1. Verify the version of the Bot Framework Emulator being used. It is recommended to use version V4. 2. Test the adaptive card again in the emulator. 3. If the issue persists, share a screen recording of the issue for further investigation.



## Area: Bots
### Error Message: 401   Unauthorized Error Ngrok
### Scenario: The developer is trying to set up a bot for the C# Sequential Flow Adaptive Card but encounters a 401 Unauthorized Error when trying to call the bot and test a sample incident.
### Remediation: Check the messaging endpoint URL in bot registration and ensure it is correctly set to https://<your_ngrok_url>/api/messages. If the issue persists, try reregistering the AAD app, recreating the bot, and changing the settings from single tenant to multi-tenant.



## Area: Task Module
### Error Message: Unable to load a different TeamsJS app inside of a task module/dialog.
### Scenario: The developer was trying to load another app inside of a different app's tab using a Task Module in Microsoft Teams.
### Remediation: The developer cannot load a different TeamsJS app inside of a task module/dialog. The loading information and context will be based on the manifest of the app that triggered the dialog. Instead, the developer can use Deeplinks instead of tasks.startTask method.



## Area: Developer Portal
### Error Message: Provided add-in package was not understood. Please, make sure that the file being submitted is a valid Office add-in package.
### Scenario: The error occurred while importing an AppStudio app in the Developer Portal in Teams.
### Remediation: 1. Ensure that the Manifest Version is provided in $schema and manifestVersion. 2. Avoid using reserved ids 'about' and 'conversations' for entity id in the manifest. Also, do not specify the 'Name' property if you use reserved ids. 3. Either provide a value for property 'defaultGroupCapability.meetings' or remove it.



## Area: Tabs
### Error Message: Admin Permissions Consent window does not close back after granting or cancelling permissions in the Desktop/ Mac Teams app.
### Scenario: A developer is building a Microsoft Teams Tab application that requires opening the admin permissions consent page within the app. The consent window works fine on the web version of the application, but on the Desktop/ Mac Teams app, the window does not close after granting or cancelling permissions.
### Remediation: 1. Do not mix Teams Tab SSO supports and the idea of having an admin do a pre-consent in the same place. Provide a separate link for admin to pre-consent or rely on the standard SSO experience. 2. Use 'microsoftTeams.authentication.getAuthToken' which handles SSO better than 'authentication.authenticate'. 3. Your redirect page should call the 'notifySuccess(…)' method to close the login screen. 4. Mark your app as 'needs admin pre-approval' and set 'defaultBlockUntilAdminAction' to 'true' and 'publisherDocsUrl' to the page with the instructions for the admin.



## Area: Developer Portal
### Error Message: Package Loading Failure   Provided add-in package was not understood. Please, make sure that the file being submitted is a valid Office add-in package.
### Scenario: The error occurred while trying to import an existing app to the developer portal.
### Remediation: Ensure that you have created a zip folder that does not contain any subfolders. Select the manifest.json, color.png, outline.png and create a zip folder directly. If the issue persists, share your zip folder with the support team for further investigation.



## Area: Bots
### Error Message: Invalid client secret provided   The client secret provided in the GetAuthenticationToken() method is invalid. The secret being sent in the request should be the client secret value, not the client secret ID.
### Scenario: The developer was trying to run a bot and encountered an error in the GetAuthenticationToken() method due to providing an invalid client secret.
### Remediation: Ensure that the client secret value is being used, not the client secret ID. If the issue persists, try creating a new client secret.



## Area: Adaptive Card
### Error Message: Microsoft Teams does not post back the Data property of Action.Submit if it is a string.
### Scenario: The developer is trying to send a Card to Teams with an Action.Submit's Data set to a string. However, Teams does not send it back in the `value` property of the message event. If the Data is an object, then Teams sends it back.
### Remediation: Currently, there is no workaround for this issue. The issue has been raised as a bug and is under investigation. Please monitor the original GitHub issue for updates.



## Area: Authentication
### Error Message: SSO-Token   SSO Token is not getting generated for some users in Azure AD.
### Scenario: The issue occurs when users enter the Una Chat Bot in MS Teams. The SSO Token should be automatically generated for all users, but it's not happening for some.
### Remediation: Update the Teams version and check again. If the issue persists, ensure that the application is correctly registered through Azure Active Directory for SSO. Check the user permissions and roles in Azure AD. If the problem continues, escalate the issue using the provided link.



## Area: Tabs
### Error Message: VM5:2   Failed to execute 'postMessage' on 'DOMWindow': The target origin provided does not match the recipient window's origin.
### Scenario: The developer is trying to initialize a Teams application with a Tab that serves each tenant their own self-hosted version of the app. The initialization fails when trying to redirect to the tenant specific app.
### Remediation: Ensure that all possible domains are listed in the 'validDomains' field of the manifest. Also, experiment with the 'validMessageOrigins' option in 'app.initialize()'. If the issue persists, check if there are any child windows/frames involved in the scenario.



## Area: Adaptive Card
### Error Message: BadSyntax   Failed to read card payload as JSON
### Scenario: The developer is trying to add color to the text in an adaptive card using conditions in a bot that generates adaptive cards into the channel.
### Remediation: First, install the Adaptive Card Templating for JavaScript library. Then, use the 'if' condition to set the color to 'good' and 'attention'. Make sure to use the 'ACData.Template' function on your cardJson before expanding it with your data. Finally, use the resulting 'finalCardJson' to send an adaptive card in the channel or as per your use case.



## Area: Developer Portal
### Error Message: Error while reading manifest.json: root | Required properties are missing from object: ['description.short','description.full']   Manifest parsing has failed due to missing required properties in the manifest.json file.
### Scenario: The developer was trying to upload manifest files for a team extension-based commercial application on Microsoft Teams.
### Remediation: Check the manifest.json file for missing required properties. In this case, 'description.short' and 'description.full' were missing. Update the file with the required attributes and re-upload the manifest zip from Teams App > Manage Apps.



## Area: Microsoft Graph
### Error Message: The 'Get-Team' command in the PowerShell script is not returning any results.
### Scenario: A developer is trying to write a PowerShell script to display all teams in Microsoft Teams software. However, the 'Get-Team' command in the script is not showing any output.
### Remediation: Ensure that the 'Get-Team' cmdlet is used with the correct parameters. The cmdlet supports retrieving teams with particular properties/information, including all teams that a specific user belongs to, all teams that have been archived, all teams with a specific display name, or all teams in the organization. Refer to the official Microsoft documentation for more details: https://learn.microsoft.com/en-us/powershell/module/teams/get-team?view=teams-ps#examples



## Area: Bots
### Error Message: Ext.SetUpBotError   Failed to create an app in Azure Active Directory.
### Scenario: The developer is trying to set up an interactive bot using the sbs-gs-notificationbot.yml file. The process fails at the step of registering the AAD app which is required to create the bot.
### Remediation: 1. Ensure that you have the necessary permissions to create an app in Azure Active Directory. 2. Check the Azure Active Directory setup and configuration. 3. Follow the steps outlined in the 'Set up bot' task documentation at https://aka.ms/teamsfx-debug-set-up-bot-task. 4. If the issue persists, escalate the issue using the link https://aka.ms/DevCommunityEscalationForm.



## Area: Bots
### Error Message: Bot is not receiving all channel messages despite having the ChannelMessage.Read.Group RSC permission.
### Scenario: The developer is trying to receive all channel messages through a bot, which is expected to receive all messages even when not mentioned, as per the ChannelMessage.Read.Group RSC permission. However, the bot is not receiving all messages unless explicitly mentioned.
### Remediation: Ensure that the bot is in Public Developer Preview as this feature is currently available only in this mode. If the issue persists, test the bot using the sample provided at https://github.com/OfficeDev/Microsoft-Teams-Samples/tree/main/samples/bot-receive-channel-messages-withRSC/csharp. If the problem still exists, provide a screen recording of the issue for further investigation.



## Area: Authentication
### Error Message: OAuth token for user authentication is not working on iOS 16.
### Scenario: The developer is using an OAuth token from an HTTP response to authenticate users. The authentication works on Android, desktop, and web platforms, but fails on iOS 16.
### Remediation: 1. Check if the issue is specific to iOS 16 or all iOS versions. 2. Verify if the issue is related to WebKit WebView cookies management. 3. Ensure that the cookie settings are in line with the recommendations in the Microsoft Teams platform documentation. 4. If the issue persists, escalate it using the provided link.



## Area: Authentication
### Error Message: 53001   The error message is about incompatible browsers and authentication failure of a custom Teams app due to Conditional Access policy.
### Scenario: The developer is trying to authenticate a custom Teams app for a customer who has a Conditional Access policy that restricts browsers. The user is presented with a 53001 error and a message about incompatible browsers.
### Remediation: The developer should ensure that the customer is using a domain joined device as the Conditional Access policy requires it. If the device isn't domain joined, it gives a 53001 error. If the issue persists, the developer should check the browser compatibility and update the browser details in the Teams app.



## Area: Bots
### Error Message: BadRequest,Microsoft.Teams.ConfigAPI.Cmdlets.Generated.Cmdlets.SetCsPhoneNumberAssignment_Set   The user 'XXX-XXX-XXX-XXX-XXX' is not found
### Scenario: The developer is trying to assign a phone number to a bot using PowerShell. The error occurs when the developer tries to assign the number to the bot.
### Remediation: 1. Create the application instance without application id. 2. Assign the number. 3. Assign the application id to the application instance. Microsoft is currently working on a fix for this issue.



## Area: Adaptive Card
### Error Message: 209   Invoke validation failed. User forbidden to perform action
### Scenario: The developer is trying to use the 'Refresh' action in an adaptive card in a one-to-one chat in Teams. The action works for the developer but not for the other user in the chat. The error occurs after the Teams cache is cleared and the chat is opened in a browser.
### Remediation: The issue was resolved by adding a bot at the launch of the messaging extension. The bot was not automatically added to the 'groupchat'. The developer used the 'OnTeamsMessagingExtensionFetchTaskAsync' method to check if the app is installed by fetching member information. If the bot is not in the conversation roster, the 'GetAddMissedBotCard' method is called to add the bot.



## Area: Developer Portal
### Error Message: Uncaught SyntaxError SyntaxError: Invalid or unexpected token   An unexpected syntax error occurred while trying to build the React template.
### Scenario: The developer was following the instructions to build a React template for a Teams app. Upon building, an unexpected syntax error occurred, even though no changes were made to the code.
### Remediation: 1. Ensure that the Teams client is updated to the latest version. 2. Check the code for any syntax errors, even if no changes were made. 3. Try to rebuild the app. 4. If the error persists, consider using Teams SDK 2.0 and making necessary changes to the Manifest file. 5. Ensure that the domain of the website is added to the validDomain list in the manifest.



## Area: Bots
### Error Message: 401   Unauthorized access error. All bot interactions are failing with 401 or failing to reach the local server completely.
### Scenario: The developer has completed the setup instructions for the `app-complete-auth` NodeJS example. However, all bot interactions are failing with a 401 error or failing to reach the local server. The bot registration has been configured as UserAssignedMSI and the developer is using an unpaid ngrok account.
### Remediation: Check the ngrok configuration and ensure it is set up correctly. Also, verify the bot registration settings. The bot should be configured as MultiTenant, not UserAssignedMSI. Make sure to use the existing app registration option to create the bot using the app registration ID created in the first chapter of the setup instructions.



## Area: Microsoft Graph
### Error Message: 403   You do not have the required permissions to access this item.
### Scenario: The developer is trying to list tasks for a plan using MS Graph API in a Teams app. The error occurs when a non-admin user tries to access the tasks.
### Remediation: The developer needs to ensure that the user has the necessary permissions to access the tasks. The required permissions are either Tasks.Read, Tasks.ReadWrite, Group.Read.All, or Group.ReadWrite.All. The user must also be a member of the group that the plan belongs to. The developer can test the API using Graph Explorer against their own tenant.



## Area: Task Module
### Error Message: Failed to load web view in Task Module on Android.
### Scenario: The developer implemented an Adaptive Card containing an Image element that uses $data looping, each image given a selectAction that sends a task/fetch activity and data payload. This works fine on web client and iOS, but not on Android.
### Remediation: 1. Check if the Android device is set up for remote debugging. 2. Ensure that the Virtual Device is in Developer Mode, USB and Wireless Debug options are enabled on Device in Developer Options, Remote debug prompts set to always allow, and Developer Preview is enabled on Teams app. 3. Test with different browsers to see if the debug option is coming or not. 4. Configure the logs to debug the application.



## Area: Message Extension
### Error Message: Error encountered while running the msgext-search bot sample, with issues in bot registration and GraphQL resolver error with the 'searchMessageExtension' field path.
### Scenario: The developer was running the msgext-search bot sample in a development environment with Node.js 16 and the latest version of Chrome. Errors were encountered and displayed in the console log, indicating issues with bot registration and a GraphQL resolver error.
### Remediation: Ensure that the bot registration is correctly configured. Follow the steps provided in the Microsoft Teams documentation for setting up a messaging extension search command. Also, check the GraphQL resolver for the 'searchMessageExtension' field path for any errors and correct them. If the problem persists, it may be an intermittent issue and could be reported for further investigation.



## Area: Bots
### Error Message: 0   <BadArgument>Unknown bot
### Scenario: The developer is trying to use a contentBotId from a different tenant in the MS Teams manifest file. When the contentBotId is from the same tenant as the MS Teams domain, it works and loads the data. However, when the contentBotId is from a different tenant, MS Teams does not load anything.
### Remediation: Create a multi-tenant bot using ML Studio before creating the MS bot. Register the application and check the manifest file for the required ContentBotId. Test the URL after app registration into multi-Tenant. If the error still occurs, setup the connection settings under configurations. Add Oauth connection settings to get some kind of authentication for different clients for the same authentication URL. If the issue persists, it might be due to the use of existing AAD instead of creating from Azure bot template. The manually created AAD have email address of user who have created this in Owners section, while AAD created from Azure bot template have 'Bot Framework Dev Portal' user.



## Area: Bots
### Error Message: AADSTS700016   Application with identifier 'Application (client) ID' was not found in the directory 'Bot Framework'.
### Scenario: The developer was trying to run a proactive installation sample app using the client id from Azure bot configuration. The error occurred when the application was not found in the directory 'Bot Framework'.
### Remediation: Verify if the correct client/app id is being used. Ensure that the bot is set up through the CLI and not through the web interface. Confirm if the required Microsoft graph Application-level permissions 'TeamsAppInstallation.ReadWriteForUser.All' have been added. Follow the instructions to add proper ids and secret details in the 'appsettings.json' file. Upload the app at the org level to get 'AppCatalogTeamAppId' and then try to add the app in either personal or team scope. If the error persists, retry the steps by following the guidelines step by step creating a new app id.



## Area: Authentication
### Error Message: CORS   Access to XMLHttpRequest at 'https://login.microsoftonline.com/common/oauth2/v2.0/token' from origin has been blocked by CORS policy.
### Scenario: The developer is trying to enable SSO for a Teams App and is using client-side code to acquire a token using MSAL. The token API is failing due to a CORS issue in both local and development environments.
### Remediation: The 'OnBehalfOf' token call should only be made from a backend server, where CORS would not apply. The only call that needs to be made from the front-end code is 'microsoftTeams.authentication.getAuthToken()'. It is recommended to review the linked video and blog post for a more detailed understanding.



## Area: Tabs
### Error Message: getTabInstances API does not resolve in personal chat and on mobile.
### Scenario: The developer is trying to get Tab information for a personal chat using getTabInstances API, but it never resolves. The same behavior is observed on mobile as well.
### Remediation: The getTabInstances API is not implemented on mobile and it's performance is poor. It is advised not to use it as it will get deprecated. Instead, use the Graph APIs to know what tabs are pinned in a given chat or channel. The links to these APIs are: https://learn.microsoft.com/en-us/graph/api/chat-list-tabs?view=graph-rest-1.0&tabs=http and https://learn.microsoft.com/en-us/graph/api/channel-list-tabs?view=graph-rest-1.0&tabs=http. Keep in mind that using these APIs may require extra permissions on the app registration.



## Area: Adaptive Card
### Error Message: The response from the Teams Adaptive Card is not being recorded in the Azure Logic App.
### Scenario: The developer is trying to capture the input text from a Teams Adaptive Card and use it in their Azure Logic App, but the response is not being recorded.
### Remediation: Ensure to use the 'Post adaptive card and wait for a response' action if you expect a response from the card. The output of this action doesn't give any output options, so you have to format it yourself. Use 'Parse json' and enter input in the expression field: @Outputs('adaptivecardname')?[body]



## Area: Bots
### Error Message: 401   UserNotAuthorizedToGrantResourceSpecificPermission error is received when trying to add bot to a meeting.
### Scenario: The developer implemented a 'Meeting-Attendance-bot' in Azure and tried to add it to a meeting. Despite granting Graph API permissions for the tenant, the bot could not be added due to a UserNotAuthorizedToGrantResourceSpecificPermission error.
### Remediation: Ensure that the required permissions are granted and access is allowed. Refer to the documentation on granting Resource Specific Consent (RSC) permissions. Confirm if the correct sample is being used. Make sure to allow applications to access online meetings on behalf of a user. Check the application access policy setup using PowerShell. Create an application access policy and grant the policy to the user to allow the app ID contained in the policy to access online meetings on behalf of the granted user.



## Area: Bots
### Error Message: 403   CSRF token validation failed
### Scenario: The error occurs when trying to trigger a PATCH request via HTTP AZURE Gateway from Power Virtual Agent BOT to S/4 HANA through OData v2 service. The CSRF token is fetched and stored in a local variable and passed to PATCH request. The error is seen in Power Automate Flow.
### Remediation: The issue is with the Microsoft on-premise-gateway which is used to connect your OData service. The on-premise-gateway always establishes a new HTTP connection that expires the X-CSRF-TOKEN. Wait for a version that supports this or try a different method to connect your OData service.



## Area: Tabs
### Error Message: 100   `registerBeforeUnloadHandler` does not work for mobile devices.
### Scenario: The developer is trying to use `registerBeforeUnloadHandler` and `registerOnLoadHandler` in a custom Teams app on mobile devices. The functions work well on Web and Desktop Teams but not on iOS and Android Teams.
### Remediation: Currently, there is no alternative to `registerBeforeUnloadHandler` for mobile devices and there are no plans to support it in the future. The developer can suggest this feature in the Microsoft Teams Community.



## Area: Bots
### Error Message: Azure Teams Bot stops responding after a few minutes of operation in Teams.
### Scenario: A bot developed for Teams using Azure Bot Service and C# works well in local environment using Bot Framework Emulator, but stops responding after some time in Teams. Uninstalling and reinstalling the bot temporarily resolves the issue but it reoccurs.
### Remediation: Downgrade the .Net version and SDK version to 3.14. Implement a BotJwtRefreshWorker class that refreshes the bot's token every 30 minutes. This ensures that the bot always has a valid token and reduces or eliminates the waiting time.



## Area: Authentication
### Error Message: SDK initialization timed out   The error message indicates that the SDK initialization is timing out when trying to authenticate with Adobe ID in a Teams app.
### Scenario: The developer is trying to implement simple authentication in a Microsoft Teams app using Adobe ID as a third-party OAuth provider. However, an exception is thrown when the 'app.initialize()' function is called, stating that the SDK initialization has timed out.
### Remediation: The developer should confirm the SDK version and MS Teams version being used. They should also try using 'microsoftTeams.app.initialize().then(() => { })' to see if it resolves the issue. If the problem persists, they should check if the sample works with '@microsoft/teams-js 2.7.1' and 'Microsoft Teams Version 1.6.00.2979' as these versions have been confirmed to work without throwing any exceptions or errors.



## Area: Developer Portal
### Error Message: TypeError   Cannot set property closed of #<Readable> which has only a getter
### Scenario: The error occurred when the developer was trying to set up the 'app-hello-world' nodejs sample using a newer version of node.
### Remediation: Downgrade the node version to a compatible one. Alternatively, check for updates or fixes in the restify library that support the newer version of node.



## Area: Bots
### Error Message: Bad Request - Error in query syntax   Error in the GetUserProfile query syntax in Power Virtual Agents Flow Template.
### Scenario: The developer is trying to get detailed user information using Microsoft Virtual Agent in Microsoft Teams. The error occurs when the developer tries to get the user's email by calling SearchForUsers() and then GetUserProfile().
### Remediation: Instead of passing in display name, pass in UserID. This eliminates the need for the call to SearchForUsers().



## Area: Bots
### Error Message: ProvisionError   Failed to provision Developer Portal bot registration.
### Scenario: The error occurred while trying to debug a sample bot project locally using TeamsFx-Samples/share-now. The error was thrown during the 'set-up-bot' task, specifically at the step of 'Registering the bot in Bot Framework Portal'.
### Remediation: The issue was related to a server-side API issue which has been resolved. Verify the local debug experience of Teams Toolkit (TTK) to ensure it's working properly now. Stay updated with the issue on the provided GitHub link for any further updates.



## Area: Microsoft Graph
### Error Message: PreconditionFailed   Failed to execute TeamsGraphService backend request RevokeGroupResourceSpecificPermissionsRequest.
### Scenario: The error occurred when trying to remove a side-loaded application from a Team installation using the Graph API.
### Remediation: Ensure that the Teams app does not have Resource-Specific Consent (RSC) permissions. Installation or removal of apps with RSC permissions is not supported in app-only context. If the app needs to read members of a Team and direct message users in a Team, RSC permissions are not required. Use the bot API to get members of a Team and send 1:1 personal chat messages in Teams.



## Area: Developer Portal
### Error Message: Mgmt.AppCatalog.LOBApp.Upload.BadRequest.Error   Error occurred while adding app manifest to MS Teams admin center.
### Scenario: The developer is trying to add an app manifest to MS Teams admin center but encounters an error.
### Remediation: 1. Update your manifest version to a newer one if you don't need it so old. 2. Ensure your manifest Id and Bot Id are not the same. The Bot Id should be the Azure Application ID for the Bot itself, which you can get from Azure's Bot registration. 3. Review your 'validdomain' entries. They are not typically needed for a bot and are mostly needed for other app types like a Tab app.


