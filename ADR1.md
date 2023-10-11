## **ADR 1:**

**Status**

Proposed

**Context**

We are trying to create a retail app which can allow users to shop online/offline, receive push notifications, allow users multiple safe ways to pay, track user behaviour which can be used to enhance the app, display product images optimally to improve the speed and appearance of the app, and be capable of catering to multiple regions and languages all across the world. The three main choices are a native, web, or hybrid app type.  Please read the below details for more information: 
1. Offline Capabilities: The user must be able to browse products and view their order history even when they are not connected to the internet and the app should 
sync data when an internet connection is available.
2. Push Notifications: The retail company has to be able to send push notifications to customers to inform them about order updates, new product arrivals, and   
exclusive offers. 
3. Payment Gateway Integration: The app has to integrate with various payment gateways to ensure a secure and convenient transaction for customers.
4. User Behavior Tracking: The retail company should be able to track user behavior which includes product views, purchases, and loyalty program interactions.  
5. Optimal Image Display: The app will display product images that are different in terms of size and resolution. 
6. International Expansion: The retail company wants to expand its customer base internationally. To ensure the success of this goal, the app should support 
 multiple languages and adapt to various cultural preferences. 

**Decision**

Keeping the requirements mentioned in mind, we have decided to choose native as our app type. Our reasoning is as follows: 
Offline Capabilities: Native apps can easily integrate with the local storage of a device which ensures that customers can browse products and view order history even when they are not connected to the internet. Once there is an available internet connection, the Native App, using its inbuilt functionality, can efficiently sync data with the server. 
1. Push Notifications: Native apps allow for integration of notification services like APN for iOS and FCM for Android which ensures timely, personalized, and accurate sending and optimization of push notifications. 
2. Payment Gateway Integration: Native apps have increased and high-level security features due to the direct access they have to device features which allows them to easily integrate with different payment gateways. Also, native apps can support many different types of payment gateways which gives users and the company many ways to pay and receive money respectively.
3. User Behaviour Tracking: Native apps can closely integrate with analytics tools like Google Analytics or Flurry. Due to this close integration, native apps can collect information such as how much time a user spends on a specific screen or how they navigate throughout the app. This information allows developers to get a better understanding of user behavior which allows them to further enhance their app. 
4. Optimal Image Display: Native apps are designed to efficiently use the GPU of their respective device which allows them to render optimized images of the best quality. Key optimization techniques such as caching, lazy loading, and compression are also built within a Native app further enhancing photo quality and optimization.  
5. International Expansion: Native has “Native Development Environments” such as Xcode (iOS) and Android Studio (Android) which offer tools such as localization and internalization that allow the app to easily cater to different cultures and languages. 

**Consequences**

Easier:
1. Optimized Performance & Integration: Native apps are specifically tailored and designed for the operating system and device they will be running on. Due to this, load times and responsiveness are faster and they are much more deeply integrated with their ecosystem which includes the hardware and software of their device.
2. Advanced Offline Capabilities: Native apps have one of the best offline capabilities compared to other app types such as Hybrid due to the direct access they have to their devices' resources.
3. Access To Latest Features: Native apps are easily able to access the newest features of their respective OS which allows for faster updates and optimization to developing technologies. 

Difficult:
1. Dedicated Development For Platform: Native apps are specifically designed for the OS they will be operating on. Due to this, it is necessary that developers know all the OS’ that their app will be functioning on (which requires extra training), or that there will be different developers for each OS to ensure the highest quality (which requires extra staff and increases staff costs).
2. Maintenance: Managing different codebases for each OS that the app will be operating on, can increase overall costs and possibly slow down future updates and development as each operating system’s app will need to be updated before anything is rolled out to the public.
3. Reduced Opportunity for Scalability: Due to the different codebase for each operating system a native app functions on, it may become difficult to scale and expand the app. The reasoning for this is that each codebase needs to be separately planned, designed, and developed before any big changes are made. 
