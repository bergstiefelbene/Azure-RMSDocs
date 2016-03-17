Deploying your application
=============================================================================

This topic outlines and guides you through deployment options for your rights-enabled application.

**Important**  It is a recommended best practice to test your Rights Management Services SDK 2.1 application first with the RMS pre-production environment against an RMS Server. Then, should you want your customer to have the ability to use your application with the Azure RMS Service, move to testing with that environment. For more information see, [Enable your service application to work with cloud based RMS](how_to_use_file_api_with_aadrm__cloud_.md).

 

<span id="Installation_options_for_Active_Directory_Rights_Management_Services_Client_2.1"></span><span id="installation_options_for_active_directory_rights_management_services_client_2.1"></span><span id="INSTALLATION_OPTIONS_FOR_ACTIVE_DIRECTORY_RIGHTS_MANAGEMENT_SERVICES_CLIENT_2.1"></span>Installation options for Active Directory Rights Management Services Client 2.1
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Once you create your manifest file using a production certificate, your application is ready to be deployed. Given that you utilized RMS SDK 2.1, you will need Active Directory Rights Management Services Client 2.1 to be deployed on the end-user machine.

**AD RMS Client 2.1**

The AD RMS Client 2.1 is software designed for your client computers to help protect access to and usage of information flowing through applications that use RMS whether installed on your premises or in a Microsoft datacenter.

The AD RMS Client 2.1 is not a Windows operating system component. The AD RMS Client 2.1 ships as an optional download which can be, with acknowledgment and acceptance of its license agreement, freely distributed with your third-party software to enable client access content that has been rights protected by use and deployment of RMS servers in your environment.

**Important**  The AD RMS Client 2.1 is architecture specific and must match the architecture of your target operating system.

 

**AD RMS Client 2.1 installation choices**

-   **Redistributing the AD RMS Client 2.1**

    The recommended approach is to bundle RMS Client installer package with your application or solution using your preferred installation technology. The RMS Client can be freely redistributed and bundled with other applications and IT solutions.

    You can choose to install the AD RMS Client 2.1 interactively by starting the AD RMS Client 2.1 installer or silently install it. The integration steps will be:

    -   Download RMS Client 2.1 installer
    -   Integrate the AD RMS Client 2.1 installer run with your application installer

    Two good examples of integrating the AD RMS Client 2.1 with your application are the RMS SDK 2.1 installer package and the Right Protected Folder Explorer package. Try installing them yourself to understand the approach.

-   **Make AD RMS Client 2.1 a pre-requisite for your application install**

    In this case, you will create a pre-requisite such that your application install will fail if AD RMS Client 2.1 is not present on the end-user machine.

    If the client is not present, provide an error message informing the user where they can download a copy of the AD RMS Client 2.1

    If the client is present, proceed with your application installation.

**Enabling Azure Rights Management Services with your application**

In order for your end-user to take advantage of Azure Rights Management services, you must deploy the *Online Services Sign-in Assistant*. As the application developer, you do not know whether the end-user will use RMS (on premises) or Azure Rights Management services (cloud service).

**Important**  Running your RMS SDK 2.1 client application with Azure RMS, requires that you request an Azure RMS Tenant. Send mail to <rmcstbeta@microsoft.com> with your tenant request.

 

-   Download the [Microsoft Online Services Sign-In Assistant](http://www.microsoft.com/en-us/download/details.aspx?id=28177) from the Microsoft Download Center.
-   Ensure that your deployment of a rights-enabled application includes a pre-requisites check for this service selection.
-   For your own testing and for your end-users use of the on-line service see the TechNet topic, [Configuring Rights Management](https://TechNet.Microsoft.Com/en-us/library/jj585002.aspx).

For more on enabling your application to use RMS for Azure Rights Management services see, [Enable your application to work with cloud based RMS](how_to_use_file_api_with_aadrm__cloud_.md).

<span id="related_topics"></span>Related topics
-----------------------------------------------

* [How-to use](how_to_use_msipc.md)
* [Microsoft Online Services Sign-In Assistant](http://www.microsoft.com/en-us/download/details.aspx?id=28177)
* [Configuring Rights Management](https://TechNet.Microsoft.Com/en-us/library/jj585002.aspx)
* [Enable your application to work with cloud based RMS](how_to_use_file_api_with_aadrm__cloud_.md)
 

 


