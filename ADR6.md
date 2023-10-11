## **ADR 6:**

**Status**

Proposed

**Context**

To further enhance and properly deliver the app's main requirements we require additional programs and frameworks. More information regarding them is listed below:

1. Offline Capabilities: Technology that provides offline-first strategies and tools are necessary to provide a smooth offline experience for users.  
2. Push Notifications: Notification systems and technologies are necessary to provide users with accurate and timely notifications according to their preferences. 
3. Payment Gateway Integration: Different secure payment processing systems are needed to allow users multiple ways to checkout safely. 
4. User Behavior Tracking: Analytical and monitoring tools that can gather and analyze user data are necessary so that the developer can enhance their app and provide users with a better overall experience.
5. Optimal Image Display: A system that can efficiently store/cache and retrieve images, when necessary, is needed so that the app's loading speed and appearance are improved.
6. International Expansion: Localization, translation, and internalization technologies are needed to help the company achieve their goals of expanding globally.  

**Decision**

We decided to use PouchDB for offline capabilities, Leverage One Signal for push notifications, Stripe SDK for payment gateway, Mixpanel for user behavior tracking, Cloudinary for image display, and i8next for international expansion. More details are found below: 

1. Offline Capabilities: PouchDB, an open-source JavaScript database can be used to store data locally and sync it with online databases once an internet connection has been established. 
2. Push Notifications: Leverage OneSignal, a high-capacity notification delivery service can be used as it can deliver a large number of personalized notifications according to user preferences.
3. Payment Gateway Integration: Stripe SDK, which is a suite of APIs, can be used to manage business transactions and various payment gateways seamlessly and securely.  
4. User Behavior Tracking: Mixpanel, an advanced analytics platform,  can provide a detailed analysis of user behavior within an app.  
5. Optimal Image Display: Integrate Cloudinary (a cloud-based service) that efficiently stores, manages, optimizes, and delivers images to provide users with a seamless app experience. 
6. International Expansion: i8next can be used which is a framework that allows for the translation of web applications, handles app localization, and ensures that an app's various components (i.e. UI) are specifically tailored for different regions, languages, and cultures. 

**Consequences**

 Easier: 
 Efficient Development: Since the app uses many different frameworks and programs, development becomes easier as specific developers can focus on improving specific parts of the app. This gives them more freedom as they are not tied to a single technology stack or language, and will also improve the app's overall performance since each part of the app is getting its due time and respect. For example, only PouchDB developers will work on all the PouchDB-related work, while Stripe SDK developers will focus only on the Stripe SDK-related work. Improved User Experience: By using tools that are specifically made to only do their tasks, the app's overall performance and, therefore, the user experience will benefit greatly as these tools will only focus on their work and not interfere with anything else. This will help to increase the app's speed and can make development and debugging much easier as mentioned before. 
 
 Difficult: 
 Increased Complexity: Using and managing multiple different tools can turn into something difficult as every tool is different from one another and it becomes essential to learn about each tool separately and keep them updated and working. The difficulty may also increase while trying to integrate all the different tools and will require advanced planning and experts. Need for More Resources: Since we are using multiple different tools, it is obvious that we will have to use multiple different resources as well. It may become difficult to efficiently manage and distribute all the available resources as failure to do so can lead to higher costs and a lower-quality final product.  
