# CreateImageURLforCC
This repo contains a PowerAutomate flow, that provides an URL for an uploaded image.
It was built as an extension for [Company Communicator](https://github.com/OfficeDev/microsoft-teams-apps-company-communicator) but can easily be adjusted to any use case.

You simply upload a picture in the file section of your Microsoft Teams Team.
The Flow will generate a URL for the image that you can use to view the image.
(And include it in a Company Communicator Post).

This Flow was built with Power Automate.

## Requirements

1. The Company Communicator App is already deployed.
	-This will create an Azure Blob Storage, that we can use.
	-We already have the Authors Team set up. 
	-The **known** Sharepoint-Site can be used to upload the images.
	
2. The administrator who deployes the Flow needs access to PowerAutomate and the Premium Connectors. 
BUT ONLY HIM, The Flow will run on his behalf. So noone else needs the premium license.

## Deployement Guide
