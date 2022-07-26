# Generate a public URL for a Company Communicator Post
This repo contains a PowerAutomate flow, that provides an URL for an uploaded image.
It was built as an extension for [Company Communicator](https://github.com/OfficeDev/microsoft-teams-apps-company-communicator) but can easily be adjusted to any use case.

You simply upload a picture in the file section of your Microsoft Teams Team.
The PowerAutomate flow will generate an URL for the image that you can use to view the image.
(And include it in a Company Communicator Post).

### Motivation for this solution:
In the standard App Template of the Company Communicator it is required that the image you use in a post is public.
This means, that the standard sources like e.g. SharePoint are not the perfect fit, as they require the user to have permission to view the image.

Company Communicator authors and users are often challenged by this restriction.

That is why I built this flow, that automatically generates a public URL for an image that is uploaded to Sharepoint.

Here you can see the normal file upload tab in Microsoft Teams. This is where you upload the image you want to use in your post.
![File Upload in Microsoft Teams](![Flow Overview](https://github.com/MSFT-srothhaupt/CreateImageURLforCC/blob/main/Deployment_Photos/File%20Upload%20to%20Sharepoint%20in%20Teams.png)

Here you can see how the Power Automate Flow responds to your upload: It provides this public URL as a clickable hyperlink and as written text and posts it into the Teams channel.
![Flow answers in your Teams Channel](https://github.com/MSFT-srothhaupt/CreateImageURLforCC/blob/main/Deployment_Photos/Post%20with%20public%20URL%20in%20Teams%20Channel.png)

## Here is an overview of the PowerAutomate flow:

![Flow Overview](https://github.com/MSFT-srothhaupt/CreateImageURLforCC/blob/main/Deployment_Photos/FlowOverview.png)

## Requirements

1. The Company Communicator App is already deployed.
- This will create an Azure Blob Storage. So the for the flow required Blob Storage is already set up and just needs to be adjusted.
- We already have the Authors Team set up. 
- The **known** Sharepoint-Site can be used to upload the images.
	
2. The administrator who deployes the Flow needs access to PowerAutomate and the Premium Connectors. 
But ONLY the admin, the flow will run on his behalf. So no further premium licenses are required.

## Deployement Guide

1. Download the PowerAutomate flow [here](https://github.com/MSFT-srothhaupt/CreateImageURLforCC/raw/main/CreateaURLforuploadedimages._20220707142958.zip) if you have not done it so far.
2. Follow this [Video Guide](https://sway.office.com/2LuEFfKSBU9yIWiw?ref=Link)


