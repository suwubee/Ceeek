GETTING STARTED

## Installing Support Board

+   [PHP](#)
+   [WordPress](#)
+   [Cloud](#)

To install the PHP version of Support Board on your server follow the steps below:

+   Open the archive **supportboard X.X.X.zip** and extract the folder in a server location of your choice.
+   Navigate to the link **http://\[your-site\]/supportboard/admin.php** and complete the installation. Replace \[your-site\] with with your website URL. If you change the directory name, replace **supportboard** with the new directory name.
+   Once the installation is complete, log in with the email and password you created in the previous step and you're done!

[![](https://board.support/media/play-video.svg)](https://www.youtube.com/watch?v=md-1ZiLRPMQ)

#### Display the chat

To display the chat on your website include the following scripts into the **<head></head>** or **<footer></footer>** area of each page where the chat is shown.

                                        <!-- Not required if jQuery is already loaded -->
                                        <script src="\[SUPPORT-BOARD-URL\]/js/min/jquery.min.js"></script>
                                        <script id="sbinit" src="\[SUPPORT-BOARD-URL\]/js/main.js"></script>
                                    

Replace **\[SUPPORT-BOARD-URL\]** with the URL of your Support Board installation, get it from **Settings > Miscellaneous > Support Board URL**. E.g. https://example.com/supportboard/js/main.js.

#### URL parameters

+   **lang=LANGUAGE-CODE** See the [multilingual](#multilingual) docs for more details.
+   **url=APP-URL** Use this parameter if your application directory URL / folder has been changed. Replace APP-URL with the FULL URL of the application folder. You can also define the URL via JavaScript: **var SB\_INIT\_URL = "APP-URL"**.

#### Site migration

If you migrate the chat to a new domain / URL you need to edit the **config.php** file (it's in the Support Board folder) and update the **SB\_URL** constant with the new URL.

#### Minify JS

For performance reasons, you may want to load the minified main.js file: **\[SUPPORT-BOARD-URL\]/js/min/main.min.js**. Please note that if you contact us for support you will need to load again the non-minified version.

To install the WordPress version of Support Board on WordPress follow the steps below:

+   Go to the **Plugins** page and click **Add new** then **Upload plugin** and upload the file **supportboard 1.2.3.zip**.
+   Once the installation is complete you should see a new left menu item named **Support Board** .
+   You're done, the chat is automatically shown on all pages.

If you want to show the chat on another website, follow the steps of the **PHP installation**.  

[![](https://board.support/media/play-video.svg)](https://www.youtube.com/watch?v=UnF-BiyNl0Y)

To display the chat on your website go to [https://cloud.board.support/account/?tab=installation](https://cloud.board.support/account/?tab=installation) and copy the embed code, then paste it into your website pages. If you are using WordPress, you can download the Support Board Cloud plugin [here](https://wordpress.org/plugins/support-board-cloud/).

* * *

#### Requirements

+   Your web project must support HTML and PHP, and pages containing the chat must be opened via a web browser.
+   You cannot display the chat on a HTML page opened directly on a local computer. Use a local server like Xampp instead.
+   Your server must allow the access of the following file: **supportboard/include/ajax.php**
+   If you're using the WordPress version of Support Board and you have any security plugins installed, please make sure that they don't block the **supportboard/include/ajax.php** file.
+   JQuery 1.1+
+   PHP 7.4+
+   In your server settings, **CURL**, **ZIP ARCHIVE**, must be enabled and working correctly.
+   Read and write file permissions must be granted for the Support Board **uploads**, **resources/language** and **apps** folders. Support Board must be able to save and read the files in these folders.
+   MySQL 5.5+
+   MySQL - The SQL mode "ONLY\_FULL\_GROUP\_BY", and the setting "ANSI\_QUOTES", must be disabled.
+   All Support Board folders should have 755 permissions, all Support Board files should have 644 permissions.

Once the installation is completed you can check the system requirements from **Settings > Miscellaneous > System requirements**.

* * *

## Activation

To activate Support Board and enable all of the features (including updates and more secure encryption), you need to enter the Envato purchase code in **Admin > Settings > Miscellaneous**.

#### Apps installation

To download, install, and activate the apps go to the **Settings > Apps** area of Support Board and enter the Envato purchase code or license key.

[Find your Envato purchase code](https://help.market.envato.com/hc/en-us/articles/202822600-Where-Is-My-Purchase-Code-)

* * *

## Updates

+   To update Support Board and the apps, enter the admin area and click on the version number in the lower left corner.
+   You can also activate automatic updates via **Settings > Miscellaneous**.
+   To enable the updates, you need to have a valid Envato purchase code. To update the Support Board apps you need to have a separate valid License Key or Envato purchase code for each specific app. Besides, the License Key must not be older than 1 year (only for apps purchased outside of CodeCanyon). If your License Key is expired, you will need to purchase a new license to enable App updates again. Apps purchased on CodeCanyon have lifetime updates.
+   The latest versions of the apps may not work if Support Board has not been updated to the latest version.
+   If you're using the WordPress version of Support Board , keep in mind that you cannot update Support Board from the WordPress plugins page.

#### Manual updates

To manually update Support Board and the apps go to [https://board.support/synch/manual.php](https://board.support/synch/manual.php).

* * *

## Optimal configuration

Support Board is a powerful tool, but its abundance of features can pose a challenge when it comes to quick setup. To streamline the process, we provide a list of the most commonly used features that we advise setting up. By incorporating all these features, you will have access to the most essential and beneficial functionalities.

+   Activate email notifications from **Settings > Notifications**. Make sure to activate the following options: **Agent email notifications**, **Sounds admin > Incoming conversations and messages**, and **Push notifications** (if you are using the cloud version, push notifications are already active). For more information on how notifications work, you can click [here](#notifications).
+   Configure the SMTP server under **Settings > Notifications > SMTP**. Afterwards, test the email feature by sending a trial email from **Settings > Notifications > Send an agent email notifcation**. In case you are using the cloud version, the Support Board SMTP is already activated, but you may want to use your own anyway.
+   Navigate to **Settings > Messages** and set up the [follow-up message](#follow-up-message) and [offline message](#offline-message).
+   If you are using the WP or PHP version of Support Board, activate [Pusher](#pusher). In case you are using the cloud version, Pusher is already activated.
+   Navigate to **Settings > Miscellaneous > Performance optimization** and turn off any features that are not being used.
+   In case you are utilizing the chatbot, make sure to check out the optimal configuration [here](#optimal-configuration-ai).
+   If you are facing difficulties in synchronizing services like Google or WhatsApp, our team can help you by configuring them. For further information, please visit our [hire us](https://board.support/hire-us) page. By utilizing your personal accounts such as Google or Facebook, you can enjoy free credits, free quotas, and significantly lower costs compared to other chat services. Additionally, you will have full control and transparency over your data and expenses.

* * *

## Having Problems?

If you're having any issues at all, please contact our support team via the chat widget on right of this page. Before contacting us, please make sure that your server has all the requirements listed above.

#### General issue

For any issue you can check the system requirements from **Settings > Miscellaneous > System requirements**. We can not provide support about solving the issues reported by the system requirement function, please contact your hosting or server support if you need help.

#### Blank screen when accessing the admin area

+   Check if the browser console has error (on Chrome you can open it from **Settings > More tools > Developer tools > Console**).
+   Enable the PHP debug and check the PHP error logs.
+   If you have the WordPress version, disable all security plugins and plugins related to your hosting.

#### Cross-domain configuration

If you want to use the same chat installation on multiple domains, your server should allow cross-origin requests. To enable cross-origin requests on your server follow the steps below:

#### Cross-domain configuration via server

+   **For Apache servers** — Edit the **.htaccess** file of the domain where the plugin is installed and enter the code **<IfModule mod\_headers.c>Header set Access-Control-Allow-Origin "\*"</IfModule>** or **<IfModule mod\_headers.c="">header('Access-Control-Allow-Origin: \*');</IfModule>** at the very top of the file. To make it works you need to have at least **AllowOverride +FileInfo** or **AllowOverride All** in the Apache config.
+   **For nginx servers** — Edit the file **/etc/nginx/nginx.conf** of the domain where the plugin is installed and enter the code **add\_header Access-Control-Allow-Origin "\*";** at the very top of the file. If you're using Plesk go to **Domains > example.com > Apache and nginx settings > Additional nginx directives** and insert  
    **add\_header 'Access-Control-Allow-Origin' '\*';**.[](https://board.support/media/docs/plesk-1.jpg)
+   **For OpenLiteSpeed servers** — Visit [https://openlitespeed.org/kb/setting-up-cors-on-openlitespeed/](https://openlitespeed.org/kb/setting-up-cors-on-openlitespeed/).

You can view tutorials for the most common server administration software in the list below:

+   [Plesk](https://support.plesk.com/hc/en-us/articles/115001338265-How-to-set-up-CORS-cross-origin-resource-sharing-in-Plesk-)
+   [All Apache servers](https://enable-cors.org/server_apache.html)

#### Cross-domain configuration via PHP

If none of the previous solutions work or you can't change the server settings, follow the steps below:

+   Edit the file **supportboard/config.php** and enter the code **define('SB\_CROSS\_DOMAIN', true);** at the end of the file.
+   Upload the following folders into your destination domain(the domain where the chat should be shown, not the one where Support Board is installed): **supportboard/media/fonts** and **supportboard/media/icons**. You can upload the files where you want, for example, **http://www.example.com/chat-files**. If the chat is loaded on multiple domains upload the files on each domain.
+   Edit again the file **supportboard/config.php** and Enter the code **define('SB\_CROSS\_DOMAIN\_URL', 'YOUR-URL');** at the end of the file. Replace **YOUR-URL** with the URL that points to the files you just uploaded, for example, **http://www.example.com/chat-files**. If the chat is loaded on multiple domains replace **YOUR-URL** with the an array of URLs, for example, **\["http://www.example.com/chat-files", "http://www.example-2.com/chat-files"\]**.

#### Unable to install an app

Your server/hosting has file and folder permissions issues, or a firewall is blocking our website. You can verify it from **Settings > Miscellaneous > Check Requirements** (keep in mind that even if it's all green, you still have a server problem, it just isn't caught by the requirements checks). You can solve the issue by installing the apps manually. Go here for the manual installation: [https://board.support/synch/manual.php](https://board.support/synch/manual.php)

#### Blocking zoom on iOS devices

When using the chat on iPhones the textarea is automatically zoomed when the user's start typing a new message. To stop the zoom Enter the code below into the **<head>** area of all the pages that include the chat.

                                <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1.0, user-scalable=no" />
                            

#### Hide admin.php from URL

By default, the admin URL is something like **https://your-website.com/support/admin.php**. You can hide the **admin.php** part of the URL and make it like **https://your-website.com/support/** by inserting the following code in your **.htaccess** file:

                                    <ifmodule mod\_dir.c> DirectoryIndex admin.php</ifmodule>
                                

#### Chat widget not displaying

The chat may not be showing due to the following reasons.

+   You cannot see and test the chat as a user if you're logged-into the admin area. To test the chat as a user, please log out of your admin account or from WordPress. Alternatively, you can use another browser window in "private" or "incognito" mode. Additionally, you can force a logout by executing the SBF.reset() function in the browser console.
+   You may not see the chat because you have disabled it in the settings area. To fix this, visit the settings section and deselect all options related to that: **Chat > Manual initialization**, **Chat > Login initialization**, **Chat > Hide chat outside of office hours**, **WordPress > Manual initialization**.
+   You're trying to access the chat from a domain, or subdomain, different from the one of the installation. Details [here](#cross).

#### Conversations are not visible to administrators or agents

The conversations may not be showing due to the following reasons.

+   The agent has been given a department, yet the conversations have not been assigned to that specific department.
+   One or more of the following settings have been activated: **Miscellaneous > Routing**, **Miscellaneous > Queue**, **Miscellaneous > Hide conversations of other agents**
+   You are using the WordPress version and the setting **WordPress > Multisite routing** has been activated.
+   You are using the chatbot and the setting **Artificial Intelligence > Human takeover** has been activated.

For cases 1, 2, and 3, make sure to log in with the correct admin/agent or check your admin/agent profile to ensure that there are no departments assigned. In case 4, please check the archived conversations.

#### Reset email or password of the admin account

If you can no longer log in to the admin area you can reset your password and email by following the steps below:

+   Edit your **MySQL Database**. You can edit it from your hosting panel, usually with **phpMyAdmin**.
+   Edit the table **sb\_users**.
+   Find your admin account, and make sure the value of the column **user\_type** is **admin**.
+   Reset your password by editing the **password** column and by inserting the new password as a hash. To generate a hash for your password, visit [https://phppasswordhash.com/](https://phppasswordhash.com/), or Enter the hash **$2y$10$i7OComVhUh8BHcyx9VzUfuN.hnNsnKzK1Hd/GKK2KIwBo7Y6stppu** (password: 12345678).
+   Reset your email address from the column **email**.

If you're using the WordPress version, you can delete the user from the database and WordPress will generate it again. You can also create a new WordPress user with administrative privileges, then logout from your current account, and log in with the new one. Once you're into Support Board , change the password of your previous agent from **Users > Agents**.

If you encounter the "Too many login attempts. Please retry again in a few hours." error, click [here](#ip-ban).

#### Admin account deleted

If you have accidentally deleted all your admin and agent accounts and you can no longer log in to the admin area, you can resolve this issue by following the steps below:

+   Edit your **MySQL Database**. You can edit it from your hosting panel, usually with **phpMyAdmin**.
+   Edit the table **sb\_users**.
+   You can convert any existing user to an admin by editing the column **user\_type**, and entering the value **admin**.
+   You can also add a new user by assigning a value to the columns first\_name, last\_name, password, email, and user\_type fields. The value of the password column must be a hash. To generate a hash for your password, visit [https://phppasswordhash.com/](https://phppasswordhash.com/). Also, the value of the column **user\_type** must be **admin**.

#### Server down

If your server and/or website goes down or suddenly stops working after a few minutes of chat usage, the issue could be related to your server's Firewall. This usually happens as a result of an IP Address Banning (Fail2Ban) or Web Application Firewall (ModSecurity) settings. The multiple AJAX requests from the chat to the database are recognized as a "server attack" and so your server places a temporary block on your IP address. This issue should only affect you and/or your developers; visitors/users should not be affected. To confirm whether or not this is the issue, use a VPN service like [Hotspot Shield](https://www.hotspotshield.com/). When the server goes down, activate the VPN to change your IP and try accessing your website again. If the website works normally, the issue is confirmed. To solve it temporarily disable fail2ban or contact your hosting support for additional support.

#### Disable chat via JS

Enter the code **var SB\_DISABLED = true;** into a page to prevent the chat from loading.

* * *

CONVERSATIONS

## Manage Conversations

Conversations have a total of four different statuses: **mark as read**, **archive**, **delete** and **restore**. You can manage the status of a conversation by opening it in the conversations area and then clicking any of the corresponding icon buttons in the top right of the conversation window.

#### Search for conversations

You can for conversations by department ID, assigned agent ID, conversation title, conversation ID, message text, message attachments name, user first name, user last name, user email

#### Information

+   When you empty the **trash**, all the conversations in the trash are permanently deleted.
+   When a user sends a new message to an archived or trashed conversation, the conversation is automatically restored and will now be visible in the **Inbox area**.
+   Trashed conversations are deleted automatically after 30 days.
+   When a user is deleted, all the conversations and messages are permanently deleted too.
+   An agent can delete their messages by opening the message menu and clicking **Delete**. The message menu becomes visible when you hover the mouse cursor over the message.

* * *

## Text Editor and Automated Messages Features

The text editor of the admin area and automated messages(example: welcome and subscribe messages) can be used to create stylized messages:

+   Links formatting — All text links are automatically converted to clickable hyperlinks.
+   Text formatting — The editor also supports text formatting syntax:
    +   To make text **bold**, surround it with **\***: \*your text\*.
    +   To make text *italic*, surround it with **\_\_**: \_\_your text\_\_.
    +   To make text strikethrough, surround it with **~**: ~your text~.
    +   To insert a **single-line code** comment, surround it with**\`**: \`your text\`.
    +   To insert a `code block`, surround it with **\`\`\`**: \`\`\`your text\`\`\`.
+   HTML and other code languages — For security reasons, no HTML, JavaScript (JS), or other code languages are permitted. However, you can use HTML snippets by utilizing custom rich messages (discussed below).
+   To insert a line break into a message, use the keyboard combination **SHIFT + ENTER** or **CTRL + ENTER**.

* * *

#### Merge fields

Merge fields are strings replaced by external values when used. Merge fields can be used in any message or automated message, including chatbot messages.

* * *

| Code | Description |
| --- | --- |
| 
{user\_name}

 | Full name of the active user. |
| 

{user\_email}

 | Email of the active user. |
| 

{agent\_name}

 | Full name of the active agent. |
| 

{agent\_email}

 | Email of the active agent. |

* * *

## Rich Messages

Rich messages are special messages with interactive features like buttons, dropdowns, or inputs. They allow an agent to request information from the user via a user input form or to diplay interactive contents. Rich messages can be inserted into a chat message using shortcodes. Shortcodes accept various parameters like title and description. The available rich messages are listed below.

#### How it works:

* * *

1

### Create and send

![Rich message](https://board.support/media/docs/rich-message-1.jpg) Create a rich message by inserting the shortcode into the text editor of the admin area. Customize all of the parameters with your information and send your message.

2

### Message is displayed

![Rich message](https://board.support/media/docs/rich-message-2.jpg) When a shortcode is used, the user sees the rich message (not the shortcode) and can select or enter the required information to complete the form submission.

3

### User's response is submitted

![Rich message](https://board.support/media/docs/rich-message-3.jpg) Once the rich message form has been filled out and sent by the user, a success message is shown and the form data is saved.

* * *

#### Rich Messages

* * *

| Name | Shortcode | Description |
| --- | --- | --- |
| Card | 
\[card image="URL" header="TITLE" description="Lorem ipsum dolor sit amete" link="URL" link-text="Purchase" extra="$599" target="\_blank"\]

 | Call-to-action card with an image, title, description, link, and more. |
| Slider | 

\[slider image-1="URL" header-1="TITLE" description-1="Lorem ipsum dolor sit amete" link-1="URL" link-text-1="Purchase" extra-1="$599" image-2="URL" header-2="TITLE" description-2="Lorem ipsum dolor sit amete" link-2="URL" link-text-2="Purchase" extra-2="$599" target="\_blank"\]

 | Slider of call-to-action cards with an image, title, description, link, and more. You can add up to 10 slides. |
| Slider images | 

\[slider-images images="URL,URL,URL"\]

 | Slider of images. |
| Chips | 

\[chips options="A,B,C"\]

 | List of buttons. |
| Buttons | 

\[buttons options="A,B,C"\]

 | List of buttons. |
| Select | 

\[select options="A,B,C"\]

 | Dropdown list of options. |
| Inputs | 

\[inputs values="A,B,C" button="Send now"\]

 | List of text inputs. |
| Email | 

\[email name="true" last-name="true" phone="true" phone-required="false" placeholder=""\]

 | Form to collect the user's email and phone number. All attributes are optional. Follow up settings used as default values. Add the attribute **required-messaging-apps="true"** to force users to provide their email and phone on messaging apps. [Merge fields](#merge-fields) are supported. |
| Registration | 

\[registration\]

 | Registration form. |
| Timetable | 

\[timetable\]

 | Timetable. |
| Articles | 

\[articles link="https://board.support/articles-demo"\]

 | Articles with search area. The **link** attribute is used as fallback message for Facebook Messenger, WhatsApp, Telegram messages. |
| Rating | 

\[rating label-positive="Helpful" label-negative="Not helpful" label="Rate and review" success-negative=""\]

 | Agent rating form. To make the rating shortcode work on WhatsApp, Messenger, Telegram you need to use Dialogflow and the chatbot, create a new **Intent** with **rating** as **input Context**, nothing as **output Context**, a list of the user's most common messages for a positive rating as **Training phrases**(e.g. good, positive) and **{ "rating": 1, "force-message": true }** as **Custom Payload** response. For the negative rating create a new intent with same context but replace the training phrases and the custom payload to **{ "rating": -1, "force-message": true }** [](https://board.support/media/docs/rating-intent.jpg). The shortcode must include also a **title** or **message**. |
| List | 

\[list values="A,B,C"\]

 | Text list. |
| List double | 

\[list values="A:X,B:Y,C:Z"\]

 | Text list with titles. |
| List image | 

\[list-image values="URL:A,URL:B,URL:C"\]

 | Text list with titles and images. |
| Table | 

\[table header="A,B,C" values="A:B:C,A:B:C,A:B:C"\]

 | Table. |
| Button | 

\[button link="https://board.support" name="Click here" target="\_blank" style="link"\]

 | Display a link or open an article. The attribute **target="\_blank"** is optional and open the link in a new window. The attribute **style="link"** is optional and change the button design. To open an article on click the link value must be **#article-ID**, replace ID with the article ID. |
| Video | 

\[video type="youtube" id="0TImic4N1ko" height="350"\]

 | Display a YouTube or Vimeo video. The value of the attribute **type** can be **youtube** or **vimeo**. The attribute **id** is the ID of the video, get it from the URL. The attribute **height** is optional and sets the video height in px. |
| Image | 

\[image url="https://board.support/media/admin.png"\]

 | Image. |
| Share | 

\[share fb="https://board.support/" tw="https://board.support/" li="https://board.support/" pi="https://board.support/" wa="https://board.support/"\]

 | Social share buttons. |

* * *

#### Commas

If your texts include commas you need to replace all commas with the characters **\\,**.

* * *

#### Global parameters

All of the rich messages support the following parameters:

* * *

| Parameters | Description |
| --- | --- |
| 
id="123"

 | The ID of the rich message (used also to save the JSON data). |
| 

title="ABC"

 | The rich message title. |
| 

message="ABC"

 | The rich message description that appears underneath the title. |
| 

success="ABC"

 | The message that appears when the user completes and sends the rich message. The user input is appended to this message. |
| 

settings="ABC"

 | Extra field for optional extra values. |

* * *

#### Rich message response

When a user completes a rich message, the response data is saved in JSON format in the database under table **sb\_messages** and column **payload**. Example:

{"rich-messages":{"4Voyu":{"type":"email","result":{"email":\["example@gmail.com","Your email..."\]}}}}

* * *

#### Rich message translations

To translate a rich message string, the original rich message text must be in english, add the exact english text and its translations in **Setting > Translations > Front End**.

* * *

#### Custom rich messages

You can create custom rich messages with your own custom content by going to **Settings > Miscellaneous**. Currently, custom rich messages are static and there are no interactive options available as there are with shortcodes. However, you can insert custom HTML codes.

* * *

#### HTML codes

When creating a custom rich message, you can use the following codes:

* * *

| Code | Description |
| --- | --- |
| 
<a href="https://www.google.com" target="\_blank" class="sb-rich-btn sb-btn">Click here</a>

 | Link with button design. |
| 

<a href="https://www.google.com" target="\_blank" class="sb-rich-btn sb-btn-text">Click here</a>

 | Link. |
| 

<div class="sb-image"><img src="https://via.placeholder.com/1500x600" class="sb-image" /></div>

 | Image that zoom on click. |

* * *

## Built-in messages

The built-in messages are pre-programmed messages sent automatically by Support Board. You can find them by going to **Settings > Messages**.

#### Offline message

Notify the user when their message is sent outside of the scheduled office hours or or all agents are offline.

+   [Text formatting](#text-editor) is supported.
+   [Merge fields](#merge-fields) are supported.
+   To learn more about the office hours option, please click [here](#office-hours).
+   The offline message is sent to the same user maximum 1 time per hour.
+   If the chatbot's [human takeover](#human-takeover) is active, the offline message is not sent. Instead, it is only sent when human takeover is initiated.
+   If you or any other agent is online using [Slack](#slack), the offline message will not be sent.

#### Privacy message

Present a privacy message accompanied by Accept and Decline buttons. The user's approval by clicking on the Accept button is required to start using the chat. This feature ensures privacy policy enforcement and GDPR compliance.

+   The privacy message is not shown if the **Require registration** option has been enabled.
+   The privacy message is also sent to messaging channels like WhatsApp, but the user does not have the option to approve or decline the privacy policy. The messaging functionalities are not blocked either. The message is sent after the user initiates the conversation by sending their first message.

#### Pop-up message

Show a pop-up notification to all users.

+   The popup message is always shown until the user manually closes it; then it stays closed.

#### Welcome message

Send a message to new users when they visit the website for the first time.

+   [Text formatting](#text-editor) is supported.
+   [Merge fields](#merge-fields) are supported.
+   [Rich messages](#rich-messages) are supported.
+   The welcome message is not sent to slack.
+   Conversations containing only the welcome message (and no response) are automatically archived.

#### Follow up message

If no agents respond within the specified time interval, a message will be sent to request the user's details, such as their email.

+   [Text formatting](#text-editor) is supported.
+   [Merge fields](#merge-fields) are supported.
+   If the **delay** is not set, a dynamic time interval is utilized and it is determined as follows: If **Settings > Miscellaneous > Office hours** is configured, and the current time falls within the defined office hours, or if at least one agent is online, then the delay will be set to 15 seconds. In all other cases, the delay will be set to 5 seconds.
+   Follow-up messages are sent a maximum of once every 24 hours.
+   If the user provides an email address and the [newsletter](#newsletter) feature is enabled, the email address will be subscribed.
+   The follow-up message is sent only to users without email address.

#### Subscribe message

If no agents respond within the specified time interval, a message will be sent to request the user's details, such as their email.

+   [Text formatting](#text-editor) is supported.
+   [Merge fields](#merge-fields) are supported.
+   If the user provides an email address and the [newsletter](#newsletter) feature is enabled, the email address will be subscribed.
+   The subscribe message is sent only to users without email address.

* * *

## Attachments

The allowed file attachments extensions are set in the supportboard/include/upload.php file. The following image formats are displayed automatically:.jpg,.jpeg,.png.

Add new allowed file extensions by adding the code **define("SB\_FILE\_EXTENSIONS", \["exe", "abc",...\])** to the **config.php** file of your Support Board installation folder. Replace \["exe", "abc",...\] with an array containing the extensions you want to allow.

For instructions on sending attachments with a chatbot, click [here](#dialogflow-info).

* * *

## More information

Here, you can access information regarding a variety of features associated with conversations.

#### Tags

Tags enable more efficient organization and grouping of conversations. Please refer to the information below for further details.

+   Tags can be assigned to conversations through different methods: via the admin area by navigating to **Settings > Automations > More**, through [Dialogflow actions](#dialogflow-actions), and by inserting the JS variable **SB\_DEFAULT\_TAGS** into a page showing the chat or into a web page displaying the chat or the tickets panel.
+   To locate conversations with specific tags, simply enter the tag names into the search bar located at the top-left corner of the admin conversations area, or you can select the desired tag from the dedicated filters menu on top-left.
+   You can disable the tags from **Settings > Admin > Disable tags**.

* * *

USERS

## Manage Users

Manage users from the **Users area** in the left menu of the admin area.

* * *

#### Search users

You can search users by name, surname, email, and custom fields.

#### Delete users

You can delete a user by opening the **User edit box** and then clicking **Delete user**. To delete multiple users at once, select the users you want to delete from the Users table and then click the top right **Delete icon**.

+   When a user is deleted, all of their conversations and messages are automatically deleted permanently.
+   The conversation attachments will be deleted permanently. If [AWS S3](#aws) is enabled, also the AWS S3 files will be deleted.
+   If a user of a deleted user come back to the website, a new user is automatically created.
+   Visitors are automatically deleted every 24 hours.

#### Additional user table columns

To display additional columns in the user table go to **Settings > Admin > Users table additional columns** and add the new columns. The value of each column is the slug of the user detail or extra user detail you want to display. The slug is lowercase and with spaces replaced by the char **\-**. For example, the slug of the extra user detail "Date of birth" is "date-of-birth".

#### User types

* * *

| Type | Description |
| --- | --- |
| 
user

 | A "user" is any user with an email. |
| 

lead

 | A "lead" is any user with no user details, who is automatically registered, and with at least one conversation. |
| 

visitor

 | A "visitor" is any user who has not started a conversation. Note: Visitors are automatically deleted every 24 hours. |

* * *

## Manage Agents and Admins

Manage, create, and delete agents and admins from the **Users area**.

+   Configure agents' privileges and permissions from **Settings > Admin > Agent privileges**.
+   It can create a supervisor from **Settings > Admin > Supervisor**. The Supervisor is a special agent with specific privileges, it must be an administrator. You can add multiple supervisors by adding comma separated admin IDs.
+   To create an agent or ad admin, go to the **users** area and click the button **Add user** on the top right.
+   Only agents and admins can log in the Support Board admin area.
+   When you activate the Support Board plugin on WordPress, an admin account is automatically created using the same username and password as the currently logged-in user.

* * *

## Registration Form

The registration form is a pre-chat form that requires the user to enter specific information before starting the chat.

+   You can use the registration form as a pre-chat form by limiting the information requested to the user to only the user's email address or the user name, for example.
+   The log-in form is shown only if the registration password field is shown.
+   The password field is always shown when the user system is set to "WordPress".
+   If **Settings> Users > Allow Duplicate Emails** is enabled and a user enters an already registered email, a new user is created and the email is removed from the old user. The new user will not have access to the old user's messages and conversations. You can also automatically log in a user via [URL parameters](#url-parameters).

* * *

## Information

+   New users are automatically displayed in the user table in real time.
+   To view online users enable **Settings > Users > Register all visitors**.
+   To receive the online user notification you have to enable **Settings > Miscellaneous > Pusher** and **Settings > Users > Register all visitors**. The feature covers all user types, including visitors and leads. However, notifications are only sent upon a user's initial visit to the website. Subsequent visits do not activate the notification.
+   Agents and admins can set their status to online or offline from the bottom-left profile panel. The offline status is activated automatically when the agent or admin has been inactive in the admin area for at least 10 minutes. Inactivity is defined as not performing any mouse clicks, movements, or key presses. The automatic offline status feature is not enabled on mobile devices. For this feature to work correctly, [Pusher](#pusher) should be enabled.

* * *

SETTINGS

## Settings

* * *

## Office Hours

You can set the office hours timetable from **Settings > Miscellaneous > Office hours**. Office hours are used for:

+   Sending the [offline message](#offline-message).
+   Disabling and hiding the chat during out-of-office hours.
+   Disabling the chatbot during regular office hours and enabling it during out-of-office hours.

#### More information

+   Blank values in the timetable settings are considered out-of-office hours.
+   The office hours are in UTC format. Your UTC is generated automatically when you click the field **Settings > Miscellaneous > UTF offset.** To manually get the UTC offset of your area, go to: [https://browserspy.dk/](https://browserspy.dk/date.php) or [wikipedia.org/wiki/List\_of\_UTC\_time\_offsets](https://en.wikipedia.org/wiki/List_of_UTC_time_offsets) and copy the offset (e.g. for UTC −12:00, enter -12). Only integers are accepted. If your offset is not an integer (e.g. UTC -12:30 or UTC -12:45), try searching for an alternative UTC offset. If you can't find an integer offset, you will need to manually adjust the times in the office hours table to fix the gap.
+   The date and time format of the timetable matchs automatically the one used in the country of the browser language of the user.

* * *

## Knowledge Base Articles

Knowledge base articles provide instant answers to customers to help reduce customer support volume. To manage the articles, go to **Settings > Articles**. Articles support HTML code, which can be used to add images, videos, and other content. Here are some HTML code examples that you can use:

| Name                  | Code                                                                                                                                                                                                                                             |
|-----------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Button                | `<a href="https://www.google.com" target="_blank" class="sb-rich-btn sb-btn">Click here</a>`                                                                                                                                                       |
| Image                 | `<img src="https://via.placeholder.com/1500x600" />`                                                                                                                                                                                              |
| Image with lightbox   | `<div class="sb-image"><img src="https://via.placeholder.com/1500x600" class="sb-image" /></div>`                                                                                                                                                  |
| Video                 | `<video controls><source src="video.mp4" type="video/mp4"></video>`                                                                                                                                                                               |
| YouTube and Vimeo     | Enter the **embed code** provided by YouTube or Vimeo                                                                                                                                                                                             |


#### Display articles

+   The articles can be shown in the chat dashboard by enabling them from the **Settings > Chat** area.
+   The articles can be shown in a dedicated page by inserting the code **<script>var SB\_ARTICLES\_PAGE = true;</script>** into any page showing the chat. To set the location of the articles area Enter the code **<div id="sb-articles" class="sb-loading"></div>**. If you're using the WordPress version you can use the shortcode **\[sb-articles\]**.
+   Alternatively, articles can be shared via the rich message shortcode, **\[articles\]**.

[![](https://board.support/media/play-video.svg)](https://www.youtube.com/watch?v=SqZso0ouUPQ)

#### More information

+   Translate the categories from **Settings > Translations** by adding the translation name and its translation. The original translation name must be in English.
+   If you use categories, all the articles must be assigned to a category.
+   If there is at least one translated article in the user's language, only the translated articles are displayed.
+   If some block is not saved, e.g. text block, disable all browser extentions and try again.
+   Articles are synchronized automatically with the Dialogflow knowledge base if the Dialogflow app is installed.
+   You can create an internal chat link to an article with the [button rich message](#rich-messages).
+   You can create a link to a specific article with the URL attribute **article=ID**, replace **ID** with the article ID. Example: [https://board.support/articles-demo?article=Ucsx6](https://board.support/articles-demo?article=Ucsx6).
+   You can create a link to an article category with the URL attribute **category=ID**, replace **ID** with the category ID. Example: [https://board.support/articles-demo?category=LnNaZ](https://board.support/articles-demo?category=LnNaZ).
+   The articles are always included into the training of your [OpenAI](#open-ai) chatbot.

* * *

## Language and Translations

Support Board is fully multilingual and provides powerful features to detect the user's language on the fly.

#### Edit translations

To edit the languages of both chat and admin, go to **Settings > Translations**. Some settings, such as e-mail contents, are directly translatable and therefore do not need to be translated here.

#### Chat language

Support Board is already translated into 41 languages. There are many options available to set the language:

+   **OPTION 1** Go to **Settings > Chat** and check the **Translate automatically** option. This feature will automatically use the chat language of the user's browser or the language saved in the user profile.
+   **OPTION 2 - PHP ONLY** Add the URL parameter **lang=LANGUAGE-CODE** to the script that loads the chat, replacing "LANGUAGE-CODE" with the two-letters language code you would like to display. E.g. **https://board.support/supportboard/js/main.js?lang=en**.  
    This feature will force the chat to always use the same language and the option **Chat > Translate automatically** will be ignored. Go to [wikipedia.org/wiki/List\_of\_ISO\_639-1\_codes](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for the complete languages code list (see column 639-1).
+   **OPTION 2 - WORDPRESS ONLY** Go to **Settings > WordPress** and set the option **Force language**. This feature will force the chat to always use the same language and the option **Chat > Translate automatically** will be ignored.
+   **OPTION 3 - WORDPRESS ONLY** The WordPress version of Support Board uses the default language of the WordPress installation; or the language of the current page or post if the website is multilingual. This feature is compatible with WPML, Polylang, and other multilingual plugins. This feature is automatically disabled if the option **Chat > Translate automatically** is active.

#### Admin language

To translate the admin area follow the steps below:

+   Translate the texts in your language from the **Settings > Translations**.

To set the admin area language you have three options:

+   Activate the option **Settings > Admin > Automatically translate admin area**. This feature automatically translate the admin area to match the agent profile language or the agent browser language.
+   Edit the file **config.php** inside your Support Board installation directory and Enter the code **define('SB\_ADMIN\_LANG', 'LANGUAGE-CODE');** at the end of the file content. Replace **LANGUAGE-CODE** with the language code of the language you want to use, use only 2 letters, for example, insert only **es**, not **es\_ES**.

#### Translate custom contents

You can translate almost any custom content like [rich messages](#rich-messages), titles, descriptions, automatic messages, chat header, and more. To include translations, visit **Settings > Translations** and click on the **New translation** button. Then, enter the English content you wish to translate in the first field and its corresponding translation in the second field. The original text must be in English. If you have the artificial intelligence app you can also translate all contents to any language automatically through the [multilingual via translation](#multilingual-via-translation) feature.

#### Add a new language

To add a new language, follow the steps below:

+   Via FTP or a File Manager, go to **supportboard\\resources\\languages\\front**.
+   Duplicate (copy and paste it in the same directory) the **supportboard\\resources\\languages\\front\\source.json** file.
+   Rename the file with the language code you would like to add. Go to [wikipedia.org/wiki/List\_of\_ISO\_639-1\_codes](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) for the complete languages code list (see column 639-1).
+   Go to **Settings > Translations** and the new language should appear automatically.

To add a new language for the admin area, follow the exact same steps, but use folder **admin** instead. New languages will not be lost or deleted on plugin updates.

#### Information

+   If a translation string is missing, add it by clicking the button **Add new translation**.
+   If a translation string is not working, make sure to remove all white spaces and break lines at the start and the end of the string.
+   The translations edits are not saved in the database but directly in the translation files. When a translation is edited, and saved, a backup is created into the **uploads** folder. The backup is restored automatically on plugin update and plugin activation.
+   Some special chars like **&** are replaced by the HTML equivalent code (see [https://www.w3schools.com/html/html\_entities.asp](https://www.w3schools.com/html/html_entities.asp)). Ex. **&** is replaced by **&amp;**.
+   You can add missing translation strings also by code. Edit the language files located in **supportboard\\resources\\languages**. After editing a file, the new strings will be visible under **Settings > Translations**. Remember to click **Save changes** in order to preserve your translations and avoid losing them when Support Board is updated.

* * *

## Departments

Departments give you the power to distribute conversations and assign various agents to specific departments. For example, you can create a department entitled "Sales" and assign specific conversations to that department. To start using departments, follow the steps below:

+   Go to **Settings > Miscellaneous** and add, delete and manage the departments. After saving, reload the page.
+   Go to **Users > Agents** and edit an agent, you will see a new field where you can set the department of the agent.
+   Reload the page and you're done! In the **Conversations area**, you will now see an option to set the department.

#### Settings

+   **Display in dashboard** Displays the departments' list in the chat dashboard and force users to choose a department before starting a conversation.
+   **Display images** Displays the department image instead of the department color.
+   **Label** Replace the label **Departments** (plural) with another text. The name is displayed in the admin and tickets area.
+   **Label single** Replace the label **Department** (singular) with another text. The name is displayed in the admin and tickets area.
+   **Dashboard title** Set the title of the chat dashboard list. Default: Departments.

#### How it works

+   Agents and admins can only access conversations, users, and agents that have been assigned to their specific department.
+   When an agent is assigned to a new department, an email notification is sent to all of the agents assigned to the new department.
+   The **General department** is global and gives agents access to all of the conversations within all departments. Also, all agents without a department are automatically assigned to the General department.
+   To automatically assign a department to the user conversations you can Enter the JavaScript variable **var SB\_DEFAULT\_DEPARTMENT = ID;** into the pages where the chat is displayed, replace ID with the department ID. For more details check the APIs [here](https://board.support/docs/api/use-cases#auto-departments).
+   Admins with no assigned department always see the conversations of all departments.
+   The chatbot can assign a department to the active conversation via [Dialogflow actions](#dialogflow-actions).

#### How to assign a department

You can assign a department to a conversation in several ways:

+   Via **Settings > Miscellaneous > Departments settings > Display in dashboard**. This setting will force the user to choose a department when starting a new conversation.
+   Via **Settings > Automations > More**.
+   Via JavaScript the variable **var SB\_DEFAULT\_DEPARTMENT = ID;**. Enter the code into the pages where the chat is displayed and replace ID with the department ID. For more details check the API [here](https://board.support/docs/api/use-cases#auto-departments).
+   Via [API](https://board.support/docs/api/js).

* * *

## Queue

When the queue is activated via **Settings > Miscellaneous > Queue**, users enter into a queue automatically when an agent's chat limit is reached. When a user enters the queue, a message with the current position in the queue and the estimated waiting time is displayed. Support Board automatically assigns the conversations to all available agents proportionately. When an agent marks a conversation as completed (by archiving it), the queue is updated and a new conversation is received.

#### More information

+   Only online agents are counted as "available" agents.
+   Only online agents will receive new conversations.
+   Admins are not included; admins always see all the conversations.
+   Agents must archive a conversation to mark it as completed; this will automatically give them access to the next conversation in the queue.
+   Agents can switch their status between online and offline by hovering over their profile image and then clicking the label of the profile pop-up at the bottom-left of the admin area.
+   Agents can only view their conversations; however, they can see all of the conversations of a single user.
+   Agents can only search and filter their conversations.
+   The waiting time is displayed in minutes and is calculated as follows: queue position X response time = waiting time. For example, if a user is 5th in the queue, and the response time has been set to 4 minutes (via Settings > Miscellaneous > Queue), then the total wait time displayed to the user will be 20 minutes.
+   If a user is in the queue and leaves (e.g. by closing the browser) for more than 1 minute, the conversation is saved; however, once the user comes back, the queue is reset and the user will lose their previous position. If the user leaves, the conversation remains unassigned and therefore invisible to agents, but only visible to admins.
+   To enable agents to view all unassigned conversations, activate **Settings > Miscellaneous > Hide conversations of other agents** and **View unassigned conversations**.
+   The queue is compatible with the departments.
+   If Dialogflow human takeover is active, the queue is activated only on human takeover.
+   For conversations started from messaging apps like WhatsApp, it is not possible to respect the limit of conversations per agent, all conversations will be immediately and proportionally assigned to an agent.
+   Use the [offline message](#offline-message) to prevent the chat from showing the queue update message to the user.
+   When the sound option is active, a sound is played when it's the user's turn.

#### How to test the queue

+   To simulate multiple users and agents, open the chat in multiple different browsers (e.g. Opera, Firefox, Brave, Chrome, etc.). Each browser can simulate two users/agents: one in normal mode and one in "private" or "incognito" mode.
+   To reset the chat and start a new user session, open the browser console, enter **SBF.reset()**, and press **ENTER**.

* * *

## Routing

When the routing is activated via **Settings > Miscellaneous > Routing**, Support Board automatically assigns the users conversations to all available agents proportionately.

#### Information

+   Conversations are assigned to online agents first. If all agents are offline, conversations are assigned proportionally between all agents.
+   Conversations are assigned to agents with less active conversations. A conversation is active if it's not deleted, or archived. If routing is active, you should archive the conversations once completed.
+   Admins are not included; admins always see all the conversations.
+   Agents can switch their status between online and offline by hovering over their profile image and then clicking the label of the profile pop-up at the bottom-left of the admin area.
+   Agents can view only their conversations; however, they can see all of the conversations of a single user.
+   Agents can search and filter only their conversations.
+   The routing is compatible with the departments.
+   When routing is active agents can manually route conversations to other agents from the right panel of the conversations area.
+   If the conversation is archived and the user reopens it in the future by sending a new message, if the assigned agent in the conversation is offline, the conversation is assigned to another agent.

* * *

## Manual routing

When the routing is activated via **Settings > Miscellaneous > Hide conversation of other agents** agents see only their own conversations and can select the unassigned ones.

+   **Agents menu**: displays the agents' menu to assign the active conversation to another agent.
+   **Routing if offline**: if the conversation is archived and the user reopens it in the future by sending a new message, if the assigned agent in the conversation is offline, the conversation is assigned to another online if there is at least one, otherwise to no agent.
+   **View unassigned conversations**: allow agents to view the unassigned conversations, when an agent replies the conversation is automatically assigned to him and the conversation is removed in real-time from the admin area of the other agents. Check this option to enable the manual routing.

* * *

## Email piping

Email piping lets you, your agents, and your users reply to chat messages via email.

#### Activation

To activate the email piping go to **Settings > Notifications > Email piping** and enter your POP3/IMAP email server information, then set the email address to use for the email piping in **Settings > Notifications > SMTP** and you're done! The email address must be the one to which the email piping server connects to. Support Board will send all emails from this email address and you, your agents, and your users will reply to this email address.

#### Information

+   The email address of **Settings > Notifications > SMTP > Sender email** must match the one used by the email piping server.
+   The setting **Notifications > User email notifications** must be enabled to send replies to the user email.
+   If you're using the Dialogflow App, and the settings **Settings > Artificial Intelligence > Human takeover** is active, no emails are sent if the chatbot knows the answer.
+   If the setting **Convert all emails** is active, all emails sent to your inbox will be converted to chat messages, mind that all emails, including spam, promotional emails and more would be wrongly converted too.
+   If the setting **convert all emails** is active, email sent by email addresses of agents and admins will be ignored, use another email address for testing.
+   If the setting **convert all emails** is active, each email sent directly to the email piping address will generate a new user conversation.
+   You can not use the same email address used for the email piping to reply. All your Support Board agents and admins must use a different email address.
+   Agents must reply via email from the same email address registered in Support Board.
+   When agents reply in Support Board, emails are always sent to the user, even if user email notifications are disabled.
+   The email is sent to the Agents only if they are offline. If they are online no emails are sent.
+   For Google Gmail and Google Workspace emails, you need to replace your Google password with a Google app password, details on [https://support.google.com/accounts/answer/185833](https://support.google.com/accounts/answer/185833) (Create & use App Passwords section). Enter **imap.gmail.com** as host and **993** as port.
+   Email piping requires **php5-imap** module (IMAP module). If it's not installed on your server you can install it with the command **apt-get install php5-imap**. If you have issues contact your hosting/server support.
+   The **Delimiter** option add a text at the top of all emails:
    
    \### Please type your reply above this line ###
    
    . This text tells Support Board to delete all the content below it and it's usefult to cut out all of the reply quotes. Activate it if you see duplicated messages in the chat. If this option is active, you and your users can not use the string **\###** in the emails.
+   Email attachments are supported.
+   In order for email piping to work, email replies must contain the Support Board recipient's name. Ex. **Support Board | SB2457-4734 <example@email.com>**. All major email clients like Outlook Web, Outlook, Gmail, Yahoo Mail, support the recipient's name by default via chatbot reply or reply all buttons.
+   Because of the nature of how emails work, each email client uses their personal codes, delimiters, and automatic strings, and more. For this reason, some chat messages converted from emails can contain invalid texts. We are working to optimize as many email clients as possible, for now, the following email clients are optimized and should not return any invalid text: Outlook Web, Outlook, Gmail, Yahoo Mail.
+   Email piping supports departments, if the user's conversation is assigned to a department, the email notifications are sent only to the agents assigned to that department.
+   If the email includes the **reply-to** attribute, it will serve as the primary user email address and notifications will be sent to that email.

#### Cron job

+   Support Board tries to process emails via cron jobs every 60 seconds, details [here](#cron-jobs).
+   You can manually trigger execution and speed up cron jobs via API with the PHP function [sb\_email\_piping()](https://board.support/docs/api/php#email_piping), or the WEB API function [email-piping](https://board.support/docs/api/web#email-piping).
+   You can create a cron job that runs the URL **\[SUPPORT-BOARD-URL\]/include/api.php?piping=true**. Use the command **\*/59 \* \* \* \* wget \[SUPPORT-BOARD-URL\]/include/api.php?piping=true** to run it via a command. Replace **\[SUPPORT-BOARD-URL\]** with your Support Board URL. To obtain the URL, follow these steps:  
    If you are using the WP or PHP version, go to **Settings > Miscellaneous > Support Board URL**. If you are using the cloud version, use this URL: **https://cloud.board.support/script/include/api.php?piping=true&cloud=API-TOKEN** and replace API-TOKEN with your own API Token which can be found at https://cloud.board.support/account/?tab=installation.
+   You can also use this cron job file: [download](https://board.support/docs/files/cron.zip). The cron job command is **php -f YOUR-FILE-PATH/cron.php**.
+   If you manually run the cron job, check the setting **Disable cron job** to stop Support Board from manually triggering it and to improve performance.

* * *

## Pusher

Activate Pusher from **Settings > Miscellaneous > Pusher** to use the WebSockets instead of HTTP AJAX requests for the chat functionalities. WebSockets drastically improve the chat performance by removing the need for repeated AJAX requests to your server for checking for new messages and conversations. WebSockets also improve responsivness of the chat: faster messages delivery, more accurate online and typing status, more accurate online users list and more.

#### Activation

+   Go to [https://dashboard.pusher.com/accounts/sign\_up](https://dashboard.pusher.com/accounts/sign_up) and create a new account.
+   From your dashboard at [https://dashboard.pusher.com](https://dashboard.pusher.com/), choose the **Channels** product by clicking **Get started**.[](https://board.support/media/docs/pusher-1.jpg)
+   Enter the name of your app and choose the cluster closest to your location.[](https://board.support/media/docs/pusher-4.jpg)
+   From the left menu of the dashboard click **App Settings** and enable **client events**.[](https://board.support/media/docs/pusher-6.jpg)
+   From the left menu of the dashboard click **Keys**, copy **App ID**, **Key**, **Secret**, **Cluster**.[](https://board.support/media/docs/pusher-5.jpg)
+   Go to **Settings > Miscellaneous > Pusher**, and paste app ID, key, secret, cluster.
+   You're done.

#### Information

+   Pusher is free to use for up to 200k messages and 100 concurrent connections per day. Messages are used for the following functions and more: user registration, online user status, chat messages, and chatbot messages. Pusher channels count calculation is explained [here](https://support.pusher.com/hc/en-us/articles/4412259287569-How-Is-My-Message-Count-Calculated-In-Channels-).
+   When Pusher is active the following AJAX requests are replaced by WebSockets: checking for new messages, checking for new conversations, online/offline status, typing status, online users list.
+   When Pusher is active the **last activity** value of users and agents is updated only on page load or when they send new messages.
+   When Pusher is active the option **Settings > Users > Register all visitors** is automatically activated and it can not be disabled.
+   If your server becomes overloaded, crashes, experiences excessive RAM usage, high CPU usage, or in general, slows down or has performance issues, activate Pusher.

* * *

## Direct messages

Direct messages allow you to send а single chat message, email, or text message, to a single user or several users. Read the information below to understand how it works.

#### General

+   To send a message go to the **Users** area and click the direct message icon. Direct message buttons are also available in the profile box of the user.
+   To send a message to all users, enter **All** in the **User IDs** field.
+   To send a message to a group of users, enter their IDs in the **User IDs** field. You can check the users and then click the direct message icon to enter the IDs automatically.
+   All message types support [merge fields](#merge-fields).

#### Direct chat message

+   The chat message is sent to the active conversation, if any, otherwise to a new conversation.
+   If the option **Settings > User email notifications** is active, all users with an email are notified via email.
+   If the option **Settings > Text message notifications > Active for users** is active, all users with a phone number are notified via text message.
+   If the option **Settings > Push notifications** is active, a push notification is sent to all users.
+   The message is also sent to messaging apps such as WhatsApp and Messenger if the user is connected to them.
+   To send a message to all users of a single messaging app enter one of the following strings: **whatsapp**, **messenger**, **instagram**, **telegram**, **twitter**, **google**, **wechat**. Enter **tickets** to send a message only to the users who created a Support Board ticket via the Tickets app.

#### Direct email

+   Email header and email signature are automatically included in all emails, set them from **Settings > Notifications**.
+   The HTML language is supported.
+   The subject supports merge fields.

#### Direct text messages

+   To enable direct text messages you must enable the SMS in **Settings > Notifications > Text message notifications**.

#### Direct WhatsApp template messages

+   For more details click [here](#whatsapp-templates).

* * *

## Automations

Automations allow running multilingual automatic tasks when conditions set by you are met.

+   To delete a condition, set it to empty. To disable an automation, delete all conditions.
+   Automations are sent only 1 time to users.
+   If you used an automation in the past, and users already received it, you need to delete the automation and create a new one to show it to the users.
+   **Repeat** only works if used in conjunction with **date time**.
+   When **date time** is used in conjunction with the criteria **is exactly**, the value must not contain hours and minutes (hh:mm). Ex. 25/10/2021 (25/10/2021 10:30 will not work).
+   The setting **Settings > Users > Register all visitors** must be active if there are message automations that are executed on page load.
+   **City**, **countries**, **languages** work automatically only if both the settings **Settings > Users > Register all visitors** and **Settings > Users > Full visitor details** are enabled.
+   **Cities** work only if the user detail **location** is set and equal to **city, country**, or if the user detail **city** is set.
+   **Countries** work only if the user details **country\_code**, or **country** is set, or if the user detail **location** is set and equal to **city, country**. The country name must be in english.
+   **languages** work only if the user details **browser\_language**, or **language** is set.
+   A visitor is a **Returning visitor** only if it visits the website again after 24h or more.
+   The pop-ups appear only if the chat is closed, and they overwrite the default pop-up. You can check the **message fallback** option to send a message instead of showing the pop-up if the chat is open.
+   You may need to enable **Settings > Users > Register all visitors** if you want to send an automated message to new users.
+   Chat messages and popup fallback messages are sent only if the last user or agent message of the conversation is older than 10 minutes. This feature prevents unwanted automated messages to be sent during an agent-user conversation.
+   The **Custom variable** condition check for the JavaScript variables with the given names and values. For example, the condition **example=ABC** is met if into the chat's page there is this JavaScript code: **var example = "ABC";**. Add multiple variables separated by commas.

* * *

## Newsletter

Follow the steps below to complete the synchronization with your newsletter service. The user is subscribed in the following cases: registration form, user update, follow-up message, subscribe message, email shortcode.

#### Mailchimp

+   To get the **Key**, follow the docs at [https://mailchimp.com/help/about-api-keys/](https://mailchimp.com/help/about-api-keys/).
+   To get the **List ID**, follow the docs at [https://mailchimp.com/help/find-audience-id/](https://mailchimp.com/help/find-audience-id/).

#### Sendinblue

+   To get the **Key**, follow the docs at [https://account.sendinblue.com/advanced/api](https://account.sendinblue.com/advanced/api).
+   To get the **List ID**, follow the docs at [https://my.sendinblue.com/lists](https://my.sendinblue.com/lists).

#### SendGrid

+   To get the **Key**, follow the docs at [https://app.sendgrid.com/settings/api\_keys](https://app.sendgrid.com/settings/api_keys).
+   To get the **List ID**, enter in SendGrid and click **Marketing > Contacts**([https://mc.sendgrid.com/contacts](https://mc.sendgrid.com/contacts)), then click on a list, or create a new one. The last part of the URL is the list ID. Ex. https://mc.sendgrid.com/contacts/lists/8558c1e7-3c99-4428-a68f-78df2e437f8e (the list ID is 8558c1e7-3c99-4428-a68f-78df2e437f8e).

#### Elastic Email

+   To get the **Key**, enter in Elastic Email, then click **Settings** from the top right profile menu. Click **Create Additional API key** ([https://elasticemail.com/account#/settings/new/create-api](https://elasticemail.com/account#/settings/new/create-api)), set a name and choose **Plugin** or **Full access**, or **Custom** and make sure the permission **Contacts** is set to **View & Modify**.
+   The **List ID** is the list name. Important! Existing list's or segment names must not have any spaces in them.

#### Campaign Monitor

+   To get the **Key**, enter in Campaign Monitor, then click **Account settings** from the top right profile menu. Click **API keys > Generate API key**.
+   To get the **List ID**, enter in Campaign Monitor, then click **List and subscribers** from the top menu. Select a list and then click **Settings** from the left menu and copy the **List API ID**.

#### HubSpot

+   To get the **Key**, enter in HubSpot, then get it from **Settings > Integrations > API key**.
+   To get the **List ID**, enter in HubSpot, then get it from **Contacts > List > List details**.

#### Moosend

+   To get the **Key**, enter in Moosend, then click **Settings > API key**.
+   To get the **List ID**, enter in Moosend, then get it from **Audience > Email lists**.

#### GetResponse

+   To get the **List ID**, enter in GetResponse, then get it from **Lists > Your list > Settings**(https://app.getresponse.com/lists). Copy the **List token** value.
+   To get the **Key** visit [https://app.getresponse.com/api](https://app.getresponse.com/api).

#### ConvertKit

+   To get the **Key**, enter in ConvertKit, then get it from **Settings > Advanced > API secret**.
+   To get the **List ID**, enter in ConvertKit, then get it from **Grow > Landing Pages & Forms**. Open you form and copy the numeric part of the URL. For example the ID of the form with URL **https://app.convertkit.com/forms/designers/3003412/edit** is **3003412**.

#### ActiveCampaign

+   To get the **Key**, enter in ActiveCampaign, then get it from **Account settings > Developer**.
+   To get the **List ID**, enter in ActiveCampaign, then get it from **Left menu > Lists** or **Left menu > Contacts > Lists**. Open your list and copy the list ID in the URL. For example the ID of the list with URL **https://schiocco.activehosted.com/app/contacts/?listid=1&status=1** is **1**. The list ID must be in this format: **domain:list-ID**. The **domain** is the first part of your dashboard URL. For example the domain of **https://schiocco.activehosted.com/** is **schiocco** and the final value to insert in Support Board is **schiocco:1**.

#### MailerLite

+   To get the **Key**, enter in MailerLite, then get it from **Left menu > Integrations > MailerLite API**.
+   To get the **List ID**, enter in MailerLite, then get it from **Left menu > Subscribers > Groups**. View a group and copy the Group ID from the URL (e.g. **....group=18783408688903967...**).

#### Mailjet

+   To get the **Key**, visit [https://app.mailjet.com/account/apikeys](https://app.mailjet.com/account/apikeys), or enter in Mailjet, then get it from **Account settings > Account settings**.
+   To get the **List ID**, enter in MailerLite, then get it from **Contacts > Contacts lists > Your list**. Get the List ID by clicking the **?** icon next to the lists's email, e.g. 1202546.

#### Sendy

+   To get the **Key**, enter the Sendy settings area and copy the API KEY.
+   To get the **List ID**, enter your brand, then click **View all lists** and copy the list ID. The list ID setting must also include your Sendy full URL. Enter the URL plus the list ID spearated by the char **|**, e.g. https://example.com|TDf6o892Mx11VXGC51ui567u.

* * *

## Amazon Web Services

#### Amazon S3

Upload attachments to your Amazon S3 bucket instead of the server where Support Board is installed. Follow the steps below to set it up.

+   Log in to AWS as the root user from [https://aws.amazon.com/](https://aws.amazon.com/).
+   Enter the **IAM** dashboard and click **Left menu > Access management > Users**.
+   Click **Add new user**, enter the username and continue.
+   Select **Add user to group** and on the **User groups** section below click **Create group**. In **Permissions policies** search for **AmazonS3FullAccess** and select it. Click **Create user group**.
+   Assign the new group to the user you are creating and continue, then click **Create user**.
+   Select the newly created user and open the **Security credentials** tab.
+   In the **Access keys** area, click **Create access key** and select **Application running outside AWS**. Continue until you get the keys and save them in **Support Board > Settings > Miscellaneous > Amazon S3**.
+   Visit the **Amazon S3** dashboard and click **Create bucket**.
+   Set the bucket name and region you want. Save the region and name in **Support Board > Settings > Miscellaneous > Amazon S3**. Check **ACLs enabled** and **Bucket owner preferred**. Uncheck **Block all public access** and all related checkboxes.
+   Click **Create bucket**.
+   This feature is technical and optional. Support does not cover any help related to this feature.

* * *

## More settings

#### Saved replies

Saved replies, also known as canned messages, refer to a collection of pre-written messages that agents can quickly access and employ in the chat editor.

+   Saved replies can be printed by typing **#** followed by the **saved reply name**, plus a **space**.
+   Use **\\n** to do a line break.
+   If you are using the Dialogflow chatbot, the saved replies panel search will include results from Dialogflow Intents.
+   You have the option to add all Dialogflow Intents to the saved replies list by using the setting at **Settings > Artificial Intelligence > Google > Add Intents to saved replies**.

* * *

NOTIFICATIONS

## Notifications

To understand how notifications work and when they are sent read the information below. If you think notifications are not working, most probably you're just testing them in the wrong way, please read the information below before asking for support.

* * *

## Email notifications

Both agents and users can receive an email notification when a new message is received.

* * *

#### Email notifications for admin and agents

+   When a user sends their first message, if the conversation is assigned to a department, an email is sent only to the agents assigned to that department, if the conversation is assigned to a specific agent, an email is sent only to that agent, otherwise an email is sent to all agents who are not online at the moment. Subsequent emails are sent only to the last agent in the conversation.
+   Email notifications are sent only if the last agent in the conversation is offline.
+   If you're using the Dialogflow App, and **Settings > Artificial Intelligence > Human takeover** is active, no emails are sent if the chatbot knows the answer.
+   To prevent admins from receiving email notifications check **Settings > Notifications > Do not send email notifications to admins**.

#### Email notifications for users

+   When an agent sends a message to a user, an email is sent to the user only if the user is offline.
+   Only 1 email is sent. Subsequent messages will not trigger a new email alert.

#### Create the email

To manage the emails and create the contents go to **Settings > Notifications**. You can use text and HTML. New lines are automatically converted to **<br />**. You can use the following merge fields in the email. Merge fields are automatically replaced with the updated information.

* * *

| Code | Description |
| --- | --- |
| 
{recipient\_name}

 | The name of the user or agent who is receiving the email. |
| 

{sender\_name}

 | The name of the user or agent who was sending the message that triggered the email notification. |
| 

{sender\_profile\_image}

 | The profile image of the user or agent who was sending the message that triggered the email notification. |
| 

{message}

 | The links to any attachments that were part of the message that triggered the email notification. |
| 

{attachments}

 | Emails may not be delivered for several reasons; below are the most common ones: |

#### Cron job

You can run the following cron job for sending email notifications to both users and agents, in which case you also need to select **Settings > Notifications > Email notifications via cron job**. Sending emails via cron job will improve your email notifications: they will include the whole conversation and will be sent only 1 time.

+   You can create a cron job that runs the URL **\[SUPPORT-BOARD-URL\]/include/api.php?email-notifications=true**.
+   Use the command **\*/59 \* \* \* \* wget \[SUPPORT-BOARD-URL\]/include/api.php?email-notifications=true** to run it via a command.
+   Replace **\[SUPPORT-BOARD-URL\]** with your Support Board URL, get it from **Settings > Miscellaneous > Support Board URL**.
+   We don't provide support for problems related to your cron job.

#### Problems?

Emails may not be delivered several reasons; below are the most common ones:

| Reason | Description | Solution |
| --- | --- | --- |
| Hosting problems | The email server of your web hosting provider is not able to send emails or the emails are sent but they are automatically detected as spam and deleted by the email clients. | If the settings at **Settings > Notifications > SMTP** are not set, your server will send the emails instead. Contact your web hosting provider regarding email support or use your SMTP server by activating it in **Settings > Notifications > SMTP**. |
| SMTP problems | The email is not sent also if you activated the SMTP option in the **Notifications** area. | If you don't receive the emails make sure they are working by sending a test email from **Settings > Notifications > Send a user email notifcation** or **Send an agent email notifcation**. If you don't receive the test email, your SMTP server, is not working. Open the browser console for more details about the error. Because this is not an issue related to Support Board , the support doesn't cover it, please contact your server/hosting/SMTP support instead. You can use [sendgrid.com](https://sendgrid.com/solutions/smtp-service/), you can send 40000 emails for 30 days for free, then 100/day forever for free. |
| Google Gmail | The email is not sent also if you activated the SMTP option in the **Notifications** area and you are trying to the Gmail SMTP server. | If you're using Gmail enter **smtp.gmail.com** as host and set **465** or **587** as port. You need also to allow access to Gmail to less secure apps, you can do it from [https://myaccount.google.com/lesssecureapps](https://myaccount.google.com/lesssecureapps). |

* * *

## Push notifications

Push notifications are like Desktop notifications but with some key difference. Desktop notifications, also called Web notifications, are requested directly by the client while Push notifications come from a server. The main difference is that the Push notifications work always, also if your device is offline, or Support Board is not open. Also, they are persistent and always visible until closed. Push notifications require an external service to work. We use Pusher, it is free to use for the admin notifications sent to the agents, and it's free to use for up to 2000 users/devices when sending notifications to the users.

#### Activation

+   Go to [https://dashboard.pusher.com/accounts/sign\_up](https://dashboard.pusher.com/accounts/sign_up) and create a new account.
+   From your dashboard at [https://dashboard.pusher.com](https://dashboard.pusher.com/), choose the **Beams** product by clicking **Get started**.[](https://board.support/media/docs/pusher-1.jpg)
+   Enter the **Instance name** and create the instance. You can enter any value you want.[](https://board.support/media/docs/pusher-2.jpg)
+   From the left menu of the dashboard click **Keys**, copy the **Instance ID** and **Primary key**.[](https://board.support/media/docs/pusher-3.jpg)
+   Enter the Support Board admin area, go to **Settings > Notifications > Push notifications**, and paste instance ID, primary key.
+   You're done.

#### Activation for users

+   Download the service worker file [here](https://board.support/docs/files/service-worker.zip).
+   Upload this file to your site at the following location: **https://your-site.com/service-worker.js**
+   Go to **Settings > Notifications > Push notifications > Service Worker URL** and enter the URL of the file. Ex. **https://your-site.com/service-worker.js**. If you are using the cloud version, enter **https://cloud.board.support/sw.js**. If you are using the SaaS version, replace **cloud.board.support** with your domain.
+   You're done.

#### Information

+   Pusher is free to use for up to 1000 concurrent subscribers. While you should be able to use the free plan for the admin area and all the agents, you may need a paid plan for Push notifications sent to the users depending on your site traffic.
+   Push notifications only work for full HTTPS websites. The only exception is localhost to ease development.
+   When a user click the notification the last page visited by the user is open and the chat is open automatically.
+   On desktop the browser needs to be running since that is the process that receives the push messages.
+   When push notifications are active, they replace desktop notifications.
+   On Android and mobile devices, desktop notifications may not work, in which case you need to use push notifications.
+   If Push notifications are active and not working, disable them and try again.
+   Push notifications can not be received on a desktop PC unless a browser is running.
+   Push notifications on iOS devices (iPhone) are available only from iOS 16.4. You need to install Support Board as a PWA (details [here](#pwa)).

#### Push notifications for admin and agents

+   When an agent click the notification the admin area is open and the right conversation is selected. If the admin area is already open the notification will not open a new tab.
+   When a user sends their first message, a Push notification is sent to all validated agents; subsequent notifications are sent only to the last agent in the conversation.
+   If you're using the Dialogflow App, and **Settings > Artificial Intelligence > Human takeover** is active, no notifications are sent if the chatbot knows the answer.
+   If you're using the WordPress version, Push notifications are not supported in the WordPress admin area, you need to access the Support Board admin area directly, more details [here](#pwa).
+   If the **Routing** setting is active, only the agent assigned to the conversation receive the notification, admins see all conversations but don't receive notifications.
+   If the **Queue** setting is active, only the agent assigned to the conversation receive the notification. Notifications are not sent for messages sent by the user while waiting in queue. Admins see all conversations but don't receive notifications.
+   If a user conversation is assigned to a department, only the agents assigned to that department receive the notification.
+   If a user conversation is not assigned to any department, only agents with no assigned department receive the notification.
+   Notifications are sent only if the last agent in the conversation is offline.
+   If **Settings > Artificial Intelligence > Human takeover** is active, no notifications are sent if the chatbot knows the answer.
+   If push notifications are not working, make sure you allowed the notifications, in Chrome you can check this from **Privacy and Security > Site settings > Notifications**. If they don't work on a mobile device, try these steps too: install the PWA or delete it and install it again, restart the mobile device.
+   If push notifications are not working, and you are using Windows, ensure that the notification feature is not being blocked by Windows. To do this, click on the **Start** button and search for **Notifications**. Then, open the **Turn app notifications on or off** option and verify that your browser is not being blocked.
+   If push notifications are not working, ensure that the Support Board admin area is not visible and open. If the admin area is open, please minimize it or open another window or browser tab.
+   If push notifications are not working, your system might be blocking them. If you are using Windows 10+ check [this link](https://www.makeuseof.com/ways-fix-notification-banners-not-working-windows-10/). If you are on Mac check [this link](https://www.makeuseof.com/fixes-for-mac-not-getting-notifications/).

* * *

## Desktop notifications

#### Desktop notifications

+   Desktop notifications are not sent if the user is viewing a page with include the chat (the user browser is open and visible, and the active page contains the chat).
+   Desktop notifications are not supported on iPhone and iOS devices.
+   Desktop notifications work only for secure URLs that use HTTPS (not HTTP). Your Support Board admin URL must use HTTPS.
+   When push notifications are active, they replace desktop notifications.
+   If desktop notifications aren't working, try the solutions in the [push notifications section](#push).

* * *

## Text message notifications

Both agents and users can be notified via text message when a new message comes in. Text message notifications are provided by Twilio. Twilio is a paid service, but it is cheap, and you can use the trial version to test text message notifications for free.

#### Activation

+   Go to [https://www.twilio.com](https://www.twilio.com/referral/5GOe1g) and create a new account.
+   Verify your phone number.[](https://board.support/media/docs/sms-1.jpg)
+   Complete the form and choose **SMS**.[](https://board.support/media/docs/sms-2.jpg)
+   Once into the dashboard, click **Get a Trial Number**, then **Choose this number**.[](https://board.support/media/docs/sms-3.jpg)
+   Enter the Support Board admin area, go to **Settings > Notifications > Text message notifications**, and paste account SID, auth token, trial number (or a purchased phone number). Find all details in the [Twilio dashboard](https://www.twilio.com/console).
+   If you're using the trial version, you can send notifications only to verified numbers. Enter the Twilio dashboard and click the left button **\# (Phone Numbers)**, then click **Verified Caller IDs** and add your phone number.[](https://board.support/media/docs/sms-4.jpg)
+   To start using the service live and to receive text messages in Support Board you need to purchase a phone number. After the purchase go to **Phone numbers > Manage > Active numbers**, click your number, and enter the URL of Support Board, get it from **Support Board > Settings > Notifications > Text message notifications > Get configuration URL**.[](https://board.support/media/docs/sms-5.jpg)
+   You're done.

#### Information

+   Ensure that your agents and admins are assigned a phone number so that agent text messages can be sent to the appropriate numbers.
+   All phone numbers must have the country code starting with the symbol **+** (eg. +15558675310).
+   You can get the user's phone number via registration form, follow-up message, subscribe messageor, or via **\[email\]** shortcode. You can manually enter the user phone from the admin area or via API.
+   When a user sends their first message, if the conversation is assigned to a department, a test message is sent only to the agents assigned to that department, if the conversation is assigned to a specific agent, a text message is sent only to that agent, otherwise an text message is sent an email is sent to all agents who are not online at the moment. Subsequent text messages are sent only to the last agent in the conversation.
+   Text message notifications are sent only if the last agent in the conversation is offline.
+   If you're using the Dialogflow App, and **Settings > Artificial Intelligence > Human takeover** is active, no text messages are sent if the chatbot knows the answer.
+   To use the Sender ID feature enter the sender name in the **Sender number** field.

* * *

## Sound notifications

+   Sounds work only after the user or agent interact with the document (the user or agent clicked somewhere).
+   If the sound settings are on **All messages**, a sound will play for each new message or conversation, but only when the admin area is closed or minimized. On the other hand, if the setting is set to **Always All messages**, a sound will play for every single message and conversation, even when the Support Board is open.

* * *

GOOGLE

## Google

The settings below are related to the Artificial Intelligence app.

* * *

## Synchronization

To start using the Google AI services and Dialogflow follow the steps below.

+   Enable the setting **Support Board > Settings > Artificial Intelligence > Google > Dialogflow Chatbot** and save the changes.
+   Go to [console.cloud.google.com](https://console.cloud.google.com/) and sign in.
+   Select or create a project by clicking the **Select a project** button on top-left. [](https://board.support/media/docs/dialogflow-sync-1.jpg)Name the project as you want.[](https://board.support/media/docs/dialogflow-sync-2.jpg)
+   Activate the Dialogflow API by entering **Dialogflow API** on the top search bar. Click **Dialogflow API** and then click **Enable**.[](https://board.support/media/docs/dialogflow-api.jpg)
+   Select the project and the go to **Left menu > APIs and services > OAuth consent screen**. Select **External** and click **Create**. [](https://board.support/media/docs/dialogflow-sync-3.jpg)In **App name** enter what you want, in **User support email** and **Developer contact information** enter your email. Click **Save and continue**.[](https://board.support/media/docs/dialogflow-sync-4.jpg)
+   In the scopes area, click **Add or remove scopes**, scroll bottom and into the **Manually add scopes** area enter **https://www.googleapis.com/auth/dialogflow,https://www.googleapis.com/auth/cloud-language,https://www.googleapis.com/auth/cloud-translation**. Click **Add to table** and then **Update** and **Save and continue**.[](https://board.support/media/docs/dialogflow-sync-5.jpg)
+   In the test users area, click **Add users** and add your Google email, use the same email as the currently logged in account. Click **Save and continue**.[](https://board.support/media/docs/dialogflow-sync-6.jpg)
+   Go to **Left menu > APIs and services > Credentials** and click **Create credentials**, select **OAuth client ID**. [](https://board.support/media/docs/dialogflow-sync-7.jpg)As **Application type** select **Web application**. Enter any name you want. In **Authorised redirect URI** enter the redirect URL, get it from **Support Board > Settings > Artificial Intelligence > Google > Authorised redirect URI**. Click **Create**.[](https://board.support/media/docs/dialogflow-sync-8.jpg)
+   Copy **Client ID** and **Client Secret** and paste them into **Support Board > Settings > Artificial Intelligence > Dialogflow**. Save the settings.[](https://board.support/media/docs/dialogflow-sync-9.jpg)
+   In **Settings > APIs & Services > OAuth Consent Screen** click **PUBLISH APP**. There is no need to complete the review process, leave it in the pending review state.
+   Click **Support Board > Settings > Artificial Intelligence > Google > Synchronize**. Login with the same Google account you have used till now. On the next screen click **Continue**. [](https://board.support/media/docs/dialogflow-sync-10.jpg)On the next screen select all scopes and click **Continue**.[](https://board.support/media/docs/dialogflow-sync-11.jpg)
+   Copy the **Refresh token** and paste it into **Support Board > Settings > Artificial Intelligence > Google > Refresh token**.[](https://board.support/media/docs/dialogflow-sync-12.jpg)
+   You are done! If you want to activate the Dialogflow chatbot, check **Settings > Artificial Intelligence > Google > Dialogflow chatbot**. Also, you have to enter your chatbot Project ID or Agent Name, to get it follow the [steps below](#dialogflow-project-id). Note that the app does not need to be approved by Google.

[![](https://board.support/media/play-video.svg)](https://www.youtube.com/watch?v=WLz5zniq7Gk)

* * *

## Dialogflow

The information provided below is relevant to Dialogflow.

#### Get Project ID

+   Log in to the Dialogflow ES console by going to [dialogflow.cloud.google.com](https://dialogflow.cloud.google.com/). You must sign in with the same Google account used during the synchronization.
+   Click the **gear icon** at the top left, near the chatbot name, and open the settings area. [](https://board.support/media/docs/dialogflow-id-1.jpg). If you haven't created a chatbot yet, follow the [instructions below](#dialogflow-bot) to create your first bot.
+   Copy the **Project ID** [](https://board.support/media/docs/dialogflow-id-2.jpg).
+   Make sure to choose **US / GLOBAL** on the top left of the Dialogflow dashboard. Please note that our system does not support mega agents. [](https://board.support/media/docs/dialogflow-region.jpg).

#### Get Dialogflow CX Agent Name

+   Log in to the Dialogflow CX console by going to [https://dialogflow.cloud.google.com/cx/](https://dialogflow.cloud.google.com/cx/).
+   Select the project of the desidered agent and go to the agents page. You can enter the agents page by selecting the agent and by clicking the top button **Agents > View all agents** [](https://board.support/media/docs/dialogflow-cx-1.jpg).
+   Click the options menu for the desiderate agent in click **Copy name** [](https://board.support/media/docs/dialogflow-cx-2.jpg).
+   More details at [https://cloud.google.com/dialogflow/cx/docs/quick/api#detect-intent-drest](https://cloud.google.com/dialogflow/cx/docs/quick/api#detect-intent-drest).

#### Location

Set the location or region of your Dialogflow agent. This setting is optional if your agent location is set to **global**.[](https://board.support/media/docs/dialogflow-location.jpg)

#### Welcome Intent

Trigger the Dialogflow Welcome Intent for new visitors. The option **Settings > Messages > Welcome message** must be active.

#### Send the user details

Send the user details of the registration form and email rich messages to Dialogflow.

#### Add Intents to saved replies

Include the Dialogflow Intents into the saved replies. To access the saved replies option, go to **Settings > Admin > Saved replies**.

* * *

#### Create a basic chatbot

If you haven't created a chatbot yet, follow the instructions below to create your first one. The creation and management of your Dialogflow chatbot is handled entirely by Dialogflow. There are a lot of tutorials online that can help you create and configure your Dialogflow bot.

+   To create your first chatbot enter the [Dialogflow console](https://dialogflow.cloud.google.com/) and create an agent. As **Google project** select the same project used during the synchronization.
+   Add a new **Intent** from the left menu and open it.
+   In the **Training phrases** area adds the user's question you want the chatbot to reply to, add as many variants are you can. For example, if you want to the chatbot to reply to users asking for your business address, add variants like "what is your address", "address", "where are you".
+   In the **Responses** area adds the chatbot answer as a **text response**.
+   You have created your first question and answer! Test if from the right area or from the Support Board chat. Add new Intents to populate your chatbot with the questions and answers you want. You can include basic pre-built questions and answers by enabling the **Small Talk** feature from the left menu.

[![](https://board.support/media/play-video.svg)](https://www.youtube.com/watch?v=l-uAw1EoeQY)

#### Here are some great resources to help you build a more complex chatbot:

+   [chatbotslife.com/dialogflow-restaurant-bot-tutorial-1-45ce1d3c0ab5](https://chatbotslife.com/dialogflow-restaurant-bot-tutorial-1-45ce1d3c0ab5).
+   [tutorials.botsfloor.com/building-your-own-chatbot-using-dialogflow-1b6ca92b3d3f](https://tutorials.botsfloor.com/building-your-own-chatbot-using-dialogflow-1b6ca92b3d3f).
+   [marutitech.com/build-a-chatbot-using-dialogflow/](https://marutitech.com/build-a-chatbot-using-dialogflow/).

* * *

## Actions

The following actions give the chatbot the ability to interact with the website autonomously on behalf of the user. To use an action go to Dialogflow, edit an **Intent**, and add a new **Custom Payload** response with the following syntax: **{ "ACTION-NAME": ACTION-VALUE }**.

| Action code | Description |
| --- | --- |
| 
{ "human-takeover": true }

 | Disable the chatbot for 5 minutes, notify agents, and leave the conversation marked as unread. |
| 

{ "disable-bot": true }

 | Disable the chatbot for 5 minutes. |
| 

{ "redirect": "URL" }

 | Redirect the user to the given URL. Add the value **"new-window": true** to open the URL in a new window. |
| 

{ "open-article": ID }

 | Open the article with the given ID. |
| 

{ "transcript": true }

 | Generate the conversation transcript as a text file and download it. Set it to **email** to send the transcript to the user's email, add the value **message: "Your message"** to include a message in the email. |
| 

{ "tags": \["Tag 1", "Tag 2"\] }

 | Assign tags to a conversation. |
| 

{ "department": ID }

 | Change or set the conversation department and notify the agents. |
| 

{ "agent": ID }

 | Change or set the agent assigned to the conversation and notify the agent. |
| 

{ "send-email": { "recipient": "active\_user", "message": "", "attachments": \[\] } }

 | Send an email to the active user or agents. Attachments syntax: **\[\["name", "link"\], \["name", "link"\],...\]}**. Recipient value can be **active\_user** or **agents**. |
| 

{ "update-user": true }

 | Tells the admin area to update the user of the active conversation. Use this action in combination with other actions to update the user details of the admin area in real-time. |
| 

{ "archive-chat": true }

 | Archive the chat and send the close message if active. |
| 

{ "update-user-details": { "email": "", "last\_name": "", "first\_name": "", "extra": { "phone": \["+123456789", "Phone"\] }}}

 | Update the details of the active user. You can update all details, including **first\_name**, **last\_name**, **email**, **user\_type**, **password** You can update the user extra details, like the phone number, by entering the values into the **extra** key, the values must use the following syntax: **"slug": \[value, "label"\]**. Download an example [here](https://board.support/docs/files/dialogflow-example-1.zip). To upload an Intent go to the **Intents** area and click the 3-dots menu icon on the top-right, then click **Upload Intent**. Start the conversation by sending the message "start". |
| 

{ "update-user-language": "$language" }

 | Update the user language, and the chatbot language if multilingual chatbots feature is active, to match the language requested by the user. The Dialogflow Entity value for the language is represented by the parameter **$language**.[](https://board.support/media/docs/dialogflow-change-language.jpg) |

* * *

## Dialogflow Fulfillment

The fulfillment data sent to your webhook URL is like below:

 {
 	"responseId": "4a58fc4f...",
 	"queryResult": {
 		"queryText": "fullfilment",
 		"parameters": \[\],
 		"allRequiredParamsPresent": true,
 		"fulfillmentText": "Example",
 		"fulfillmentMessages": \[{
 			"text": {
 				"text": \["Response"\]
 			}
 		}\],
 		"outputContexts": \[{
 			"name": "projects/schiocco...",
 			"parameters": {
 				"no-input": 0,
 				"no-match": 0
 			}
 		}\],
 		"intent": {
 			"name": "projects/schiocco...",
 			"displayName": "Fullfilment"
 		},
 		"intentDetectionConfidence": 1,
 		"languageCode": "en"
 	},
 	"originalDetectIntentRequest": {
 		"payload": {
 			"support\_board": {
 				"conversation\_id": "3002",
 				"user\_id": "3777"
 			}
 		}
 	},
 	"session": "projects/example/agent/sessions/3777-3002"
 }

The **payload** and **session** fields contain the Support Board user ID and conversation ID.

* * *

## Dialogflow Information

#### Chatbot training and optimization

+   It will require some time for your chatbot to consistently provide correct answers to all questions. To improve its performance, you and your human agents should continuously train the chatbot by incorporating new question variations and Intents. This approach will effectively enhance the capabilities of your chatbot.
+   Agents can add new Intents and chatbot responses, and add new training phrases to existing intents on the fly from the admin area by moving the mouse cursor over a message and clicking the Dialogflow Intent icon. Enable **Settings > Artificial Intelligence > OpenAI > Generate user expressions** to automatically add variations of the question and to rewrite the answer. New Intents will contain also the responses, while the update of existing intents will add new training phrases only, but not new chatbot responses. If you're using Dialogflow CX, the chatbot responses will be added to the latest flow used in the conversation if any, otherwise to the start flow.
+   If the chatbot is replying with the wrong intents, go to **Dialogflow Console > chatbot Settings > ML Settings**, and set the **ML CLASSIFICATION THRESHOLD** to a larger number, such as 0.6. Also check the [Intent detection confidence](#dialogflow-confidence).

#### Dialogflow Intent detection confidence

When searching for a matching intent, Dialogflow scores potential matches with an intent detection confidence, also known as the confidence score. These values range from 0.0 (completely uncertain) to 1.0 (completely certain). Specify a value ranging from **0.1** to **1.0**. Any answer provided by Dialogflow that is less than this value will not be considered. If you are utilizing Dialogflow alongside your OpenAI chatbot that is trained using your resources, it is recommended to configure the value as **0.81**.

#### Knowledge Base

Knowledge Base are automatically enabled. Knowledge Base is a feature that gives your chatbot the ability to search within documents (such as a PDF) or web pages to find an answer. To create your first Knowledge Base, go to [cloud.google.com/dialogflow/docs/knowledge-connectors](https://cloud.google.com/dialogflow/docs/knowledge-connectors)

#### Dialogflow response

The full Dialogflow **JSON** response is automatically saved in the database, **sb\_messages**, column **payload**.

#### Ignore an Intent if it doesn't fit the provided keywords

Sometimes Dialogflow gives incorrect answers due to similar questions with different subjects. To solve this, you can instruct Support Board to ignore an Intent if specific keywords are not present in the user's message. Here's how you can do it:

+   Enter Dialogflow and edit the Intent.
+   For each training phrase, select the keywords you want to be required and link them to a new **Entity**, or an existing one.
+   Under **Actions and parameters** check **Required** and add a new **Prompt** with value **skip-intent**
+   Save the Intent.[](https://board.support/media/docs/dialogflow-skip-intent.jpg)

#### User attachments

User attachments are sent to Dialogflow by appending the attachments to the message details in the following format:

\[name:file-name.ext,url:URL,extension:file-extension\]

Example:

                                    \[name:archive.zip,url:https://board.support/archive.zip,extension:zip\]
                                    \[name:license.pdf,url:https://board.support/license.pdf,extension:pdf\]
                                

#### Chatbot attachments

To allow the chatbot to send attachments, add a **Custom Payload** response and insert this JSON code:

                                    { "attachments": \[\["name", "YOUR-LINK"\], \["name", "YOUR-LINK"\], \["name", "YOUR-LINK"\]\]}
                                

Replace "name" with the actual name of the attachment to display and replace "YOUR-LINK" with the actual URL of the file. Images attachments are displayed automatically as images.

#### Rich messages

To allow Dialogflow to send [rich messages](#rich-messages), simply enter the rich message shortcode into the **TEXT RESPONSE** field or add a new **Custom Payload** response and insert this JSON code: **{ "rich-message": "shortcode" }**. Replace "shortcode" with the rich message shortcode, to have a valid JSON code you need to replace all **"** chars with **\\"**. To obtain the shortcodes or to learn how to create a rich message, please click [here](#rich-messages).

#### Rich message response

When the user interacts with rich messages via the Support Board chat (e.g. by clicking a button), the rich message response is sent to Dialogflow in the following format: **ID|response**, or **ID** if the rich message type is registration, email, follow up, in this case the rich message values are sent as array in the **queryParams\['payload'\]** key. **ID** is the rich message ID, which can be set by adding the attribute id="YOUR-ID" to the shortcode. If no ID has been set, a random ID will be used instead. **response** is the input or selection of the user. To block Dialogflow from replying to a rich message add a new intent with **ID** as the only user expression and no response.

If the user is interacting with the chatbot via a messaging app (e.g. WhatsApp), the response of the rich message does not contain the rich message ID and Dialogflow **contexts** must be used to allow Dialogflow to understand which Intent to activate for a specific rich message response.

#### Get rich message response for registration, email, follow up

+   Check the option **Support Board > Settings > Artificial Intelligence > Google > Send user details**.
+   From **Left menu > Fulfillment** enable **Webhooks**, you only need to enter the URL of the file that will receive the Dialogflow webhook data.
+   Create an Intent with the ID of the rich message, for the registration form, enter **registration**, for the follow up form enter **sb-follow-up-form**, for email forms enter **email**.
+   Enable the Fulfillment for the Intent.
+   You're done! The file of the webhook URL will receive the Support Board rich message user details.

#### Sequential survey

To create a sequential survey like the one of the demo you need to Enter the **Rich message ID** in the **Training phrases**, check the example below.

+   Go to Dialogflow and create a new intent. In the **Training phrases** area enter the user expression **survey example**. In the **Responses** area enter the code **\[buttons id="test-survey-1" options="Software,Physical products,Services" title="What is your type of business?" message="Please choose the type that best suits your company." success="Your company type is "\]**
+   Create a new intent. Enter the user expression **test-survey-1** and as response enter **\[select id="seq-survey-2" options="Priority post, Express courier, International courier" title="Shipping methods" message="Choose the preferred shipping method of your customers" success="Your customers preferred shipping method is"\]**
+   Create a new intent. Enter the user expression **test-survey-2** and as response enter **Thank you for completing our survey!**.
+   You're done.

#### Departments linking

+   Get the department IDs from **Settings > Miscellaneous > departments**.
+   Get the project IDs from the Dialogflow settings area of your agents.

#### More information

+   Dialogflow supports the use of voice messages through speech recognition.
+   You can activate the chatbot via API but sending a message with no text and payload **{ "event": "activate-bot" }**.
+   The following details are sent to Dialogflow in the **queryParams** parameter when detecting an intent: **conversation\_id**, **user\_id**.
+   To trigger the welcome event in Dialogflow CX, create a **Event Handler** and insert **Welcome** as **Custom Event**.
+   Support Board articles are synchronized automatically with the Dialogflow knowledge base.
+   Use the JS variable **SB\_DIALOGFLOW\_AGENT = "AGENT ID"** to change the default Dialogflow agent, replace "AGENT ID" with the **project ID**.
+   If the user sends the same message again, triggering the same Intent in Dialogflow, and OpenAI is active, Support Board will attempt to send a message from OpenAI and will ignore the response from Dialogflow.

* * *

## Dialogflow Multilingual

Check if there is a Dialogflow agent in the user's language and activate it. Make sure to activate this setting even if your OpenAI sources consist of multiple languages.

* * *

## Automatic Translation

The automatic translation feature automatically translates user messages into agent language and agent messages into user language. To enable the language detection feature and automatic translation of agent messages to the language of the user, and user messages to the language of the agent, check the option **Settings > Artificial Intelligence > Automatic translation** and complete the synchronization process. The [multilingual via translation](#multilingual-via-translation) feature also requires these steps.

+   The Google account used for the Dialogflow synchronization must have billing and the **cloud-translation** service enabled, to do that follow the steps below:
+   Log in to [https://console.cloud.google.com](https://console.cloud.google.com/) with your Google account and select the project of your Dialogflow Agent.
+   On the top search bar type **cloud translation**, select the **Cloud Translation API** service and enable it. Please note that this is a paid service with a free tier, additional charges may occur.
+   Enable the billing by clicking **Left menu > Billing** and by enabling a billing account with a valid payment method. Enable billing for the project of your Dialogflow agent.

#### Information

+   The user messages in the admin area are translated automatically in real-time to match the agent language.
+   The agent messages are translated automatically in real-time to match the user language.
+   Agents can view the original message by opening the message menu and by clicking **View original message**.
+   The agent language is based on the **language** user detail of the agent if set, otherwise on the browser language, or admin area language.
+   The user language is based on the **language** user detail, if set, otherwise on chat language, if set, otherwise on the browser language. The language can also be detected with the feature **Setting > Artificial Intelligence > Language detection**.
+   The notifications are also translated.
+   To avoid translating a string, enclose it with the characters **\`** or **\`\`\`**.

#### Multilingual via translation

The feature at **Settings > Artificial Intelligence > Multilingual via translation** automatically translates user messages into the default language of Dialogflow or OpenAI, and translates Dialogflow or OpenAI messages into the language spoken by the user. Additionally, this feature translates all text displayed within the chat, such as the chatbot's rich messages, registration forms, and pop-up notifications. To enhance performance and minimize translation costs, the translations are automatically integrated into the translation files. Combine this feature with the language detection feature for optimal results.

+   The original texts must be in English.

#### Language detection

Detect the language of the user' messages and change the user language and Dialogflow agent language accordingly, if available, otherwise, show a fallback message. You can use the following merge fields in the message: **{language\_name}**.

+   The user message must be at least 2 words long.
+   Language detection is executed only for the first 2 user messages of a conversation.
+   As long as the OpenAI chatbot is operational and programmed to respond to generic inquiries, the fallback message will never be dispatched, since OpenAI will consistently provide answers to any use message.

* * *

## Google search

The Google search features give your chatbot the ability to search for answers on Google and your website and automatically correct misspelled user questions. To start using it, follow the steps below.

+   Register at [https://programmablesearchengine.google.com/](https://programmablesearchengine.google.com/).
+   Create a search and setup it is as you want. We recommend to add only your website and Wikipedia if you want your chatbot to reply to general questions, leave disabled the option **Search the entire web**. Use the setting **Entities** to exclude invalid results.
+   Go to **Edit search engine > Setup > Basic** and copy the **Search engine ID** value, paste it in Support Board.
+   To get the API key visit [https://developers.google.com/custom-search/v1/overview](https://developers.google.com/custom-search/v1/overview) and click **Get a key**.

#### Spelling correction

In the case where Dialogflow is unable to find the appropriate response to the user's message, this function verifies if there are any spelling errors. If any such errors exist, Dialogflow is prompted again with the correctly spelled version of the message for an accurate response. Although it has a lower priority, this feature can still work together with the OpenAI Dialogflow spelling correction feature.

#### Entities

The **Entities** setting analyze the user's message and recognize and extract entities like cities, events, dates, and more. Use it to exclude invalid results returned by Google search. To enable this setting follow the steps below.

+   Log in to [https://console.cloud.google.com](https://console.cloud.google.com/) with your Google account and select the project of your Dialogflow Agent.
+   Enter **Cloud Natural Language API** in the search bar at the top, select **Cloud Natural Language API** and enable the API [](https://board.support/media/docs/cloud-natural-language-api.jpg).
+   Enable the billing by clicking **Left menu > Billing** and by enabling a billing account with a valid payment method. Enable billing for the project of your Dialogflow agent.

#### Information

+   The Google search is performed only if the chatbot does not know the answer to the user's question and if the length of the user's message is greater than 4 characters.
+   If the Google search returns a result, the Dialogflow context **google-search** is automatically activated. The context contains the attribute **link** which is the website's link of the Google search result. Use the context to create a new intent that provides the link, if the user sends a message like **tell me more** or **I want to know more**.[](https://board.support/media/docs/google-search-intent.jpg)
+   Google Search is not required to activate the spelling correction. You can disable Google Search and activate only spelling correction.
+   If Google Search is active, it will have priority over OpenAI.

[![](https://board.support/media/play-video.svg)](https://www.youtube.com/watch?v=8cSOL_N2wSc)

* * *

OPENAI

## OpenAI

The settings below are related to the Artificial Intelligence app.

## Synchronization

OpenAI (ChatGPT) integration gives your chatbot the ability to answer general questions about almost anything you can imagine. To start using it, follow the steps below.

+   Register at [https://beta.openai.com/signup](https://beta.openai.com/signup).
+   Get an API key from [https://beta.openai.com/account/api-keys](https://beta.openai.com/account/api-keys) and paste it into **Settings > Artificial Intelligence > OpenAI > API key**
+   Enable the chatbot from **Settings > Artificial Intelligence > OpenAI > Chatbot**.

#### Information

+   If OpenAI is not working, click [here](#ai-problems).
+   If you want to send only the latest user message and prevent all previous conversation messages from being sent to OpenAI, you can select the option **Omit previous messages**. If OpenAI is unable to reply after a few user messages, you can try checking this option and attempting again.
+   If Dialogflow is active, the OpenAI query is performed only if the chatbot does not know the answer to the user's question and if the length of the user's message is greater than 4 characters.
+   The following settings are compatible with OpenAI: **Smart reply**, **Human takeover**, **Disable for the tickets area**, **Disable during office hours**, **Bot response delay**, **Reply to user emails**, **Reply to user text messages**.
+   The following Google settings are compatible with OpenAI: **Multilingual**, **Multilingual via translation**, **Automatic translation**, **Language detection**
+   If a human takes control, the OpenAI chatbot is deactivated, and is remains deactivated also if the agent goes offline. The Dialogflow chatbot continues to function whenever necessary.
+   The default model is **gpt-3.5-turbo-instruct**.
+   OpenAI supports the use of voice messages through speech recognition.

* * *

## Settings

See information about most OpenAI settings here.

#### Chatbot

The OpenAI chatbot feature functions similarly to Dialogflow, providing automated responses to user messages. Select the **Chatbot mode** setting to specify the questions that the chatbot is capable of responding to. Utilize the [human takeover](#human-takeover) feature to enable the chatbot to redirect the chat to a human agent as necessary.

#### Fallback message

The fallback message is sent when OpenAI is unable to understand the user question. If the Dialogflow chatbot is enabled, the fallback message will be turned off and the Dialogflow chatbot's fallback message will be utilized instead.

#### Prompt

The prompt instructs OpenAI on how to respond by providing relevant information that can be utilized to answer user inquiries. To comprehend the process, refer to the example prompts listed below.

#### Prompt - Message rewriting

This prompt instructs OpenAI on how to rewrite a message when the **Message rewrite button** is active. This prompt should be in English. Support Board automatically add the following text when required: **and use the user langauge, add greetings**.

Replies from the training sources can be utilized with the prompt feature as they are compatible.

If you choose to activate the human takeover feature, you need to include a particular phrase in your query to prompt OpenAI to respond with **I don't know** if it is unable to provide an answer to the user's question. For example you can use: **Respond "I don't know", if not sure about the answer**.

#### Spelling correction

This feature automatically fix any spelling mistakes in the agent's message.

#### Dialogflow spelling correction

In the case where Dialogflow is unable to find the appropriate response to the user's message, this function verifies if there are any spelling errors. If any such errors exist, Dialogflow is prompted again with the correctly spelled version of the message for an accurate response. Although it has a higher priority, this feature can still work together with the Google Search spelling correction feature.

#### Message rewrite button

This feature adds a button to the text field of the conversation area, click on it to rewrite your message and make it more friendly and professional. Greetings will be added automatically if there is no previous agent messages. If your language is not English, you have to edit your agent/admin profile and set the correct language.

#### OpenAI parameters

Support Board allows you to adjust various OpenAI parameters such as temperature and logit\_bias, for more details visit [https://platform.openai.com/docs/api-reference/completions/create](https://platform.openai.com/docs/api-reference/completions/create). Don't set any values if you don't know what these parameters do or OpenAI may stop working.

#### Generate user expressions - Option

When this option is active, OpenAI will generate new user expressions in real time when you open the [chatbot training window](#chatbot-training-window).

#### Generate user expressions - Button

When you click the button **Generate user expressions**, openAI will update your Dialogflow agent and generate new user expressions for each Intent.

+   Make a backup of your Dialogflow agent first.
+   This task can take several minutes or even hours if your chatbot has a lot of Intents. Since the operation takes a long time, your server may interrupt the operation (operation timeout) before it finishes, in which case you need to click the button again. You can verify if the operation is interrupted by checking the browser console for errors.
+   This task is performed only once per Intent. Previously processed Intents will be ignored.
+   This task checks existing user expressions and does not create duplicates.
+   The first 5 user expressions will be used to generate new user expressions.
+   Since this is an automated process, we strongly recommend reviewing your Intents after the task has been completed.

[![](https://board.support/media/play-video.svg)](https://www.youtube.com/watch?v=eNsK-Kj7eGM)

* * *

## Training

With this feature, your chatbot can undergo training using your website texts or PDF documents. Once the training is successfully completed, the chatbot will be able to answer questions related to your contents.

+   To initiate the chatbot training, input the URL of your content in **Settings > Artificial Intelligence > Open AI - Training Sources**. It is possible to enter URLs for websites, text or PDF files, or XML sitemaps. PDF and text files can also be uploaded from **Settings > Artificial Intelligence > OpenAI - Training Sources - PDF and Text Files**.
+   Once the sources are set, click the **Train your chatbot** button and await completion of the training process.
+   You can add and manage personalized question and answers from **Settings > Artificial Intelligence > OpenAI - Questions and answers** and from the [chatbot training window](#chatbot-training-window).

#### Information

+   It is only possible to upload files in PDF and TXT formats.
+   You can provide the website URL and all child URLs will be included and crawled, but with large websites, it is more efficient and less prone to errors and infinite link loops to utilize an XML sitemap instead of relying on the website URL. You can create it with a service like [https://www.xml-sitemaps.com](https://www.xml-sitemaps.com/).
+   If you want to train your chatbot using specific pages from your website instead of all of them, you can make use of an XML sitemap. Create one using a tool like [https://www.xml-sitemaps.com](https://www.xml-sitemaps.com/), and then remove the pages you do not wish to include by editing the file in a text editor. To use the XML sitemap, you need to upload it either onto your server or an external online location. Afterward, add the URL of the sitemap in **Settings > Artificial Intelligence > OpenAI - Training sources**.
+   You can upload large files and your XML sitemap with a service like [https://tmpfiles.org](https://tmpfiles.org/).
+   If you are training OpenAI with a multi-language website, you can limit the chatbot to retrieve answers only from the pages in the user's language. To activate this feature, go to **Settings > Artificial Intelligence > OpenAI > Multilingual Training Sources**. For Support Board to comprehend the language of your web pages, the **<html>** must contain the attribute **lang**.
+   As soon as the training is completed, the uploaded files are removed. Every time you need to retrain the chatbot, you are required to upload all the necessary documents for its training once again.
+   To add new training sources, simply train the chatbot again. The previous training sources will not be lost, and only the new sources will be added.
+   The Support Board articles are used as training sources automatically.
+   If you are using the cloud version, there are character limits for training the chatbot. You can review the quotas by visiting [](https://cloud.board.support/account/?tab=membership). However, if you are using the PHP or WP version, there are no limits imposed.
+   The **ADA embedding model** is essential for training your chatbot and handling all user messages. It is necessary for these scenarios and cannot be disabled. Please note that the ADA Embedding model is different from the ADA model and is available at a much lower cost. You can find pricing information at [https://openai.com/pricing](https://openai.com/pricing). Check out the pricing for the **Ada** model in the **Embedding models** section.
+   The responses generated by OpenAI have the feature to include in the reply a link to the corresponding website page where the answer was sourced.
+   Click **Delete training** to remove all previous training data for the chatbot.
+   The embeddings are stored as JSON files in the Support Board [uploads folder](#config) and are secured using the password-by-filename approach.

* * *

AI

## ARTIFICIAL INTELLIGENCE

The settings below are related to the Artificial Intelligence app.

* * *

## Human Takeover

#### General information

+   When the human takeover is activated the chatbot is automatically disabled for as long as the agent is online. After that, the chatbot is activated again but no default fallback messages will be sent within 10 days of human takeover if the chatbot doesn't know the answer to the user's question in the same conversation. You can force a Dialogflow message to be always sent by adding to the Intent the custom Payload value **"force-message": true**.
+   The OpenAI chatbot is disabled for 10 days, and it will continue to remain inactive even if the agent is offline.
+   The chatbot is fully activated again when the conversation is archived or deleted.
+   If you're using Slack, no messages will be sent if the chatbot knows the answer. Once the human takeover is active all conversation's messages are sent to Slack.
+   When a human agent reply to a user the human takeover is activated automatically.
+   The human takeover feature is compatible with OpenAI and will continue to function even if the Dialogflow chatbot is deactivated.
+   To fully disable the chatbot on human takeover, check the option **Human takeover > Disable chatbot**.
+   If the human takeover is already active, it will not be activated again, and the human takeover message will not be sent.

#### Human takeover option

When the option **Human takeover** is active the following happens:

+   If enabled, the request is sent only if the message sent by the user is longer than 3 chars and contains at least two words. This optimization prevents mistaken requests.
+   The conversations to which the chatbot was able to answer correctly, are marked as read and moved at the bottom of the **Inbox** list.

When the user confirms the human takeover, or if it is automatic, the following happens:

+   The conversation is marked as unread and moved on top of the **Inbox**.
+   Any future user messages in the same conversation sent within 10 days of the human takeover, and without an answer from the chatbot, will trigger agent notifications.
+   If agents email notifications are active, an email notification is sent to the agent assigned to the conversation, or, if the user's conversation is assigned to a department, to the agents assigned to that department, otherwise it is sent to all offline agents.
+   If push notifications are active, a push notification is sent to the agent assigned to the conversation, or, if the user's conversation is assigned to a department, to the agents assigned to that department, otherwise it is sent to all offline agents.
+   If text message notifications are active, a text message is sent to the agent assigned to the conversation, or, if the user's conversation is assigned to a department, to the agents assigned to that department, otherwise it is sent to all offline agents.
+   No human takeover requests within 10 days of the human takeover will be sent in the same conversation.
+   If the [follow-up message](#follow-up-message) is active, the message requesting the user's email is sent only if the user does not have the email.
+   If the [offline message](#offline-message) is active, the offline message is sent only if it is not office hours or if all agents are offline.
+   If the [queue](#queue) is active, the queue is activated.

#### Manual human takeover - Dialogflow Only

+   You can manually trigger the human takeover by creating a new Dialogflow **Intent** with the following **Custom Payload** response: **{ "human-takeover": true }**.
+   The manual takeover automatically notify agents via email and leave the conversation marked as unread.
+   To manually send a human take over request use the chips rich message with ID **sb-human-takeover**. Ex. **\[chips id="sb-human-takeover" options="Human support,Cancel" message=""\]**.

#### WhatsApp, Messenger, Telegram

The make the human takeover request work on WhatsApp, Messenger, Telegram and the other messaging apps, you need to create a new **Intent** with **human-takeover** as **input Context**, nothing as **output Context**, a list of the user's most common confirmation messages as **Training phrases**(e.g. ok, yes) and **{ "human-takeover": true }** as **Custom Payload** response [](https://board.support/media/docs/human-takeover-intent.jpg).  
[![](https://board.support/media/play-video.svg)](https://www.youtube.com/watch?v=O0UFpdQ2kYs)

* * *

## Smart Reply

Smart Reply suggests quick responses in real-time during a conversation. Once active, you will see the suggested replies in the conversation area, if any.

#### Information

+   The Smart Reply feature initially checks for suggestions from the Dialogflow chatbot, provided it is active. If there is at least one suggestion, it will promptly display the results. However, if Dialogflow is inactive, or there are Dialogflow suggestions, the OpenAI suggestions will be returned instead.
+   If the [Language detection](#google-translation) feature under **Settings > Artificial Intelligence > Google > Language detection** is active, the smart replies will use language detection as well.
+   If the [multilingual via translation](#multilingual-via-translation) feature is enabled, the smart replies will utilize multilingual translation as well.
+   To read the complete text of a smart reply, hover the mouse pointer over it for a duration of 3 seconds.
+   To restore the previous message, press the keyboard shortcuts **CTRL + Z**.

* * *

## Optimal configuration for the chatbot

Support Board provides powerful tools to assist you in the process of creating the chatbot.

+   Activate **Artificial Intelligence > Google > Dialogflow chatbot**. If you have general or specific inquiries that require a definitive response, the Dialogflow chatbot is the best option and it can work alongside the OpenAI chatbot. The Dialogflow and OpenAI chatbots can work together simultaneously. More details [here](#dialogflow-bot).
+   Keep improviding the chatbot from the [chatbot training window](#chatbot-training-window).
+   Activate **Artificial Intelligence > Smart Reply**. More details [here](#smart-reply).
+   Activate the following **OpenAI** settings: **Chatbot**, **Spelling Correction**, **Dialogflow spelling correction**, **Rewrite Message Button**, and **Generate User Expressions**. More details [here](#open-ai).
+   Train your OpenAI chatbot with your own content, more details [here](#open-ai-training).
+   Set the value of **Google > Dialogflow Intent detection confidence** to **0.81**.
+   If your website receives traffic from multiple countries, consider activating the following **Google** options: **multilingual via translation**, **automatic translation**, **language detection**.
+   Change the chatbot name from **Settings > Users > Bot name**.

* * *

## Chatbot training window

You can open the chatbot training window from the conversation area by hovering the mouse over a message, opening the message's menu, and selecting **Train chatbot**.

+   If Dialogflow is active, a new Intent will be added to the main Dialogflow agent.
+   If OpenAI is active, the OpenAI chatbot will be trained automatically with the new information. You can control the questions and answers generated from this window from **Settings > Artificial Intelligence > OpenAI - Questions and answers**.

* * *

## Problems?

The most frequent reasons for OpenAI or Google not functioning properly are listed below. For more details about the issue, open the **browser developer tools** and then the **console** tab, send a message through the Support Board chat, and an error should appear in the console. On Chrome you can open the console from **Settings > More tools > Developer tools > Console**.

#### OpenAI and Google

+   There is a [human takeover](#human-takeover).

#### OpenAI

+   You reached the quote limit or you are encountering billing problems with your OpenAI account. Check it at [https://platform.openai.com/account/usage](https://platform.openai.com/account/usage).
+   If Dialogflow is enabled, OpenAI may not work correctly because your Dialogflow agent does not have the Fallback Intent. Please verify its presence on the Intents page, and if it's missing, you can create it again by following the instructions [here](https://cloud.google.com/dialogflow/es/docs/intents-default). To quickly check if this is the issue, you can disable Dialogflow and send a message consisting of 2-3 words. Then, check if the browser console has errors.
+   Make sure to read the general [information](#open-ai-sync-info).
+   If the training is not working as intended, for instance, if the chatbot is not responding to questions relevant to the training sources, and no training errors are being shown, there may be file permission issues. To address this, please ensure that the [uploads folder](#config) includes the **embeddings** folder. It must exists and contains files.

#### Google

+   If your synchronization was not successful we suggest reviewing our documentation and repeating the synchronization steps to correct any errors. If needed, we provide integration services. Details at the [hire us](https://board.support/hire-us) page.
+   You selected the wrong agent location.
+   You are using a mega agent.
+   Make sure to read the general [information](#dialogflow).

* * *

WORDPRESS

## WordPress

The settings below are related to the WordPress version of Support Board.

* * *

## User synchronization

WordPress users can be automatically synchronized with Support Board by selecting "WordPress" under the **Users system** in the **Settings > WordPress** area. When active, the front-end chat automatically recognize all logged-in WordPress users and create a new Support Board user account with the same details (name, surname, email, and password). Also, the log-in form recognize the email and password of each WordPress user. On Support Board login, the user is automatically logged in WordPress as well.

+   To create a WordPress user when a visitor register to Support Board enable the option **Settings > WordPress > WordPress registration** and include password and email fields in the registration form, they are required. The WordPress user if logged in automtically.

* * *

## More information

#### Direct access and PWA

You can access the admin area directly without going through WordPress by navigating to **/wp-content/plugins/supportboard/supportboard/admin.php** and logging in with your default WordPress user or agent email and password. Keep in mind that your wp-content folder might be different. By accessing the admin directly, you will also be able to use the admin area as a Progressive Web App. You can find more details on this by clicking [here](#pwa).

#### Login and logout

To logout from the admin area of Support Board , logout from WordPress from the admin area of Support Board , once logged-out you will be able to login with another WordPress account. To access the admin area from within WordPress you must log in with one of the following WordPress user roles: administrator, author, editor.

#### Get a page or Post Type ID

To get the ID of a specific page or Post Type, go to the admin area of WordPress and edit the page or post. The ID is displayed in the address bar. Example: **http://your-site.com/wp-admin/post.php?post=11&action=edit&lang=en** (the page/post ID is equal to 11).[](https://board.support/media/docs/wp-id.jpg)

#### Get a Post Type slug

The Post Type slug of the blog archive and posts is **post**. The Post Type of the pages is **page**. To obtain the slug of a custom Post Type, go to the admin area of WordPress and open the custom Post Type page from the left menu. The slug is displayed in the address bar. Example: **http://your-site.com/wp-admin/edit.php?post\_type=food** (the slug is **food**).[](https://board.support/media/docs/wp-slug.jpg)

#### Disable WordPress Emoji

The prevent WordPress from replacing the chat emiji with the WordPress ones Enter the code below in the file **functions.php** of your theme.

                                    function disable\_emojis() {
                                         remove\_action("wp\_head", "print\_emoji\_detection\_script", 7);
                                         remove\_action("admin\_print\_scripts", "'print\_emoji\_detection\_script");
                                         remove\_action("wp\_print\_styles", "print\_emoji\_styles");
                                         remove\_action("admin\_print\_styles", "print\_emoji\_styles");
                                    }
                                    add\_action("init", "disable\_emojis");
                                

#### WordPress Multisite

If you have multisite installation, you must install Support Board in the main website.

#### WordPress Multilingual

If you want the chat to use the same language as the pages on your website, disable the **Chat > Automatically translate option**

* * *

WOOCOMMERCE

## WooCommerce

The settings below are related to the WooCommerce App for the WordPress version of Support Board.

* * *

## Dialogflow

#### Getting started

To start using the Dialogflow chatbot go **Settings > WooCommerce > Dialogflow synchronization** and click **Synchronize entities now**, then click **Create Intents now**. Once the synchronization is completed you're done. The chatbot will start replying to the users' questions.

#### Built-in Intents questions list

By importing the built-in Intents the chatbot can answer the questions like the below ones. For the full list please visit the Intents area of the Dialogflow console.

+   Do you sell any shoes for less than $299?
+   Show me your bags
+   Do you have anything for women in promotion?
+   What are the best shoes of 2020?
+   Add Abstract Print to the cart
+   Remove Abstract Print from the cart
+   What do you sell

+   What's the status of my order?
+   Where my order will be shipped?
+   Display the products in my cart!
+   Do you ship in Australia?
+   Where do you ship?
+   Open the shoes page.
+   Go to the cashmere tank page, please.

* * *

#### Actions

The following actions allow the chatbot to interact with the shop autonomously on behalf of the user. To use an action go to Dialogflow, edit an **Intent**, and add a new **Custom Payload** response with the following syntax: **{ "ACTION-NAME": ACTION-VALUE }**.

| Action code | Description |
| --- | --- |
| 
{ "woocommerce-update-cart": \[ "cart-add", "PRODUCT-NAME-OR-ID" \] }

 | Adds a product to the user's cart. Replace PRODUCT-NAME-OR-ID with the ID or full name of a product. |
| 

{ "woocommerce-update-cart": \[ "cart-remove", "PRODUCT-NAME-OR-ID" \] }

 | Removes a product from the user's cart. Replace PRODUCT-NAME-OR-ID with the ID or full name of a product. |
| 

{ "woocommerce-checkout": true }

 | Redirects the user to the checkout page. |

#### Multilingual

+   The multilingual feature is compatible with WPML and Polylang plugins.
+   To activate the multilingual feature go to **Settings > WordPress > Multilingual plugin** and choose WPML or Polylang. The synchronization automatically creates the Entities in all available languages of your website. For a language to work, the chatbot must be translated into that language in Dialogflow, more details [here](https://cloud.google.com/dialogflow/es/docs/agents-multilingual).
+   The built-in Dialogflow Intents are only in English, to translate them go to your [Dialogflow Console](https://dialogflow.cloud.google.com/), choose the language you want to translate, go to the **Intents** page, and translate the existing WooCommerce Intents.
+   The multilingual feature for the WooCommerce **products attributes** requires the [WooCommerce Multilingual Plugin](https://wpml.org/documentation/related-projects/woocommerce-multilingual/?aid=154204&affiliate_key=LgJiCRvycckb) if you're using WPML, or [Polylang for WooCommerce Plugin](https://polylang.pro/downloads/polylang-for-woocommerce/) if you're using Polylang.

#### More information

+   If you edit an existing built-in WooCommerce Intent in Dialogflow and then you import again the intents from **Settings > WooCoommerce > Dialogflow synchronization** you will lose your customization. To keep your edits change the Intent name.
+   The chatbot can display up to 15 products via the slider rich message.
+   The chatbot is automatically updated every 60 min by default, but it can take longer. If you update a product, category, tag, or attribute, please wait a few hours for the new contents to take effect.
+   The synchronization detects the following events: product deleted, product restored from trash, product updated, new product added, product deleted, category or tag deleted, category or tag updated, new category or tag added.
+   To improve the chatbot add all the possible variants of an attribute, including the variants not used in your products. Example: if you sell only yellow and red t-shirts add all possible colors to the attribute color, not only yellow and red.
+   You can manually synch the chatbot at any time from **Settings > WooCommerce > Dialogflow synchronization**.
+   Products must have the **Regular price** attribute set.
+   Products names must not use the double-quote char: **"**.
+   Some multilingual feature is not compatible with **sub-domains** or **external domains** language URLs.

* * *

## Merge fields and shortcodes

The following merge fields and shortcodes can be used in emails and messages.

| Code | Description | Compatibility |
| --- | --- | --- |
| 
{product\_images}

 | Slider of product's images. If there are no results, the full message is replaced by "No results found". | Dialogflow |
| 

{shipping\_location\_check}

 | Check if the store ship in the given country. | Dialogflow |
| 

{product\_attribute\_terms}

 | Attribute terms list of a product's attribute. | Dialogflow |
| 

{product\_attribute\_name}

 | Attribute name of an attribute term. | Dialogflow |
| 

{category\_link}

 | Category page link. | Dialogflow |
| 

{tag\_link}

 | Tag page link. | Dialogflow |
| 

{product\_name}

 | Product name. | Dialogflow, Automated Messages |
| 

{product\_image}

 | Product image. | Dialogflow, Automated Messages |
| 

{product\_price}

 | Product price. | Dialogflow, Automated Messages |
| 

{product\_description}

 | Product description. | Dialogflow, Automated Messages |
| 

{product\_rating}

 | Product rating. If the product has no ratings yet, the full message is replaced by "\[product name\] has no ratings or reviews yet.". | Dialogflow, Automated Messages |
| 

{product\_link}

 | Product link. | Dialogflow, Automated Messages |
| 

{shipping\_locations}

 | List of the shipping countries. | Dialogflow, Messages, Automated Messages |
| 

{shop\_link}

 | Shop link. | Dialogflow, Messages, Automated messages |
| 

{cart\_link}

 | Cart link. | Dialogflow, Messages, Automated Messages |
| 

{cart}

 | List of the products in the user's cart. If the cart is empty, the full message is replaced by "Your cart is currently empty". | Dialogflow, Automated Messages |
| 

{order\_status}

 | Status of the last user's order. If the user has never placed an order, the full message is replaced by "You haven't placed an order yet". | Dialogflow, Automated Messages |
| 

{order\_details)

 | Details of the last order user's order. If the user has never placed an order, the full message is replaced by "You haven't placed an order yet". | Dialogflow, Automated Messages |
| 

{product\_card}

 | Product card. Optional attributes:

+   **id** The product ID.
+   **link-type** The action on user click. Available values: purchase, checkout, link. Default: purchase.
+   **link-text** The button text. Default: Purchase.

 | Dialogflow, Messages, Automated Messages |
| 

{products\_slider}

 | Search for the products matching the given attribures and display them in a slider of products cards. If there are no results, the full message is replaced by "No results found". Optional attributes:

+   **id** The products IDs separated by commas. If this attribute is setted, all other attrbutes are ignored.
+   **tag** Display only the products of the given tag.
+   **category** Display only the products of the given category.
+   **discounted** Set it to true to show only the products in promotions.
+   **rating** Display only the products with a rating equal or bigger than the given value. Enter a value from 1 to 5.
+   **max-price** Display only the products with a price equal or smaller than the given value. Enter a number.
+   **min-price** Display only the products with a price equal or bigger than the given value. Enter a number.
+   **attribute** Display only the products with the given attribute term.
+   **link-type** The action on user click. Available values: purchase, checkout, link. Default: purchase.
+   **link-text** The button text. Default: Purchase.
+   **language** The language code of the products to display.

 | Dialogflow, Messages, Automated Messages |
| 

{payment\_methods}

 | Available payment methods. | Dialogflow, Messages, Automated Messages |
| 

{coupon}

 | Generate a coupon code. Optional attributes:

+   **discount** The coupon discount in percentage.
+   **expiration** The coupon expiration. Example: '60 seconds', '5 hours', '2 days'.

 | Dialogflow, Messages, Automated Messages |
| 

{product\_names}

 | Products names. | Only where specified |
| 

{discount\_price}

 | Discounted product price or total discounted price of multiple products. | Only where specified |
| 

{original\_price}

 | Original product price or total original price of multiple products. | Only where specified |
| 

{carts}

 | Multiple users carts list with products. | Only where specified |
| 

{purchase\_button}

 | Purchase product button. | Only where specified |
| 

{html\_product\_card}

 | Product details card. | Email |
| 

{html\_products\_list} 

 | List of products details cards. | Email |

#### Rich Messages

| Shortcode | Description |
| --- | --- |
| 
\[woocommerce-button name="" ids="" coupon="" checkout="true"\]

 | Add a product or multiple products to the user's cart. Optionally apply a coupon code, and redirect the user to the checkout page. |

* * *

## More information

#### Waiting list

+   The message is sent automatically when a user visits a page of a product that's out of stock.
+   The message is sent automatically when a user tries to purchase a product that's out of stock via the chatbot.
+   The message is sent a maximum of 1 time every 24 hours for each out of stock product.
+   If the user'email is not set, the chat asks for the user' email automatically.

#### Removed item from cart notification

+   If the coupon is included, the chat message is sent only for the first removed item, then again after coupon expiration.
+   The coupon is valid only for the removed items.
+   The following merge fields can be used in the email subject too: {coupon}, {discount\_price}, {original\_price}, {product\_names}, {customer\_name}.
+   Only the users with an email will get notified via email.

#### Returning visitors notification

+   The chat message is sent after 15 seconds.
+   The chat message is sent to the active conversation, if any, otherwise to a new conversation.
+   A visitor is a "returning visitor" only if at least 24 hours have passed since the last visit.
+   The chat message is sent only 1 time, if the visitor returns again, the message is not sent.

#### Follow-up message

+   If the message contains a coupon, the message is sent only if there are no other valid coupons assigned to the user.

#### Miscellaneous

+   When a visitor completes a purchase, a new Support Board user with the details provided in the checkout form is automatically created.
+   The automatic messages(abandoned cart message, follow-up messages,...) are sent to the active conversation, if any, otherwise to a new conversation.
+   The default coupon values are 0% discount and 7 days expiration.
+   Coupons in the trash are still valid, you must permanently delete them.
+   All coupons can be used only 1 time.
+   Expired coupons are deleted automatically via cron jobs.
+   The products pop-up of the admin conversations area search by product name, description, and price.
+   The products pop-up of the admin conversations area is multilingual and displays automatically the products of the user's language if available.
+   To view orders of guest users who did not send any chat message before the purchase you need to enable **Settings > Users > Register all visitors**.
+   The setting **Ticket products selector > Exclude products** accepts WooCommerce product IDs separated by commas.

#### WhatsApp shop

To allow a user to purchase your WooCommerce shop products on WhatsApp the **product ID** of your WhatsApp shop products must be the same as the **product ID** of your WooCommerce products. Once the user has sent the WhatsApp order, WooCommerce automatically saves it, use the merge field **{catalog\_checkout}** to send the user the checkout link.

Use the plugin [https://wordpress.org/plugins/facebook-for-woocommerce/](https://wordpress.org/plugins/facebook-for-woocommerce/) to automatically synchronize the WooCommerce products with the WhatsApp shop products.

* * *

TICKETS

## Tickets

The settings below are related to the Tickets App.

* * *

## Installation and usage

#### PHP installation

To display the tickets area include the following script into your page.

                                <script src="supportboard/js/min/jquery.min.js"></script> <!-- Not required if jQuery is already loaded -->
                                <script id="sbinit" src="supportboard/js/main.js?mode=tickets"></script>
                            

+   You can not include both chat and tickets area on the same page. Make sure to remove the script that loads the chat. You can show the tickets area also by inserting the code **<script>SB\_TICKETS = true;</script>** into any page showing the chat.
+   To set the position of the tickets area Enter the code **<div id="sb-tickets"></div>**. The tickets area will be displayed inside this div element. By default, the tickets area is appended to the **body**.

* * *

#### WordPress installation

To display the tickets use the shortcode **\[sb-tickets\]**. Insert it in any page, post, or post type item.

#### Cloud version installation

To display the tickets area include the cloud chat script into your page and add the attribute **&mode=tickets** to the script URL, e.g. **<script id="chat-init" src="https://cloud.board.support/account/js/init.js?id=65895623&mode=tickets"></script>**. You can show the tickets area also by inserting the code **<script>SB\_TICKETS = true;</script>** into any page showing the chat.

[![](https://board.support/media/play-video.svg)](https://www.youtube.com/watch?v=RxKIOO9IUtA)

* * *

## Information

+   If the tickets area is not visible, make sure to uncheck the option **Tickets > Manual initialization**. Additionally, you can explore other potential reasons for this issue [here](#widget-hidden).
+   Tickets are the same of chat conversations and messages, the only difference from the chat is the front-end panel.
+   Most of the settings of the chat are compatible with the Tickets App but not all of them. The dashboard settings, the pop-up message, and more are not compatible.
+   Dedicated APIs for the Tickets App are available in the API section.
+   To remove the mandatory 'New ticket' form for new users, activate the welcome message of **Settings > Messages > Welcome message. The welcome message delay is ignored in the tickets area, the message is sent immediately.**.
+   To manually disable the mandatory registration only on a single page use the JavaScript code **var SB\_REGISTRATION\_REQUIRED = true**. Set it to **true** to force the registration instead.

* * *

WHATSAPP

## WhatsApp

The settings below are related to the WhatsApp app.

* * *

## Installation

+   From **Settings > Apps**, click **WhatsApp** and enter your license key to install and activate the app. If you have the cloud version the app is already active.

#### WhatsApp Cloud API Setup

+   Create a Developer account and a new Facebook app as described at [https://developers.facebook.com/docs/whatsapp/cloud-api/get-started#set-up-developer-assets](https://developers.facebook.com/docs/whatsapp/cloud-api/get-started#set-up-developer-assets).
+   In **Support Board > Settings > WhatsApp > Cloud API settings > Secret key** enter a random string then go to [https://developers.facebook.com/apps](https://developers.facebook.com/apps) and select your app. Click **Add product** and add **WhatsApp**, then go to **WhatsApp > Configuration** and in **Webhook URL** enter the URL you get from **Support Board > Settings > WhatsApp > Cloud API > Configuration URL**. In **Verify token** enter the secret key you previously entered in Support Board. Click **Verify** and save, click **Webhook fields > Manage**, enable the following Webhook fields: **messages**.[](https://board.support/media/docs/whatsapp-cloud-1.jpg)
+   To verify the integration, simply go to [https://developers.facebook.com](https://developers.facebook.com/) and select your app. From there, click on "WhatsApp" in the left menu and then select "API Setup". Copy the **Phone number ID** and paste it into **Support Board > Settings > WhatsApp > Cloud API settings > Phone number ID.** Enter the desired phone number in the "To" field, such as your personal WhatsApp number, and send a test message. Check your WhatsApp account and send a reply, which should then appear in Support Board. To reply to the test number from Support Board, copy the "Temporary access token" and paste it in **Support Board > Settings > WhatsApp > Cloud API settings > Token**.[](https://board.support/media/docs/whatsapp-cloud-3.jpg)
+   To activate the WhatsApp integration for all phone numbers and add a live phone number, refer to the following guidelines.  
    In **Support Board > Settings > WhatsApp > Cloud API settings > Token** enter the permanent access token, follow the instructions below for getting it.
    +   Visit [https://business.facebook.com](https://business.facebook.com/) and go to **Left menu > Settings > Business settings**, then go to **Users > System Users** to view your admin system user, or create a new one. Open the user and click **Add Assets**, then select the app used for the WhatsApp API integration and check **Develop App**, or **Full control**. The system user needs to be an admin. If you do not see the option, click **Business settings**.
    +   Click **Left menu > Apps** and under **Select Assets** and choose your app, enable **Develop App**, or **Full control** and save.
    +   From **Users > System Users** select the user you just creted and click **Generate New Token**, click **Apps** and select the app used for the WhatsApp API integration, set the **Token expiration** to **Never**, enable the following permissions: **whatsapp\_business\_management**, **whatsapp\_business\_messaging**, **business\_management**. Click **Generate Token** and save. Paste the token in **Support Board > Settings > WhatsApp > Cloud API > Token**.[](https://board.support/media/docs/whatsapp-cloud-2.jpg)
+   To add additional phone numbers, you can do so by visiting [https://developers.facebook.com](https://developers.facebook.com/), selecting your app, and navigating to **Left menu > WhatsApp > API Setup**. To get started, click on **Add phone number** at the bottom and follow the instructions provided. Please keep in mind that if you use your current WhatsApp business number in Support Board, it will no longer be usable with your WhatsApp Business app, and you will need to migrate it following [these](https://developers.facebook.com/docs/whatsapp/cloud-api/get-started/migrate-existing-whatsapp-number-to-a-business-account) instructions. After activating the number, copy the **Phone number ID** and paste it into **Support Board > Settings > WhatsApp > Cloud API settings > Phone number ID.**

[![](https://board.support/media/play-video.svg)](https://www.youtube.com/watch?v=QJ_xHLnwDks)

#### 360dialog Account Setup

+   Go to [https://www.360dialog.com/](https://www.360dialog.com/) and create a new account.
+   Enter your dashboard and from **Left menu > WhatsApp Accounts** generate the **API key** and copy and paste it in **Support Board > Settings > WhatsApp > 360dialog settings**.
+   Click **Support Board > Settings > WhatsApp > 360dialog settings > Synchronize now**.
+   Done! Support Board should start receiving the WhatsApp messages sent to your number, and you can reply to those messages from Support Board.
+   Note that you can also use the free sandbox account for testing, more details at [https://docs.360dialog.com/whatsapp-api/whatsapp-api/sandbox](https://docs.360dialog.com/whatsapp-api/whatsapp-api/sandbox). The sandbox account has limitations and some features, such as media attachments, will not work.

#### Twilio Account Setup

+   Go to [https://www.twilio.com](https://www.twilio.com/referral/5GOe1g) and create a new account.
+   Verify your phone number.[](https://board.support/media/docs/sms-1.jpg)
+   Complete the form and choose **WhatsApp**, **Alerts & Notifications**, **With no code at all**, **3rd party integrations**.[](https://board.support/media/docs/whatsapp-1.jpg)
+   From the [Twilio console](https://www.twilio.com/console) copy **ACCOUNT SID** and **AUTH TOKEN** and paste them into **Support Board > Settings > WhatsApp > Twilio settings**, save the changes.[](https://board.support/media/docs/whatsapp-2.jpg)
+   You will now set up a free test account to run some tests and make sure the integration works with Support Board. From the left menu click **Messaging > Settings > WhatsApp sandbox settings** and enter into **WHEN A MESSAGE COMES IN** and **STATUS CALLBACK URL** the URL of Support Board , get it from **Support Board > Settings > WhatsApp > Twilio settings > Get configuration URL**. Mind that localhost will not work, you need a public URL and a live server.[](https://board.support/media/docs/whatsapp-3.jpg)
+   From the left menu click **Messaging > Try it out > Send a WhatsApp message**. Follow the instructions and send the message with the code to the WhatApp number provided. Click the next buttons until the configuration is complete.[](https://board.support/media/docs/whatsapp-4.jpg)
+   Done! Support Board should start receiving the WhatsApp messages sent to the sandbox account, and you can reply to those messages from the Support Board.
+   To publicly use the WhatsApp integration with your customers you need to update your account and enable billing, you can do that [here](https://www.twilio.com/console/billing/upgrade). After that you will need to purchase a Twilio number, which will be the phone number of your official WhatsApp Business account. More details [here](https://www.twilio.com/docs/whatsapp/tutorial/connect-number-business-profile). You cannot use the phone number of your existing WhatsApp Business account, you must use a Twilio number. More details [here](https://support.twilio.com/hc/en-us/articles/360052171393-Can-I-activate-my-own-phone-number-for-WhatsApp-on-Twilio-).

#### Unofficial WhatsApp API

Support Boar only supports the Official WhatsApp Cloud API, 360dialog, or Twilio. Unfortunately, unofficial WhatsApp APIs are not supported. However, you can still implement them using the Support Board API and Webhooks. For more details, visit https://board.support/docs/api/web Please be aware that you must possess coding skills as a developer to proceed with this task. Additionally, our default integrations are equipped with advanced features including chatbot support, automated messages, human takeover, WhatsApp rich messages, attachments, and more. Consequently, although setting up a basic integration for sending and receiving text messages is relatively straightforward, ensuring its flawless functionality is a more intricate process. If you wish, you have the option to hire us; however, we are available only for developing a basic integration that enables two-way text messaging and attachments.

* * *

## Templates

As for [WhatsApp Business Policy](https://www.whatsapp.com/legal/business-policy/), you cannot send outbound marketing and solicitation messages to end users. End user users must reach out to you first. You have 24 hours from when the end user's message was sent from WhatsApp to reply to the message. To communicate with a user who has not contacted you before or has not been in touch for more than 24 hours, you must opt for the text message fallback or the WhatsApp message template.

#### Text message fallback

To enable the text message fallback you must set up the SMS in **Settings > Notifications > Text message notifications**.  
More details [here](#sms)

#### WhatsApp message templates

A WhatsApp message template is a message format that you can use over and over again to message users once they have opted-in and given your app permission to send them messages. You can not Enter the original message into the template, you must use it to notify the user of a new message and instruct him on how to view it, for example by providing a link to your website where the chat is shown.

##### WhatsApp Cloud API

+   To get the **Template name** and manage the templates visit [https://business.facebook.com](https://business.facebook.com/) and go to **Left menu > Settings > More system settings**, then go to **Accounts > WhatsApp accounts > Settings** and click **WhatsApp Manager**.
+   In **Template languages** enter all the language codes supported by your template, separated by commas. Language codes list [here](https://board.support/docs/files/language-codes.txt) (copy only the language code, e.g. it, es, en\_US). If you use a template that supports multiple languages, the matching language for the user will be automatically selected. Otherwise, the default template language will be used.
+   In **Header parameters** and **Body parameters** enter the supported merge fields separated by commas, e.g. {recipient\_name}, {conversation\_url\_parameter}. The number of parameters entered here must match the number of parameters of the template. Use this feature if your template uses dynamic values. Order is important, the first merge field will be used as the first template parameter.

##### Send template messages to a user who has not contacted you before

+   In **Settings > WhatsApp > Cloud API settings > Business Account ID** enter you **Business Account ID**. Provide your **Business Account ID**, which can be obtained from [https://developers.facebook.com](https://developers.facebook.com/). Choose your app and go to **Left menu > WhatsApp > API Setup**.
+   To send the template to specific users, go to the Support Board **Users** section and choose the intended recipients. Then, click on the WhatsApp icon located at the top right corner.
+   If you are using the WhatsApp Cloud API with a template that supports multiple languages, the matching language for the user will be automatically selected. Otherwise, the default template language will be used.
+   If you are using Twilio and have parameters in your template, input the parameter values separated by commas in the **Body** section.
+   For more details click [here](#direct-messages).

##### Twilio

Enter the template code into **Support Board > Settings > WhatsApp > Template fallback** If you're using the Twilio sandbox for testing you can use pre-approved templates like **Your {{1}} code is {{2}}**, you can replace the variables with the Support Board ones like **{recipient\_name}**, for example, **Your {recipient\_name} code is {recipient\_email}**. More details [here](https://www.twilio.com/docs/whatsapp/tutorial/send-whatsapp-notification-messages-templates).

##### 360dialog

+   Get the **Namespace** value from **Left menu > WhatsApp accounts > Details**.
+   Get **Template name** and **Template default language** from your 360dialog templates area.
+   In **Custom parameters** Enter the supported merge fields separated by commas, example: {recipient\_name}, {conversation\_url\_parameter}. Use this feature if your template uses dynamic values. Order is important, the first merge field will be used as the first template dynamic value.
+   Support Board will try to use the template with the same language as the user, if it is not available, it will use the template with the default language. The following template languages are not compatible: en\_GB(use en\_US), pt\_PT(use pt\_BR), zh\_HK and zh\_TW(use zh\_CN), es\_AR and es\_MX(use es\_ES).

* * *

## WhatsApp shop

To displays the products of your shop use the merge fields below.

| Merge field | Description |
| --- | --- |
| **{catalog id="123" product\_id="123" body="" footer=""}** | Display a single product. Replace **id** with the catalog ID and **product\_id** with a product ID. The attributes **body** and **footer** are optional. |
| **{catalog id="123" product\_id\_1\_1="123" product\_id\_1\_2="123" product\_id\_2\_1="123" section\_1="" section\_2="" header="" body="" footer=""}** | Display multiple products. Replace **id** with the catalog ID. Add products by grouping them into sections, via the attributes **product\_id\_\[A\]\_\[B\]**, replace \[A\] with the section index, starting from 1, replace \[B\] with the product index, starting from 1 for each section. You must also add the attribute **section\_\[A\]=""** for each section, replace \[A\] with the section index. The attributes **header** and **body** are required, **footer** is optional. |

* * *

+   When the user sends the order, the order information is sent to the URL specified in **Settings > WhatsApp > Order webhook**. The page at that URL should process the order and send a message to the user via the PHP API function **sb\_whatsapp\_send\_message()**.
+   To connect the shop to WooCommerce click [here](#woocommerce-whatsapp).

* * *

## More information

+   If you does not receive WhatsApp messages make sure you are not assigning the WhatsApp conversations to a department and that the WhatsApp number used for testing is not a phone number of a Support Board admin or agent. Also, make sure you setup correctly the WhatsApp webhook URL.
+   If you can not send messages, an error should appear in the admin area when you try to send a message to the user.
+   We cannot provide support for Twilio or 360dialog configuration, including all related issues.
+   We cannot provide support in getting your WhatsApp account or WhatsApp message template approved.
+   WhatsApp conversations and messages are compatible with routing and queue.
+   If you are testing with the sandbox and after 72 hours you can no longer send messages to your phone number you must link again your phone number to your sandbox.
+   You can send [rich messages](#rich-messages) to WhatsApp. If you send chips, buttons or select rich messages, with more than 3 options, you can use the **whatsapp="Your menu text"** shortcode attribute to set the text of the WhatsApp message menu.
+   The [follow-up message](#follow-up-message) is supported, but the delay setting is ignored, the message is sent instantly.
+   The [offline message](#offline-message) is supported, but the timetable is not sent.
+   The chatbot is supported. The [human takeover](#human-takeover) feature is supported.
+   The supported AI features include **language detetction**, **spelling correction**, **multilingual via translation**, **Google search**.

* * *

MESSENGER

## Messenger

The settings below are related to the Messenger app.

* * *

## Installation

+   From **Settings > Apps**, click **Messenger** and enter your license key to install and activate the app. If you have the cloud version the app is already active.
+   Once the App is installed go to **Settings > Messenger** and click **Start synchronization**.
+   Complete the synchronization by choosing at least 1 Facebook page and enter the returned information in Settings > Messenger > Facebook pages.
+   You're done. All messages sent to the Facebook pages and Instagram accounts you selected will appear in the conversation admin area of Support Board.

[![](https://board.support/media/play-video.svg)](https://www.youtube.com/watch?v=t7Lq73Dt7dU)

* * *

## Instagram

To link Instagram to your Facebook page and Support Board follow the steps below.

+   Enter the Settings area of your Facebook Page and click **Left Menu > Instagram** (https://www.facebook.com/YOUR-PAGE-SLUG/settings/).
+   Click **Connect account** and complete the setup.
+   Sync Messenger with Support Board again and you're done.

[![](https://board.support/media/play-video.svg)](https://www.youtube.com/watch?v=LoohtFpBs_o)

* * *

## More information

+   If you don't receive Instagram messages make sure to enable **Settings > Privacy > Messages > Connected tools - Allow access** from your Instagram mobile app. Also, make sure your Instagram account is not setup as a professional account, it must be a business account.
+   In case you encounter duplicated messages or an ongoing chat cycle between the chatbot and Instagram messages, you are facing a problem due to the presence of two Support Board installations or Support Board Cloud accounts that are both synchronized with the same Instagram account. To resolve this, access the second Support Board admin area, navigate to **Settings > Messenger > Facebook pages**, remove the **Instagram ID** value and save the changes.
+   Every Support Board user has only 1 Facebook and Instagram conversation.
+   Support Board [rich messages](#rich-messages) are automatically converted to Facebook rich messages when possible, some part of the rich message could be removed or changed.
+   Only private Facebook messages will get sent to your team inbox. If someone posts a Facebook message on your wall it won't appear in your team inbox.
+   When someone sends a message to your company Facebook page or Instagram account they will get designated as a lead in Support Board. You'll only be able to see the user's Facebook or Instagram name and profile picture.
+   Messenger conversations and messages are compatible with routing and queue.
+   The chatbot is supported. The [human takeover](#human-takeover) feature is supported.
+   The supported AI features include **language detetction**, **spelling correction**, **multilingual via translation**, **Google search**.
+   If the chatbot is enabled, it is necessary to deactivate any automatic replies on Facebook Messenger, such as the welcome message.
+   The [follow-up message](#follow-up-message) is supported, but the delay setting is ignored, the message is sent instantly.
+   The [offline message](#offline-message) is supported, but the timetable is not sent.
+   Only 1 Facebook account can be synchronized, to link pages from multiple Facebook accounts, the account synchronized in Support Board must be an admin of all Facebook pages of the other Facebook accounts.
+   Using this integration of Instagram and Facebook Messenger comes at no additional cost.
+   If the message exceeds 1000 characters, only the initial 1000 characters will be transmitted due to the character limit.

* * *

TWITTER

## Twitter

The settings below are related to the Twitter app.

* * *

## Installation

+   Register at [https://developer.twitter.com](https://developer.twitter.com/). Make sure to verify your phone at [https://twitter.com/settings/phone](https://twitter.com/settings/phone) or the registration will fail.
+   Create your first app by entering the app name and click**Get keys**, copy **API Key (Consumer key)** and **API Key Secret (Consumer secret)** and paste them in **Support Board > Settings > Twitter**.
+   Request the **Elevated** access from [https://developer.twitter.com/en/portal/products/elevated](https://developer.twitter.com/en/portal/products/elevated). Click **Apply for Elevated** and complete the form as follow: In the first area **In your words** and in **Will your app use Tweet, Retweet, Like, Follow, or Direct Message functionality?** enter **I need access to the Account Activity API to start receiving Twitter Direct Messages to my chat software(Support Board ) and to reply to them directly from Support Board , details at https://board.support/twitter.** Disable all the other fields by clicking No: Are you planning to analyze Twitter data?, Do you plan to display Tweets or aggregate data about Twitter content outside Twitter?, Will your product, service, or analysis make Twitter content or derived information available to a government entity?[](https://board.support/media/docs/twitter-1.jpg)
+   Wait a few days for Twitter to review and approve the Elevated access, you will receive an email from Twitter.
+   Once you have Elevated access, enter the developers dashboard ([https://developer.twitter.com/en/portal/dashboard](https://developer.twitter.com/en/portal/dashboard)) and from the left menu click **Products > Premium > Dev environments** and under **Account Activity API / Sandbox** click **Set up dev environment**, in **Dev environment label** enter **sb** or the same value entered in **Settings > Twitter > Synchronization > Dev environment label**.
+   Enter your app **Settings** area from **Left menu > Projects & Apps > Your project > Your app** and under **User authentication settings** click **Set up** and activate **OAuth 1.0a**. In **App permissions** check **Read and write and Direct message**, in **Callback URI / Redirect URL** enter the URL you get from **Support Board > Settings > Twitter > Get callback URL**, in **Website URL** enter your website URL.[](https://board.support/media/docs/twitter-2.jpg)
+   Enter your app **Keys and tokens** area from **Left menu > Projects & Apps > Your project > Your app > Keys and tokens** and under **Authentication Tokens** generate **Access Token and Secret**, copy and paste them in **Support Board > Settings > Twitter**.
+   Enter your Twitter profile username in **Support Board > Settings > Twitter > Your username**. Get it from your Twitter profile page, copy the name starting with @ or the URL part containing your username. Ex. [https://twitter.com/**SupportBoard1**](https://twitter.com/SupportBoard1).[](https://board.support/media/docs/twitter-3.jpg)
+   Save the Support Board settings and click the button **Support Board > Settings > Twitter > Subscribe** and you're done. All messages sent to your Twitter account will be received by Support Board.

* * *

## More information

+   If you receive duplicate messages, the Twitter account you are using for testing may be the same as the one you synced. Try sending a message from another Twitter account.
+   Use a live domain, localhost is not supported.
+   When a message is received from a Twitter user you may send up to 5 messages in response within a 24 hour window. No messages can be sent after 24 hours of receiving the Twitter message.
+   You can send maximum 3 or 4 attachments depending by the media type.
+   The following Support Board [rich messages](#rich-messages) are not supported: images slider, slider, card.
+   The chatbot is supported. The [human takeover](#human-takeover) feature is supported.
+   The supported AI features include **language detetction**, **spelling correction**, **multilingual via translation**, **Google search**.

* * *

GOOGLE BUSINESS MESSAGES

## Google Business Messages

The settings below are related to the Google Business Messages app.

* * *

## Installation

+   In **Support Board > Settings > Business Messages > Synchronization > Client token** enter a random string and save.
+   Open the Business Communications Console ([https://business-communications.cloud.google.com](https://business-communications.cloud.google.com/)) and sign in with your Business Messages Google account.
+   Click **Partner account settings** on top.
+   Configure the **Webhook** by entering the **Webhook URL** and the **Client token** and save the changes, get the values from **Support Board > Settings > Business Messages > Synchronization**.
+   Enter back into the Business Communications Console ([https://business-communications.cloud.google.com](https://business-communications.cloud.google.com/)) and open your partner account.
+   Click **Service account** from the left menu and create a new key, download the key and open it with a text editor such as Notepad, copy **private\_key**, **client\_email**, and paste the values in **Support Board > Settings > Business Messages > Synchronization**.
+   To test your agent visit [https://business-communications.cloud.google.com/console](https://business-communications.cloud.google.com/console/), click your brand to enter your brand **Overview** area, under **Agent information > Agent test URLs** click on the button suitable for your mobile device and open the link from your mobile device.
+   To create a live agent for a real location on Google Maps, open your partner account, create a new agent, add Google Maps locations from **Left menu > Locations**, complete all other information prompts and then verify and launch the agent from **Left menu > Verify** and **Left menu > Launch**.

* * *

## More information

+   The values of chips, buttons and select rich messages must have a maximum of 25 characters, and the maximum 13 values are allowed.
+   Avatar image must be a JPG image of 1024x1024px with a maximum size of 50KB.
+   Get the **Place ID** of your locations from the **Locations** page of the Business Communications Console.
+   The chatbot is supported. The [human takeover](#human-takeover) feature is supported.
+   The supported AI features include **language detetction**, **spelling correction**, **multilingual via translation**, **Google search**.

* * *

TELEGRAM

## Telegram

The settings below are related to the Telegram app.

* * *

## Installation

+   Go to the admin area of Support Board , then go to **Settings > Apps > Telegram**, and enter the **Envato purchase code** to install and activate the app. If you have the cloud version the app is already active.
+   Go here: [https://t.me/botfather](https://t.me/botfather).
+   If you have already created a Telegram bot in the past, type the command **/mybots** and open your bot, then click **API token**.
+   If you never created a Telegram bot before, type the command **/newbot** to create a new bot. The BotFather will ask you for a name and username, enter them and generate the authentication token. More details at [https://core.telegram.org/bots](https://core.telegram.org/bots).
+   Copy the token and paste it into **Support Board > Telegram > Token**, then click **Synchronize now**. Your website must use HTTPS (SSL certificate), HTTP is not supported.
+   You're done. All messages sent to your Telegram bot will appear in the conversation admin area of Support Board.

[![](https://board.support/media/play-video.svg)](https://www.youtube.com/watch?v=KMFC8aC3zS4)

* * *

## More information

+   Support Board [rich messages](#rich-messages) are automatically converted to Telegram rich messages when possible, otherwise they are removed from the message.
+   Telegram conversations and messages are compatible with routing and queue.
+   The chatbot is supported. The [human takeover](#human-takeover) feature is supported.
+   The supported AI features include **language detetction**, **spelling correction**, **multilingual via translation**, **Google search**.
+   The [follow-up message](#follow-up-message) is supported, but the delay setting is ignored, the message is sent instantly.
+   The [offline message](#offline-message) is supported, but the timetable is not sent.
+   You can verify the webhook status from [https://api.telegram.org/bot><your\_bot\_token>/getWebhookInfo](https://api.telegram.org/bot%3Cyour_bot_token%3E/getWebhookInfo). Replace **<your\_bot\_token>** with your token.

* * *

VIBER

## Viber

The settings below are related to the Viber app.

* * *

## Installation

+   From **Settings > Apps**, click **Viber** and enter your license key to install and activate the app. If you have the cloud version the app is already active.
+   Create the bot at [https://partners.viber.com/account/create-bot-account](https://partners.viber.com/account/create-bot-account).
+   Copy the token and paste it into **Support Board > Viber > Token**, then click **Synchronize now**. Your website must use HTTPS (SSL certificate), HTTP is not supported.
+   You're done. All messages sent to your Viber bot will appear in the conversation admin area of Support Board.

* * *

## More information

+   Support Board [rich messages](#rich-messages) are automatically converted to Viber rich messages when possible, otherwise they are removed from the message.
+   Viber conversations and messages are compatible with routing and queue.
+   The chatbot is supported. The [human takeover](#human-takeover) feature is supported.
+   The supported AI features include **language detetction**, **spelling correction**, **multilingual via translation**, **Google search**.
+   The [follow-up message](#follow-up-message) is supported, but the delay setting is ignored, the message is sent instantly.
+   The [offline message](#offline-message) is supported, but the timetable is not sent.

* * *

SLACK

## Slack

The settings below are related to the Slack App.

* * *

## Synchronization

To sync Slack click the button **Start synchronization** of the **Settings > Slack** area and follow the instructions.

[![](https://board.support/media/play-video.svg)](https://www.youtube.com/watch?v=OYw1BGPu3IA)

#### Having Problems?

The synchronization of Slack may not be successful for a number of reasons; below are the most common ones:

| Problem description | Solution |
| --- | --- |
| You can receive messages on Slack, but you cannot send messages from Slack to Support Board | Navigate to **/supportboard/apps/slack/post.php** from your browser. If you receive a **403 - Forbidden** error, you will need to contact your web hosting provider and ask them to set the correct file permissions for this file and/or to add a Firewall role to prevent the firewall from blocking the file. It must be allowed to be executed freely without any restrictions. Also, in **Workspace Settings > Permissions**, you must allow anyone to create public channels. [](https://board.support/media/docs/slack-info-1.jpg)If you have further issues please contact the Slack support team at [https://api.slack.com/support](https://api.slack.com/support). |
| Slack sync not working | Double check whether or not you chose a public Slack channel when you attempted to synchronize Slack. If you did not, try syncing Slack once again, this time choosing a public channel instead. The general channel is a good option. |

#### Manually archive channels

To archive a channel in Slack, follow these steps:

+   Open the Slack channel you want to archive.
+   On the top right click the gear icon and select **Additional options**.[](https://board.support/media/docs/slack-archive-1.jpg)
+   Click the info icon in the top right area of the screen, then click the **More icon**, and then click **Additional options...**. Click **Archive this channel**.[](https://board.support/media/docs/slack-archive-2.jpg)

#### Departments linking

If the setting **Settngs > Slack > Departments linking** is active, when a conversation in the Support Board is assigned to a department, a new message is sent to the linked Slack channel, informing Slack users that a new conversation has started and inviting them to join the dedicated user Slack channel. However, the full conversation can only be accessed on the dedicated Slack channel of the specific user.

+   Get the department IDs from **Settings > Miscellaneous > departments**.
+   Get the channel IDs by clicking the button **Get channel IDs**.

#### User fields

The setting **Settings > Slack > User fields** allows you to choose which user details to include in the message sent to the main channel when a new user sends the first message. You can include the slug of your custom user details or the following slugs: **browser**, **browser\_language**, **location**, **email**, **user\_type**, **token**, **creation\_time**, **country\_code**, **current\_url**, **os**, **city**, **address**, **postal\_code**, **phone**, **birthdate**, **company**, **timezone**, **website**. Default: email, browser, browser\_language, location.

#### Information

+   When a new user sends the first message, a Slack message with the user details and a button to join the user's channel is sent to the main channel selected during the synchronization, or to the channel linked to the conversation's department. Only the Slack account used during the synchronization will automatically join the user's channel, other Slack members will have to join it manually via the button.
+   When **Settings > Slack > Agent linking** is set, if the conversation is assigned to a department, only agents assigned to that department will receive the message, if the conversation is assigned to a single agent only that agent will receive the message.
+   Slack is free to use. Only large companies may need a paid subscription plan, more details [here](https://slack.com/intl/en-gb/pricing).
+   Push notifcations are compatible with Slack, when agents send messages via Slack, Push notifications are sent to users.
+   If you're using Dialogflow, no messages will be received in Slack if the chatbot knows the answer. Once the human takeover is active all conversation's messages are sent to Slack.
+   The Slack app is compatible with email piping and the messaging apps.
+   Deleting or leaving a channel is not supported, only archiving a channel is supported.
+   When a conversation is archived in Support Board , the linked Slack channel is also archived.
+   When replying via Slack to a user, if the user is notified by email or text message, a Slack message is sent to notify you.
+   Use the Slack command **/archive** to archive a conversation from Slack.

* * *

PERFEX CRM

## Perfex

The settings below are related to the Perfex app.

* * *

## Installation

The installation requires two steps:

+   From **Settings > Apps**, click **Perfex** and enter your Envato purchase code to install and activate the app. Once the App is installed go to **Settings > Perfex** and enter the database information and the Perfex URL. You can get the information from the file **application/config/app-config.php** in your Perfex installation folder. If you do not know the Perfex prefix leave it empty, the default prefix is **tbl**.
+   Go to the admin area of Perfex, then go to **Setups > Modules** and install the Support Board module by uploading the file **module.zip**. Once the module is installed go to **Setups > Support Board** and enter the Support Board plugin URL, get it from **Settings > Miscellaneous > Support Board URL**. If you're using the WordPress version, the URL must be like this: **https://example.com/wp-content/plugins/supportboard/supportboard**.

To show Support Board inside the Perfex admin area, Support Board must be installed in the same domain and same file system of the Perfex installation. If you have issues, or if you have changed the Perfex database details, make sure the file **supportboard/config.php** use the correct Perfex database details. Updating the details in Support Board will not update the details in the config.php file.

* * *

Zendesk

## Zendesk

The settings below are related to the Zendesk App.

* * *

## Installation

+   Get the **domain** from the URL of your Zendesk admin area, copy the first part of the URL: https://**domain**.zendesk.com/. For example, the domain of **https://supportboard.zendesk.com/agent/get-started/ticketing-system/ticketing-intro** is **supportboard**.
+   Get the **API key** from **Left menu > Admin > Channels > API > Settings**. Click **Add API token**.[](https://board.support/media/docs/zendesk-1.jpg)
+   The **email** is your Zendesk account email.

* * *

## More information

+   Tickets converted by Support Board are automatically synchronized when new messages are sent and received in Support Board , and they are linked to an existing Zendesk user if any, otherwise a new Zendesk user is created.
+   Support Board links Zendesk users to Support Board users via email or phone number.

* * *

WHMCS

## WHMCS

The settings below are related to the WHMCS App.

* * *

## Installation

The process requires two installations, one is the WHMCS add-on, and one is the Support Board App.

#### App installation

+   Go to the admin area of Support Board , then go to **Settings > Apps > WHMCS**, and enter the **License Key** to install the app. Once the App is installed go to **Settings > Whmcs** and enter the database information and the WHMCS URL.

#### WHMCS add-on installation

+   Enter the folder **supportboard** inside the **addon.zip** (download it [here](https://board.support/docs/files/whmcs/addon.zip)) file into the **/modules/addons/** directory of your WHMCS installation.
+   Go to **Configuration > System Settings > Addon Modules**, find the Support Board module, and click **Activate**. More details at [https://docs.whmcs.com/Addon\_Modules\_Management#Installing\_An\_Addon](https://docs.whmcs.com/Addon_Modules_Management#Installing_An_Addon)
+   Click the **Configure** button and enter the Support Board plugin URL.

#### How to update

Updating the WHMCS App in Support Board is easy, you can enable the automatic updates or manually update it. Details [here](#updates). To update the WHMCS add-on you will need to download the latest version of the add-on from [https://board.support/docs/files/whmcs/addon.zip](https://board.support/docs/files/whmcs/addon.zip) and manually replace the **/modules/addons/supportboard/** directory of your WHMCS installation with the new one just downloaded.

If you have issues, or if you have changed the WHMCS database details, make sure the file **supportboard/config.php** use the correct WHMCS database details. Updating the details in Support Board will not update the details in the config.php file.

* * *

ULTIMATE MEMBERSHIP PRO

## Ultimate Membership Pro

The settings below are related to the Ultimate Membership Pro app.

* * *

## Users synchronization

New users are synchronized automatically. To manually syncronize existing users go to **Settings > WordPress > Synchronize users** and click **Import users**.

* * *

## More information

+   To limits the access to a specific plan only use this shortcode **\[ihc-hide-content ihc\_mb\_type="show" ihc\_mb\_who="4" ihc\_mb\_template="2"\]<script id="sbinit" src="YOUR-URL/supportboard/supportboard/js/main.js"></script>\[/ihc-hide-content\]** Replace **4** with the user's level you want and **YOUR-URL** with your WordPress /plugins/ folder URL. You also have to check **Settings > WordPress > Manual init**.

* * *

ARMEMBER

## ARMember

The settings below are related to the ARMember app.

* * *

## Users synchronization

New users are synchronized automatically. To manually syncronize existing users go to **Settings > WordPress > Synchronize users** and click **Import users**.

* * *

## More information

+   A user is a paid member only if it has at least one active paid plan which is not expired.

* * *

Active eCommerce

## Active eCommerce

The settings below are related to the Active eCommerce app.

* * *

## Installation

The process requires two installations, one is the Support Board App, and one is the installation in Active eCommerce.

#### App installation

+   Go to the admin area of Support Board , then go to **Settings > Apps > Active eCommerce**, and enter the **License Key** to install the app. Once the App is installed go to **Settings > Active eCommerce** and enter the database information, the Active eCommerce URL, and the other settings.
+   The Secret key can be found in the file **.env** located in the root directory of Active eCommerce. Copy the APP\_KEY value.[](https://board.support/media/docs/active-ecommerce-env.jpg)
+   If you have issues, make sure the file **supportboard/config.php** use the correct Active eCommerce database details.

#### Installation in Active eCommerce

+   Edit the file **\\resources\\views\\frontend\\inc\\footer.blade.php** in the directory of Active eCommerce and Enter the code below just after the footer opening tag **<footer**. Replace **\[YOUR-SITE\]** with the URL of your Support Board installation, get it from **Settings > Miscellaneous > Support Board URL**.[](https://board.support/media/docs/active-ecommerce-footer.jpg)

                                <script src="https://\[YOUR-SITE\]/js/min/jquery.min.js"></script>
                                <script id="sbinit" src="https://\[YOUR-SITE\]/js/main.js"></script>
                                @php
                                $sb\_code = '';
                                $sb\_cart = false;
                                if (Auth::check() && !isAdmin()) $sb\_code = 'var SB\_AECOMMERCE\_ACTIVE\_USER = '. Auth::user()->id. ';';
                                if (isset($detailedProduct)) $sb\_code.= 'var SB\_DEFAULT\_AGENT = "aecommerce-'. $detailedProduct->user->id. '";';
                                if (auth()->user() != null) $sb\_cart = \\App\\Models\\Cart::where('user\_id', Auth::user()->id)->get(); else { $temp\_user\_id = Session()->get('temp\_user\_id'); if ($temp\_user\_id) { $sb\_cart = \\App\\Models\\Cart::where('temp\_user\_id', $temp\_user\_id)->get(); }}
                                if ($sb\_cart && count($sb\_cart) > 0) { $sb\_code.= 'var SB\_AECOMMERCE\_CART = \['; foreach ($sb\_cart as $key => $item) { $sb\_code.= '\["'. $item\['product\_id'\]. '", "'. $item\['price'\]. '", "'. $item\['quantity'\]. '"\],'; } $sb\_code = substr($sb\_code, 0, -1). '\];'; }
                                if ($sb\_code != '') echo '<script>'. $sb\_code. '</script>';
                                @endphp
                            

#### How to update

Updating the Active eCommerce App in Support Board is easy, you can enable the automatic updates or manually update it. Details [here](#updates). If you update Active eCommerce, you will need to insert again the code above in the file **footer.blade.php**.

* * *

## Sellers chat

To force sellers to see only the conversations of users writing from their product pages enable the option **Settings > Miscellaneous > Hide conversations of other agents**. After that, just click the button **Settings > Active eCommerce > Import vendors** and you're done! The sellers will be registered in Support Board and can log in to the admin area.

Admins can always see the conversations of all agents(sellers).

* * *

Martfury

## Martfury

The settings below are related to the Martfury app.

* * *

## Installation

+   Go to the admin area of Support Board , then go to **Settings > Apps > Martfury**, and enter the **License Key** to install the app.
+   Once the app is installed go to **Settings > Martfury** and enter the **database information**, **Martfury URL**, **Secret key**. Get the information from the **.env**file located in the root directory of Martfury.
+   Set the Martfury path in **Settings > Martfury > Martfury path**. Get this information by uploading [this file](https://board.support/docs/files/path.zip) in the **/public/** folder of the root directory of Martfury, after the upload open it via browser (e.g. https://shop.com/public/path.php).
+   To show the chat on the website enter the Support Board code of the [PHP installation](#installation) into **Martfury Admin > Appearance > Custom JS > Footer JS**. Do not include jQuery.
+   If you have issues, make sure the file **supportboard/config.php** use the correct Martfury database details.

#### How to update

Updating the Martfury App in Support Board is easy, you can enable the automatic updates or manually update it. Details [here](#updates).

* * *

## Sellers chat

To force stores to see only the conversations of users writing from their product pages follow the steps below.

+   Check the options **Settings > Martfury > Private chat**, **Settings > Chat > Disable dashboard**, **Settings > Chat > Allow only one conversation**.
+   From **Settings > Martfury > Import vendors** import all vendors.
+   In **Settings > Martfury > Private chat linking** each each vendor to the correct store. You can get the vendor IDs from **Users > Agents and Admins**.

* * *

LINE

## LINE

The settings below are related to the LINE app.

* * *

## Installation

+   Login at [https://developers.line.biz/console/](https://developers.line.biz/console/) or create a new account.
+   Create a new **Provider** and then a new **Messaging API channel**, select **Messaging API** as channel type
+   From the channel **Basic settings** area copy **Channel secret** and paste it into **Support Board > Settings > Line > Synchronization > Channel secret**.
+   From the channel **Messaging API** area generate a **Channel access token (long-lived)**, copy it and paste it into **Support Board > Settings > Line > Synchronization > Access token**.
+   Enter your Webhook URL into **Webhook URL** and click **Verify**. Get the Webhook URL from **Support Board > Settings > Line > Synchronization > Webhook URL**.
+   Enable **Use webhook**.
+   Scan the **QR code** with your LINE mobile app to start writing to your channel.
+   Disable the **Auto-reply messages** setting.
+   You're done. All messages sent to your LINE bot account will appear in the conversation admin area of Support Board.

* * *

## More information

+   You have 7 days from when the end user's message was sent from WhatsApp to reply to the message.
+   Stickers are not supported.
+   Support Board [rich messages](#rich-messages) are automatically converted to LINE rich messages when possible, otherwise they are removed from the message.
+   LINE conversations and messages are compatible with routing and queue.
+   The chatbot is supported. The [human takeover](#human-takeover) feature is supported.
+   The supported AI features include **language detetction**, **spelling correction**, **multilingual via translation**, **Google search**.
+   The [follow-up message](#follow-up-message) is supported, but the delay setting is ignored, the message is sent instantly.
+   The [offline message](#offline-message) is supported, but the timetable is not sent.

* * *

WECHAT

## WeChat

The settings below are related to the WeChat app.

* * *

## Installation

+   From **Settings > Apps**, click **WeChat** and enter your license key to install and activate the app. If you have the cloud version the app is already active.
+   Visit [https://mp.weixin.qq.com/cgi-bin/readtemplate?t=register/step1\_tmpl&lang=en\_US](https://mp.weixin.qq.com/cgi-bin/readtemplate?t=register/step1_tmpl&lang=en_US) and register a **Service account**.
+   After the registration enter **Official accounts** area and from the left menu click **Settings and development > WeChat verification**. You must complete the verification, it takes a few weeks and costs USD 99, or CNY 300 for chinese entities.
+   From the left menu click **Settings and development > Basic configuration** and copy **Developer ID(App ID)**, **Developer Password(App Secret)**. Paste the information into **Support Board > Settings > WeChat**.
+   From the left menu click **Settings and development > Basic configuration** and complete the server configuration (服务器配置(已启用). In **Server Address(URL)** enter the URL you get from **Support Board > Settings > WeChat > Synchronization > Get configuration URL**. In **Token** insert any value you want, the same value must be entered in **Support Board > Settings > WeChat > Token**.
+   You're done. All messages sent to your WeChat account will appear in the conversation admin area of Support Board.

* * *

## More information

+   If you receive an error like **{"errcode":41001,"errmsg":"access\_token missing rid: 631111-470b3b22-48553870"}** you need to whitelist your server IP address from **Official Account > Settings and Development > Basic Configuration > IP whitelist**.
+   WeChat files and location attachments are not supported and are not received by Support Board.
+   Links are not supported in WeChat, they are converted to texts.
+   Support Board [rich messages](#rich-messages) are automatically converted to WeChat rich messages when possible, otherwise they are removed from the message.
+   WeChat conversations and messages are compatible with routing and queue.
+   The chatbot is supported. The [human takeover](#human-takeover) feature is supported.
+   The supported AI features include **language detetction**, **spelling correction**, **multilingual via translation**, **Google search**.
+   The [follow-up message](#follow-up-message) is supported, but the delay setting is ignored, the message is sent instantly.
+   The [offline message](#offline-message) is supported, but the timetable is not sent.

* * *

MISCELLANEOUS

## Miscellaneous

This section contains help for other features not listed above.

* * *

## Progressive Web App

The Support Board admin area is a PWA, which means that you can install it on desktop, Mac, iPhone, or mobile devices and use it like a fully-functional app. Note: This feature is optimized for Google Chrome and Safari.

#### Desktop installation

Enter in your admin area (e.g. https://www.your-site.com/supportboard/admin.php), and click the **+** icon on the top right of the URL bar of your Chrome browser.[](https://board.support/media/docs/pwa.jpg)

#### Mobile installation - Android - Cloud version only

If you are using the cloud version of Support Board on Android you can use the apps available on Google Play.

[Google Play](https://play.google.com/store/apps/details?id=support.board.cloud.twa)

#### Mobile installation - Android and Windows - All versions

+   Enter in your admin area with Google Chrome (e.g. https://www.your-site.com/supportboard/admin.php or https://cloud.board.support/)
+   Open your browser's settings.
+   Scroll down and tap **Add to Home screen.**
+   Confirm by tapping Add.

#### Mobile installation - iPhone or Mac - All versions

+   Enter in your admin area with Safari (e.g. https://www.your-site.com/supportboard/admin.php or https://cloud.board.support/)
+   Press the **Share** button and select **Add to Home Screen** from the popup.
+   Tap **Add** in the top right corner to finish installing the PWA.

#### WordPress installation

To install the PWA on WordPress, you need to access the admin area directly by going to:

\[SUPPORT-BOARD-URL\]/admin.php

Replace **\[SUPPORT-BOARD-URL\]** with your Support Board URL, get it from **Settings > Miscellaneous > Support Board URL**.

#### Change PWA icon and name

Download the file **manifest.json** [here](https://board.support/docs/files/manifest.json). Edit it and replace **YOUR NAME** with your brand name, **YOUR NAME DESCRIPTION** with any text you want, and **example.png** with the relative URL of your icon, the icon size must be 512 x 512 px. After you finished editing the file move it into the Support Board installation folder, the same folder where is located the file admin.php. Mind that because this is customization our support doesn't cover it, if you need help you can [hire us](https://board.support/hire-us).

* * *

## Keyboard shortcuts

Admin area keyboard shortcuts are enabled on both PC and MAC and work as follows:

| Shortcut | Description |
| --- | --- |
| 
ENTER

or

SPACE

 | Confirm or close a dialog alert; the same as clicking **OK**. |
| 

ESC

or

CANCEL

 | Decline a dialog alert and close it. |
| **SHIFT + ENTER** or

CTRL + ENTER

 | Add a line break to a message. This only works for the admin editor. |
| 

ESC

 | Close a lightbox. |
| 

CANCEL

 | In the admin conversations area, archive a conversation, or delete it. |
| 

CTRL + UP/DOWN ARROW

 | In the admin conversations area, navigate between the conversations of the list. |
| 

CTRL + RIGHT/LEFT ARROW

 | In the admin users area, navigate between the users. |
| 

CTRL + V

 | Paste an image from the clipboard and send it as message. |
| 

CTRL + Left mouse click

 | To perform actions like archiving, deleting, marking as read, or marking as unread on conversations in the admin area, press and hold the CTRL button while selecting them from the list on the left. |

* * *

## Config file

The **config.php** file is a special file that contains the MySQL database log-in details and other import settings. Most of the settings are generated automatically, but some are optional. You can add the following settings below:

| Code | Description |
| --- | --- |
| 
define('SB\_UPLOAD\_URL', 'YOUR-URL')

 | Change the uploads directory (the default directory is: /supportboard/uploads/). Enter a URL: for example, https://your-site.com/myuplaods/. For this setting you need also to define the SB\_UPLOAD\_PATH. |
| 

define('SB\_UPLOAD\_PATH', 'YOUR-PATH')

 | Change the uploads directory path (the default path is: /supportboard/uploads/). Enter a PATH: for example, C:\\xampp\\htdocs\\uploads. Finding the root path of your website can be a bit tricky. You can try copying the path displayed in your FTP client or simply contact your web hosting provider for additional support. |
| 

$GLOBALS\['SB\_LOCAL\_SETTINGS'\] = \[\]

 | Overwrite the default settings. The value is an array of keys and values, each key is a setting, e.g. **\["registration-required" => \[true\]\]**. View an example [here](https://board.support/docs/files/settings.txt). Get the settings list from **resources/json/settings.json** and the files **settings.json** inside the app folders. |

* * *

## Cron Jobs

+   Cron jobs are executed by the first user that visit the website at any given hour of the day.
+   Cron jobs are executed every 60 minutes, but it can take longer, or it can take less time as well, in relation to the traffic of your website.
+   Because cron jobs are initiated by users, if you have less than 1 visitor per minute, it could take longer. As long as there is at least one active user on the site, execution every minute is guaranteed.
+   You can speed up the cron jobs execution by manually run them via [WEB API](https://board.support/docs/api/web#cron-jobs), or [PHP API](https://board.support/docs/api/php#cron_jobs).

* * *

## Logs

+   The log file is saved in the Support Board installation directory.
+   The logs record the following actions of agents and administrators: message sent, message deleted, conversation archived, conversation deleted, conversation restored, conversation assigned to an agent, conversation assigned to a department, user updated, user deleted.

* * *

## URL parameters

#### Front-end chat

URL parameters allow the chat to perform specific actions on page load. To use them, append the URL parameters below to any URL on your website that displays the chat. Ex. https://example.com/?conversation=1234

| URL parameter | Description |
| --- | --- |
| 
?token=TOKEN

 | Login an existing user. Replace TOKEN with the user's token. |
| 

?conversation=ID

 | Open a conversation. Replace ID with the conversation ID. The attribute **token** is required for not logged in users. |
| 

?chat=open

 | Open the chat. |

#### Admin area

URL parameters allow the administration area to perform specific actions on page load. To use them, append the URL parameters below to your admin URL. Ex. https://example.com/supportboard/admin.php?conversation=1234

| URL parameter | Description |
| --- | --- |
| 
?conversation=ID

 | Open a conversation of the conversations area. Replace ID with the conversation ID. |
| 

?user=ID

 | Open the profile box of a user. Replace ID with the user ID. |
| 

?setting=ID

 | Open a setting of the settings area. Replace ID with the setting ID. |
| 

?report=ID

 | Open a report of the reports area. Replace ID with the report ID. |
| 

?area=name

 | Open an area of the admin. Replace name with: conversations, users, settings, reports. |

* * *

## Calendly

Follow the steps below to send a Calendly booking invitation.

+   Create an event type from [https://calendly.com/event\_types/user/me](https://calendly.com/event_types/user/me).
+   Click **share** and copy the URL.[](https://board.support/media/docs/calendly-1.jpg)
+   To send the Calendly invitation, utilize the [rich message](#rich-messages) **button** type. Ensure to enter the Calendly URL you copied in the previous step as the URL. Additionally, include the **success** attribute to customize the message that will be sent after the booking is successfully completed. E.g. **\[button link="https://calendly.com/federicoschiocchet/sb" name="Schedule a meeting" success="Thank you! Your meeting has been scheduled."\]**

* * *

## Zapier

Integrate Zapier with Support Board by following the steps below. Integration is based on the Support Board webhooks, each webhook is a Zapier trigger, so you have 15+ Zapier triggers available, for more details visit the [webhooks](https://board.support/docs/api/web#Webhooks) page.

+   Go to [https://developer.zapier.com/](https://developer.zapier.com/) and login, or register a new account.
+   Create a new integration by clicking **Start a Zapier Integration**, or visit [https://developer.zapier.com/app/new](https://developer.zapier.com/app/new). Fill in all required fields, like name and description, and click **Create**, you can enter any text you want, but keep the name of the app in mind because you will need it later.
+   From the left menu click **Triggers** and then **Add Trigger**.
+   Fill in all required fields, like key and description, and click **Save And Continue**, you can enter any text you want.
+   On top click **API Configuration**, choose **REST Hook** as **Trigger Type**, and click **Save**.
+   Go back to the **Settings** area of the trigger, or go to [https://zapier.com/app/zaps](https://zapier.com/app/zaps), and click **Create a Zap**.
+   Search for your newly created app by entering the app name and click it. In **Trigger Event** select your trigger and click **continue**.
+   Copy the **Webhook URL**, click **Continue**, and then enter the Support Board admin area and enter it into **Settings > Miscellaneous > Webhooks > URL**, activate the webhooks, save the settings and reload Support Board.
+   Make something to trigger a webhook like sending a message, or creating a new user, then go back to Zapier and click **Test Trigger** and you should see the Support Board webhook data. Click **Continue**.
+   Click the right button **Filters** and set up the filter in order to trigger the integration only if a variable exists. You need the filter because Support Board will send all webhooks to all zaps. Example: if your zap wants to integrate the messages of Support Board , you will need to set the filter to continue only if the variable **message** exists.
+   Click **Continue**, or **+** and add your integration.
+   To use multiple zaps and webhooks you will need to update **Settings > Miscellaneous > Webhooks > URL** and add the new zap IDs, separated by commas. Example: if you have two zaps with URLs **https://hooks.zapier.com/hooks/catch/10352851/bbad21f/** and **https://hooks.zapier.com/hooks/catch/10352851/aaaa66t/**, the URL must be **https://hooks.zapier.com/hooks/catch/10352851/bbad21f,aaaa66t/**.

* * *

## Envato purchase code validation

+   Get the **token** from [https://build.envato.com/create-token](https://build.envato.com/create-token/). Select the following scopes: **View and search Envato sites**, **View the user's items' sales history**, **Verify purchases of the user's items**, **Verify purchases the user has made**, **View the user's purchases of the app creator's items**
+   Add multiple product IDs, separated by commas.

* * *

## Security

Security is critical here at Support Board. We work with security experts who perform periodic security audits. We continually implement the latest security technologies and stay up-to-date on the latest security threats. Find below some of the security measures that have been implemented in Support Board.

#### IP ban

Support Board permits a maximum of 10 unsuccessful login attempts within an hour. In case the limit is exceeded by a user, admin, or agent, they will be unable to access their account or the admin area for a period of 1 hour. This blocking mechanism is based on the user's IP address and serves to deter brute force attacks aimed at uncovering login credentials. If you encounter the "Too many login attempts. Please retry again in a few hours." error, you have two options: either wait for a few hours or make changes to the Support Board database by deleting the **ip-ban** row from the **sb\_settings** table.

#### XSS injection protection

To prevent XSS injection protection attacks, all sensitive user inputs undergo sanitization.

#### Cross-Site Request Forgery (CSRF) protection

To prevent CSRF attacks, all requests are validated by checking the login cookie and the client-side login string.

#### Active sessions termination on user update

Whenever the password or the details for an admin or agent is changed, all active sessions are automatically logged out when sensitive operations are executed or after 1 hour.

#### AES-256-bit encryption

We use 256-bit AES encryption to encrypt sensitive data such as active session login data.

#### Password by filename protection

Support Board ensures that all uploads are renamed with a random alphanumeric string prepended to the original file name to prevent discovery of the URL and unauthorized download of the uploaded file. Kindly note that, for this feature to function properly, your server must prohibit directory listing.

* * *

## More Information

+   The uploads folder location is **supportboard/uploads** by default for the PHP version, while for the WordPress version it is **wp-content/uploads/sb**. You can customize it from the [config](#config) file. You can also upload files to [AWS S3](#aws).
+   If you change the plugin folder name after the installation, you need to update it in the constant **SB\_URL** of the file **config.php**.
+   The Users and Conversations sections in the Support Board admin area use auto-pagination on scroll, which is limited to 100 results per scroll.
