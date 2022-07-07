# CreateImageURLforCC
This repo contains a PowerAutomate flow, that provides an URL for an uploaded image.
It was built as an extension for [Company Communicator](https://github.com/OfficeDev/microsoft-teams-apps-company-communicator) but can easily be adjusted to any use case.

You simply upload a picture in the file section of your Microsoft Teams Team.
The Flow will generate a URL for the image that you can use to view the image.
(And include it in a Company Communicator Post).

### Motivation for this solution:
In the standard App Template of the Company Communicator it is required that the image you use in a post is public.
This means, that the standard sources like e.g. Sharepoint are not the perfect fit, as they require the user to have permission to view the image.

Company Communicator authors and users are often challenged by this restriction.

That is why I built this flow, that automatically generates a public URL for an image that is uploaded to Sharepoint.


## Requirements

1. The Company Communicator App is already deployed.
	-This will create an Azure Blob Storage. So the for the flow required Blob Storage is already set up and just needs to be adjusted.
	-We already have the Authors Team set up. 
	-The **known** Sharepoint-Site can be used to upload the images.
	
2. The administrator who deployes the Flow needs access to PowerAutomate and the Premium Connectors. 
BUT ONLY HIM, The Flow will run on his behalf. So noone else needs the premium license.

## Deployement Guide
