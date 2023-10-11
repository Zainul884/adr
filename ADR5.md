## **ADR 5:**

**Status**

Proposed

**Context**

Regarding data storage, the app must be able to efficiently store and synchronize data locally, user preferences, order and payment information, user data, images, as well as regional and language-related data for a seamless user experience. More information is given below: 

1. Offline Capabilities: The app should be able to locally store data and synchronize data as users will need to have access to their accounts and orders whether or not there is an internet connection. 
2. Push Notifications: The app must be able to store the users' preferences concerning push notifications so that they only receive the type of notifications they want to receive during the schedule they have selected. 
3. Payment Gateway Integration: Order details, transaction histories, and payment information (i.e. credit card number) need to be saved to make the checkout process convenient and for future reference of both the user and company. 
4. User Behavior Tracking: Data relating to user behaviour tracking must be stored and be able to be retrieved for analysis and further enhancement of the app. 
5. Optimal Image Display: Storing/caching high-resolution images on the device’s local storage is essential to improve the loading speed and appearance of the app. 
6. International Expansion: Storing data based on region, language, and cultural preferences is necessary so that the app can cater to different people all around the world. Every region or country will store different data (i.e. deals, prices, etc..). 

**Decision**

Use a combination of SQLite for local data storage and Firebase’s Cloud Firestore for cloud-based online data storage 

1. Offline Capabilities: SQLite provides developers with local storage tools and functionality which ensures that users can access their account data offline as well. Also, SQLite supports transactional SQL database operations which can synchronize data smoothly with online databases once an internet connection has been established.
2. Push Notifications: User preferences, with push notifications, can be stored locally in SQLite and then synced to the cloud using Firestone to ensure that user preferences remain consistent across any devices they use.
3. Payment Gateway Integration: Order details, transaction histories, and payment information can be stored locally using SQLite but can also be synced with Firestore to ensure the durability, availability, and security of the data. 
4. User Behavior Tracking: User Behavior Tracking data can be stored locally in SQLite and synced to the cloud using Firestore for analysis and future reference/retrieval.
5. Optimal Image Display: High-resolution and optimized images can be stored/cached locally using SQLite and they can also be stored in Firestore which will ensure improved app loading speeds and overall experience. 
6. International Expansion: Region-based, language-based, and cultural data can be stored locally using SQLite and can be synced to the cloud using Firestone which will allow for efficient content updates and quick data access for users around the world.  

**Consequences**

 Easier: Improved Scalability: Due to the use of a hybrid data storage method, the app can efficiently manage an increased amount of traffic and can be scaled internationally without any issues with quality. This can happen because of the app's ability to allocate region-specific databases and storage solutions, and its ability to handle different data types.  Better Performance: By using CDNs and utilizing distributed databases, the app’s content delivery and overall loading speeds are greatly increased. Apart from this, international expansion is also made easier as the CDN and distributed databases can deliver tailored content to the user depending on their language, region, and culture.  
 
 Difficulties: Increased Complexity: Using a hybrid data storage system increases complexity as the company and developers will have to combine multiple data storage systems and ensure that they work with each other efficiently.  Increased Cost: The hybrid approach can increase costs as the company will have to maintain and manage multiple different storage systems to ensure that their app works efficiently. Apart from this, the company must hire expert developers (which leads to extra hiring and staff costs) for each type of system they are using to maintain high-quality standards and ensure that all the different storage systems work together well. 
