## **ADR 4:**

**Status**

Proposed

**Context**

For optimal performance, the app will request certain permissions from the user. These permissions include accessing device networks, sending notifications, utilizing biometrics, using the camera, accessing location information, managing storage, and accessing language preferences. More information is given below:

1. Offline Capabilities: Permissions to access the device's network status and background synchronization are necessary to transfer smoothly between online and offline modes.
2. Push Notifications: Requiring permission to send notifications is essential so that the app can send notifications to users about product updates, orders, and offers. Apart from this, the user would also decide the types of notifications they want to receive and when they want to receive them, which would alter the functionality of this feature.  
3. Payment Gateway Integration: Permissions such as internet access (to communicate with servers), biometrics for authentication, and camera access for facial recognition and QR payment methods are required to ensure a secure and versatile checkout process. 
4. User Behavior Tracking: Permission to track and gather user behaviour information (i.e. device usage stats) will be required to legally collect this information and use it to enhance the app. Location services may also be required to collect user information further.  
5. Optimal Image Display: Permissions to cache high-resolution product images, which are stored on the storage of the device, are required. Caching high-resolution product images increases loading speeds and ensures that clear visuals are shown quickly without the need to download them constantly.  
6. International Expansion: Access to location services and language preferences are required to cater the app to the users' specific region, culture, and language. 

**Decision**

1. Offline Capabilities: Request network status and background synchronization permissions during the setup of the app and inform the user how allowing these permissions will ensure smooth transfers between online and offline modes. 
2. Push Notifications: Either during the initial setup process or when the user completes an order or views a product, request notification permissions and inform the user how it will help them stay updated with products and view orders/offers.
3. Payment Gateway Integration: Prompt the user with biometric and camera access when they are checking out. Inform them how allowing this permission will ensure a secure checkout process. 
4. User Behavior Tracking: In the initial setup process, explain to the user how the app will use and track user behaviour information. Inform them how, by accepting this, they will be able to enhance and personalize their experience. 
5. Optimal Image Display: Ask the user for device storage permissions so that the app can store images and inform them how it will improve the app's speed and appearance. 
6. International Expansion: During the setup process, ask the user for location and language permissions and how, by allowing these permissions, the user will be able to experience a more personalized and tailored experience.  

**Consequences**

 Easier: 
 1. Increased Trust, Respect, and Transparency: By asking for permissions contextually, users gain trust and respect for the company. The users feel that their data and preferences are valued by the company which makes it more likely for users to stay with the company in the future as well. Also, this increases transparency making the company seem more friendly which may increase user loyalty and long-term engagement as well.
 2. Enhanced and Intuitive Setup Process: By requesting permissions and tying them to the app’s features and functionality the overall setup process is made more intuitive and straightforward. This greatly reduces the chances of users leaving the app due to confusion and gives users peace of mind that their data is in their own hands and not those of any company. 
 
 Difficult:
 1. Permission Denial: There is always a chance that a user does not give the app one or many permissions. This may cause issues and it becomes essential that a strategy is developed to work around this inconvenience and/or provide the user with a FAQ page, live chat, or phone number where they can ask questions about confusion they may have regarding some permissions.
 2.  Complex Testing: Due to context-based permission prompts within the app, Quality Assurance testing is made more complex as testers must test multiple scenarios for each feature that depend on whether the permission is allowed, denied, or ignored. This increases the overall test cases and workload for the developers. 
