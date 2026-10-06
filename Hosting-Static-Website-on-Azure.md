# Static Website Hosting on Azure Using Blob Storage
## Steps for hosting website
 ## Step: 1
### Create an Azure Storage Account
- Go to the Azure Portal: Log in at Azure Portal.
- Create a Storage Account:
- Click on the “Create a resource” button.

- Search for “Storage Account” and select it.
Click “Create”.


Azure Storage provides a scalable and secure way to host static websites.
<img width="1402" height="981" alt="image" src="https://github.com/user-attachments/assets/649027bb-e94b-47ed-8666-4e90eb5c3015" />

## Step: 2
###  Configure the Storage Account:
Click on create.
<img width="1431" height="1173" alt="image" src="https://github.com/user-attachments/assets/55942627-88b4-4c49-bc58-bb49a52df218" />

## Step: 3
### Create a storage account
- Subscription: Choose your subscription.
- Resource group: Select an existing group or create a new one.
- Storage account name: Enter a unique name for your storage account.
- Region: Choose a region close to your users.
- Performance: Choose Standard.
- Replication: Choose the replication option that suits your needs (e.g., LRS, GRS).
- Click “Review + Create” and then “Create” after validation.

<img width="1429" height="1515" alt="image" src="https://github.com/user-attachments/assets/4c9606f1-bd6a-43c9-885b-521cb467d883" />

## Step: 4
After clicking you will see all details you filled 
- If your details are correct click on ``` create``` otherwise change the details as per your need 


<img width="1429" height="1515" alt="image" src="https://github.com/user-attachments/assets/0b60c4c2-f101-4aa1-9173-0afa8e9ca60d" />


## Step: 5
Now Select ``Go to resouce``

<img width="1432" height="642" alt="image" src="https://github.com/user-attachments/assets/23e06e5b-3bc0-437b-b065-f1df9b21052a" />

## Step: 6
- After clicking you will landing on this page
### Navigate to Static Website

- On Data Management dropdown
- Click on Static Website
<img width="1431" height="1506" alt="image" src="https://github.com/user-attachments/assets/1f872a5e-7e23-49d8-a469-fd9888e8b556" />

## Step: 7
### Configure the Static Website

- Enable Static Website
- Enter index document name
- Enter error document path
- Then save
- you got the endpoint


<img width="1431" height="1506" alt="image" src="https://github.com/user-attachments/assets/7485b502-6158-475b-9bb1-57a9b84c6020" />


Azure will create 2 links to host the static website. The primary and secondary endpoint.
## Step: 7
### Upload Your Website Files
- Go back to the Storage Account:
- Then navigate to the “Containers” section under “Data storage”.
- You’ll see a new container called $web (created when you enabled static website hosting).
- Upload Files:
- Click on the `$web


<img width="1431" height="1506" alt="image" src="https://github.com/user-attachments/assets/81212a2b-4e3a-4150-9782-7080b5911759" />

## Step: 8
### Upload files from the PC
- click on Upload.
- Go to where the website folder is located on the computer.
- Highlight all the files in the folder.
- Drag and Drop the files from the location to the provided box.
<img width="876" height="1320" alt="Screenshot From 2026-10-06 15-40-53" src="https://github.com/user-attachments/assets/10fd0bcc-fd5d-4fd7-a7d5-0e1759540ced" />

## Step: 9
### copy the endpoint you got above in step 6
Paste on browser
<img width="1695" height="1255" alt="Screenshot From 2026-10-06 15-58-20" src="https://github.com/user-attachments/assets/1fedd741-7509-4058-95e4-7eb451ccaa86" />

