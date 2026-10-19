# Static Website Hosting on Google Cloud Storage(GCP)
## Steps for Hosting Static Website
## Step 1: 
### Create a new Google Cloud Storage bucket
- Go to console.
- Click on the top search bar.
- Search Bucket. (Bucket is a part of cloud storage service where we can hosting our Static website)
<img width="678" height="469" alt="image" src="https://github.com/user-attachments/assets/cafdc758-48e0-494f-8728-ba9c469f90cd" />


## Step 2:
### Click on create bucket
For creating new bucket
<img width="1419" height="915" alt="image" src="https://github.com/user-attachments/assets/8ff4dce8-6dce-4931-9788-dca5dd52c551" />

### After clicking on Create bucket. you will land on this page.

<img width="1423" height="1278" alt="image" src="https://github.com/user-attachments/assets/7cc22be5-edf6-4a7c-9bd8-5af4b9fc36e6" />

## Step 3:
### Enter the name whatever u want.
- In my case i write my domain name 
- After Enter the name  click on continue.

<img width="669" height="675" alt="image" src="https://github.com/user-attachments/assets/2471f81e-9d8b-4fd9-98c5-3069cf3df7c1" />

## Step 4:
### Location type
Select the region

<img width="672" height="870" alt="image" src="https://github.com/user-attachments/assets/8e29ce9a-68aa-4466-a864-f21bb1c5c10e" />
## Step 5:Choose the Storage Class

Select Standard as the storage class for your static website.

What is a storage class?

A storage class determines how your data is stored and can affect storage costs and retrieval costs.

Standard: Suitable for frequently accessed website files.

Nearline: Designed for data accessed less frequently.

Coldline: Designed for data accessed rarely.

Archive: Designed for long-term data retention.

For this project, select Standard because website files may be accessed frequently by visitors.

<img width="697" height="952" alt="image" src="https://github.com/user-attachments/assets/f162f219-33d8-4b09-b23b-688f9a25907d" />

## Step 6:Choose How to Control Access

Select Uniform under access control.

What is Uniform access?

Uniform bucket-level access manages permissions at the bucket level using IAM (Identity and Access Management).

It simplifies permission management because access is controlled through bucket-level permissions rather than individual object ACLs.
<img width="927" height="1125" alt="image" src="https://github.com/user-attachments/assets/2fe9eb99-b330-4749-8848-d6ca5bbe9f67" />

## Step 7:Configure Public Access Prevention

Check the public access prevention setting.

If your website must be publicly accessible, public access prevention must not block the permissions required to make the website files public.

Important: Only make website files public when appropriate. Never expose private files or sensitive information.
<img width="939" height="1054" alt="image" src="https://github.com/user-attachments/assets/8f203016-3c7a-4eb6-af84-e5acbd7c3cfa" />

## Step 8:Create the Bucket

Review the bucket configuration, then click Create.

After the bucket is created, open it from the Cloud Storage bucket list.

For this project, the bucket name is:

jatinder-dev-ops-works
<img width="1437" height="1234" alt="image" src="https://github.com/user-attachments/assets/640bab16-2849-48fc-9436-8d46c15a0850" />

## Step 9:Upload Files to the Cloud Storage Bucket

After creating the bucket, open the Bucket details page for jatinder-dev-ops-works.

As shown in the screenshot, the bucket is ready to store data, but no files have been uploaded yet.

Follow these steps:

Click the Upload dropdown or the Upload files button.

Select the website files from your local computer.

Upload the required HTML, CSS, JavaScript, image, and font files.

Wait for the upload process to complete.

Verify that the uploaded files appear in the bucket's Objects list.

Why is this step required?

Uploading files stores your website content in Google Cloud Storage. The HTML files provide the page structure, CSS controls the design, JavaScript adds interactive features, and images and fonts provide visual elements.


<img width="1437" height="1234" alt="image" src="https://github.com/user-attachments/assets/6be9412c-1b00-4d2e-a819-a111ce804375" />

## Step 10: Upload Website Files to the Bucket

After creating the bucket, open the bucket named jatinder-dev-ops-works.

