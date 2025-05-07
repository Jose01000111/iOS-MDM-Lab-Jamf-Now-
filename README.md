<p align="center">
<img src="https://i.imgur.com/BZQuTqx.png" alt="osTicket logo"/>
</p>

## 🍽️ FreshTable Eats – 📱iOS MDM Lab (Jamf Now)

In this theoretical lab, I attempted to configure an old iPad, due to not being able to retrive passcodes, using Jamf Now. While I couldn't enroll my personal iPhone XR due to Apple’s MDM restrictions, I successfully set up APNs, enabled Open Enrollment, and created a Blueprint with app and policy configurations. Even though full enrollment wasn’t possible, I gained a solid understanding of Jamf Now’s features and how it supports mobile device management. I plan to retry this lab with the iPad and build on what I’ve learned.

### 🧪 Lab Tasks
#### STEP 1: Create a Jamf Now Account
Go to jamf.com

Sign up for the free plan (up to 3 devices)

#### STEP 2: Set Up the Apple Push Notification Service (APNs)
In Jamf Now, go to Settings → Apple MDM Push Certificate

<p align="center">
<img src="https://i.imgur.com/U96TSh1.png" alt="osTicket logo"/>
</p>

***

Click Connect to APNs → Download the CSR file

<p align="center">
<img src="https://i.imgur.com/s1uPgnc.png" alt="osTicket logo"/>
</p>

***

Sign in with your Apple ID

<p align="center">
<img src="https://i.imgur.com/mVtsXzh.png" alt="osTicket logo"/>
</p>

***

Click Create a Certificate

<p align="center">
<img src="https://i.imgur.com/knwmbsd.png" alt="osTicket logo"/>
</p>

***

Upload the .csr file you downloaded

Download the resulting .pem certificate

Go back to Jamf Now and upload the .pem file

✅ Now APNs is connected — you can remotely manage iPhones!

#### STEP 3: Enable Open Enrollment
Go to Open Enrollment Settings

Click Enable Open Enrollment

Jamf Now gives you:

A QR code (optional)

***

#### STEP 4: Enroll the iPhone XR
On the iPhone XR:

Open Safari

Go to your Jamf enrollment URL

Tap Allow to download the configuration profile

Go to Settings > Profile Downloaded

Tap Install and confirm

The iPhone is now enrolled in MDM!

#### STEP 5: Create Your MDM Blueprint (Policy)
In the Jamf Now dashboard:

<p align="center">
<img src="https://i.imgur.com/7ay7obN.png" alt="osTicket logo"/>
</p>

Go to Blueprints → Click + New Blueprint

Name it: FreshTable Manager iPhone

In the Blueprint settings:

Apps:

Add: Microsoft Outlook, Square POS, Zoom, Calendar

Remove or hide the App Store

Restrictions:

Disable Safari

Disable Camera

Disable Installing/Deleting Apps

Enforce passcode policy

<p align="center">
<img src="https://i.imgur.com/KJzycDI.png" alt="osTicket logo"/>
</p>

*** 

Wi-Fi Config:

Add your store’s SSID and password

### 🎯 Goals Accomplished
#### Deployed a secure MDM environment using Jamf Now for business-owned iPhones

#### Successfully connected APNs to allow remote device management

#### Used Open Enrollment for seamless, no-login device registration

#### Created a custom device policy (Blueprint) to control apps and restrictions

#### Reduced risk of data leakage and misuse through app & feature restrictions

### 💻 Technology Stack
#### ✅Jamf Now – Cloud MDM platform

#### ✅Apple Push Notification Service (APNs) – Device communication

#### ✅iPhone XR – Managed staff hardware

#### ✅Safari Browser – Enrollment using .mobileconfig profiles

#### ✅Microsoft Outlook – Company email & communications

#### ✅Square POS – Point-of-sale system

#### ✅Zoom – Meetings and communication

#### ✅Wi-Fi Auto Config – Seamless network connection

