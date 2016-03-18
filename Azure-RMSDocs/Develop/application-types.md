Application types
===========================================================

This topic covers types of applications that you might choose to create as rights-enabled.

The following application types are currently supported by Rights Management Services SDK 2.1

<span id="Simple_applications"></span><span id="simple_applications"></span><span id="SIMPLE_APPLICATIONS"></span>Simple applications
-------------------------------------------------------------------------------------------------------------------------------------

A simple application could be a command line tool built to encrypt a provided file. For an example of a simple, rights-enabled application see, [IPCHelloWorld - an example application](how_to_build_your_first_application.md).

<span id="Server_mode_applications"></span><span id="server_mode_applications"></span><span id="SERVER_MODE_APPLICATIONS"></span>Server mode applications
---------------------------------------------------------------------------------------------------------------------------------------------------------

*Server mode* is meant for non-interactive applications that consume, protect or process RMS-protected content. An example would be a *Data Loss Prevention* application that runs as a service on a file server and automatically protects sensitive documents. See the [IpcDlp sample](https://Code.MSDN.Microsoft.Com/IpcDlp-Sample-Application-d30bb99d) for an example of this application type.

If your application uses the *server mode*, it should authenticate to the RMS server silently. Unlike the *client mode*, the RMS SDK 2.1 will not open a credential prompt when it fails to authenticate silently. Also, when running in *server mode*, no application manifest is needed.

For more information on setting the API security mode see, [Setting the API security mode](setting_the_api_security_mode__api_mode_.md).

<span id="Rich_client_applications"></span><span id="rich_client_applications"></span><span id="RICH_CLIENT_APPLICATIONS"></span>Rich client applications
---------------------------------------------------------------------------------------------------------------------------------------------------------

A rich client application allows users to view and manipulate data through a graphical user interface (GUI). Often, the data presented in this GUI is high-value and sensitive to theft or accidental exposure. Information protection support typically enhances existing scenarios but, is not the primary motivation for developing the application.

Using RMS SDK 2.1 with rich client applications helps you:

-   Ensure that this data is always encrypted.

-   Prevent users from extracting data to an unprotected format (for example, prevent using the clipboard to copy and paste).

Microsoft Notepad is a simple rich client application. Microsoft Office is a more complex rich client application.

For more information on protecting your application, see [Understanding usage restrictions](understanding_usage_restrictions.md).

<span id="related_topics"></span>Related topics
-----------------------------------------------

* [Developer concepts](ad_rms_concepts-nav.md)
* [IpcDlp sample](https://Code.MSDN.Microsoft.Com/IpcDlp-Sample-Application-d30bb99d)
* [IPCHelloWorld - an example application](how_to_build_your_first_application.md)
* [Setting the API security mode](setting_the_api_security_mode__api_mode_.md)
* [Understanding usage restrictions](understanding_usage_restrictions.md)
 

 