The bucket is currently empty, as shown in the screenshot. To upload your static website files, click the Upload Files button.

You can upload files such as:

index.html — the main webpage.

about.html and contact.html — additional webpages.

css/ — contains stylesheets for the website design.

js/ — contains JavaScript files for interactive features.

images/ — contains images used on the website.

fonts/ — contains font files.

Why is this step required?

A bucket stores the files needed for your static website. Uploading these files prepares the bucket to serve your website content through an appropriately configured access and delivery method.

Note: Upload the required website files and folders while preserving their directory structure so that the links between HTML, CSS, JavaScript, and image files continue to work.
<img width="936" height="946" alt="image" src="https://github.com/user-attachments/assets/d0cc878b-cdd0-4c5c-9324-9bf0c20ba095" />

## Step 11:Verify Uploaded Website Files in the Bucket

After uploading the website files, open the jatinder-dev-ops-works bucket in Google Cloud Storage.

As shown in the screenshot, the bucket contains the following files and folders:

about.html — About page of the website.

blog.html — Blog page of the website.

contact.html — Contact page of the website.

css/ — Contains CSS files used to style the website.

fonts/ — Contains font files used by the website.

frozenyogurtshop.psd — Photoshop design file.

index.html — Main page of the website.

js/ — Contains JavaScript files for website functionality.

product.html — Product page of the website.

singlepost.html — Individual blog post page.


<img width="1461" height="1138" alt="image" src="https://github.com/user-attachments/assets/307834df-d5d7-4b55-800d-08bccc9a57e5" />

## Step 12: Check Bucket Permissions

In this step, open the Permissions tab of your Google Cloud Storage bucket.

The screenshot shows the existing IAM principals and their assigned roles.


<img width="2412" height="891" alt="image" src="https://github.com/user-attachments/assets/7880decf-9bed-4d40-8252-148c76eb5e7f" />

## After click you see this page
<img width="1299" height="661" alt="image" src="https://github.com/user-attachments/assets/5d0fb7e3-161f-4688-94c8-ec929fe955b4" />

## Step 13:Grant Public Access to the Bucket

In this step, open the Permissions tab of the jatinder-dev-ops-works bucket and click Grant access.

Configure the Permissions

Under New principals, enter allUsers.

Under Assign roles, select Storage Object Viewer.

Review the warning that explains that adding allUsers makes the resource publicly accessible.

Click Save to apply the permission, if public access is permitted.


<img width="1306" height="1114" alt="image" src="https://github.com/user-attachments/assets/00d398b9-0da7-4e7f-84b0-302c76ecf235" />

## Step 14: click on index.html
<img width="2461" height="948" alt="image" src="https://github.com/user-attachments/assets/e4b579b0-6cd8-43ba-8c29-3ca2f1ce962c" />

## Step 15:Verify Public Access and Copy the Public URL

In this step, open the uploaded website object in the Google Cloud Storage bucket. The screenshot displays the object details, including its type, size, public URL, and access permissions.


<img width="1297" height="1002" alt="image" src="https://github.com/user-attachments/assets/86d4e793-0b47-4f8f-8536-3328bcb8b352" />

## Step 16:Access the Static Website Using the Public URL

After configuring public access, open the public URL of your website in a web browser.

As shown in the screenshot, the Freeeze website loads successfully, displaying the homepage, navigation menu, frozen yogurt images, and product section.
<img width="2877" height="1701" alt="image" src="https://github.com/user-attachments/assets/cf947c08-5096-4eea-9615-e68245ed51b2" />

## Step 17: Understand Google Cloud Storage Pricing

In this step, review the Location pricing information displayed during bucket configuration.

The screenshot shows the current configuration as Region / Standard, with the bucket located in asia-south2 (Delhi).

Current Storage Configuration

Location: asia-south2 (Delhi)

Storage class: Standard

Displayed storage rate: $0.023 per GB-month

<img width="672" height="870" alt="image" src="https://github.com/user-attachments/assets/cc74a95a-54d1-4b25-b3c5-2faea4a1743b" />
