<p align="center">
<img src="https://i.imgur.com/BZQuTqx.png" alt="osTicket logo"/>
</p>

## 🍽️ FreshTable Eats – 📱iOS MDM Lab (Jamf Now)

In this theoretical lab, I attempted to configure an old iPad, due to not being able to retrive passcodes, using Jamf Now. While I couldn't enroll my personal iPhone XR due to Apple’s MDM restrictions, I successfully set up APNs, enabled Open Enrollment, and created a Blueprint with app and policy configurations. Even though full enrollment wasn’t possible, I gained a solid understanding of Jamf Now’s features and how it supports mobile device management. I plan to retry this lab with the iPad and build on what I’ve learned.

### 🧪 Lab Tasks
#### STEP 1: Create a Jamf Now Account
I went to jamf.com and signed up for the free plan, which supports up to 3 devices.

#### STEP 2: Set Up the Apple Push Notification Service (APNs)
In Jamf Now, I navigated to Settings → Apple MDM Push Certificate, clicked on "Connect to APNs," and downloaded the CSR file. I signed in with my Apple ID, created a certificate, uploaded the CSR file, downloaded the .pem certificate, and uploaded it back to Jamf Now. Now, APNs is connected, and I can manage iPhones remotely!

<p align="center">
<img src="https://i.imgur.com/U96TSh1.png" alt="osTicket logo"/>
</p>

***

<p align="center">
<img src="https://i.imgur.com/s1uPgnc.png" alt="osTicket logo"/>
</p>

***

<p align="center">
<img src="https://i.imgur.com/mVtsXzh.png" alt="osTicket logo"/>
</p>

***

<p align="center">
<img src="https://i.imgur.com/knwmbsd.png" alt="osTicket logo"/>
</p>

***

#### STEP 3: Enable Open Enrollment
I went to Open Enrollment Settings and clicked "Enable Open Enrollment." Jamf Now provided a QR code, ready for device enrollment.

***

#### STEP 4: Enroll the iPhone XR
On the iPhone XR, I opened Safari, went to the Jamf enrollment URL, tapped "Allow" to download the configuration profile, then went to Settings > Profile Downloaded, tapped Install, and confirmed. The iPhone is now enrolled in MDM!

#### STEP 5: Create Your MDM Blueprint (Policy)
In the Jamf Now dashboard, I created a new blueprint called "FreshTable Manager iPhone" under Blueprints. I added apps like Microsoft Outlook, Square POS, Zoom, and Calendar, removed or hid the App Store, disabled Safari and the camera, and enforced a passcode policy. I also configured Wi-Fi with the store’s SSID and password.

<p align="center">
<img src="https://i.imgur.com/7ay7obN.png" alt="osTicket logo"/>
</p>

***

<p align="center">
<img src="https://i.imgur.com/KJzycDI.png" alt="osTicket logo"/>
</p>

*** 


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

