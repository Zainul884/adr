## **ADR 2:**

**Status**

Proposed

**Context**

The app needs to have a consistent UI both online/offline, responsive and interactive push notifications, seamless transitions and animations during the checkout process, non-intrusive user behaviour tracking, seamless image display, and to be adaptive to different regions, languages, and cultures all around the world. Further details are provided below: 
Offline Capabilities:  A consistent UI is needed to ensure that the offline and online experience of the app is of the same quality. 
Push Notifications:  Responsiveness and interactivity of the UI is essential so that the push notifications can engage the user and provide accurate and well-formatted updates. 
Payment Gateway Integration: The UI must provide seamless transitions and animations to provide the user with a sense of security and confidence while purchasing products. 
User Behavior Tracking: The UI elements can play a key role in user behaviour tracking as they determine whether this process is intrusive or unintrusive and, therefore, its effectiveness.  
Optimal Image Display: The UI needs to display images and visuals seamlessly so that the overall app looks clean and sleek. 
International Expansion: A UI that can cater and adapt to different languages and cultures is essential to aid the company in achieving its international goals. 

**Decision**

We have decided to choose Flutter for the following reasons: 
Offline Capabilities: Flutter, due to its widget-based architecture and tools for local storage and caching, allows the UI to remain responsive and consistent whether it is connected to the internet or not which provides the user with the same high-quality experience. 
Push Notifications: Flutter’s custom widgets allow developers to create highly customized and tailored push notifications that can include brand colours, icons, and actions which improve the user's overall experience.
Payment Gateway Integration: Once again, Flutter’s widgets allow developers to use seamless transitions and animations when users are checking out. Some examples of widgets that can be used are ‘Card’ and ‘List View’. 
User Behavior Tracking: Flutter’s different elements such as buttons and sliders can be integrated and used to track user behavior without being intrusive.  
Optimal Image Display: Flutter uses widgets such as ‘Image. Network’ that includes caching mechanisms which ensure that images and visuals display smoothly and responsively.  
International Expansion: Flutter provides developers with an internalization package which allows them to customize various UI components and ensure that these elements (i.e. date formats, text elements) automatically adjust to cater to different cultures and languages.  

**Consequences**

Easier: Consistent UI: By using Flutter, we can ensure that the UI remains consistent across various platforms. Also, the UI can stay consistent whether or not the app has internet access which enhances and simplifies the user’s experience. Centralized Development: Flutter promotes and can provide one codebase for different platforms (i.e. iOS and Android). This can greatly reduce costs, time, and efficiency since there is no need to maintain and create different codebases.  Internationalization Expansion Pack: Flutter’s Internalization Expansion Pack makes it much easier for developers to adapt the UI to different languages and cultures.  

Difficult: Integration with Native Features: Some native features and integrations such as deep linking require additional plugins which increases the complexity of the project and can delay progress. Package Compatibility: There can be problems between different Flutter packages which can cause technical issues and slow development. It is essential to use these packages with care to ensure that they do not cause any issues further down the line and to make sure they are safe and secure to use. 
