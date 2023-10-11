## ADR 3:

Backend Language Selection

What is the status, such as proposed, accepted, rejected, deprecated, superseded, etc.?

Proposed

What is the issue that we're seeing that is motivating this decision or change?

The backend language of this app must be able to sync and update any changes from offline to online (and vice versa), manage and deliver proper push notifications, integrate with different payment gateways, process large amounts of user data, optimize and display images, and be able to manage information in different languages and adapt to a variety of cultures/regions around the world. More details are given below:

Offline Capabilities: The backend language must be able to synchronize and update any data changes once the device goes online (server data) from offline (local data) efficiently. 

Push Notifications: The backend language has to manage and deliver timely push notifications fast and accurately

Payment Gateway Integration: The app requires a backend language that can integrate with various payment gateways and ensure encrypted and secure transactions.

User Behavior Tracking:  The backend language should be able to process, store, and analyze large amounts of user behaviour data in an efficient and optimized manner.

Optimal Image Display: The backend language should be able to optimize images (i.e. choose the best resolution) depending on the user’s internet connection and device to improve the app's speed and appearance. 

International Expansion: The backend language should be able to manage information in different languages and adapt to a variety of cultural regions across the world.

What is the change that we're proposing and/or doing?

Use Node.js for the backend language

Offline Capabilities: Node.js, when connected with databases such as MongoDB, provides functionality like change streams which ensure that data syncs efficiently when devices go from offline to online, enhancing the user's experience. 

Push Notifications: Libraries such as “node-push” provided by Node.js allow developers to create customized push notifications, schedule them, and deliver them quickly and accurately. 

Payment Gateway Integration: Node.js allows developers to use a variety of payment gateway SDK (Software Development Kits) and APIs (Application Programming Interfaces) to add different payment options. These tools have inbuilt encryption which ensures a secure checkout process.

User Behavior Tracking: Node.js can manage a large amount of user data efficiently. Node.js can also work with different analytical tools to provide developers with user behaviour (i.e. how users navigate throughout the app) to further better the app's overall performance and ease of use.

Optimal Image Display: A Node.js framework, “Express.js”, can use middleware to process images which allows for quick adjustments such as resizing and compression depending on the user's device, connection, and browser. This framework also has functionality such as caching mechanisms which can store processed images, speed up subsequent requests and ensure that the user sees high-quality images and visuals.  

International Expansion: Node.js provides localization libraries and content delivery networks which make sure that content is optimized based on region, language, and culture. 

What becomes easier or more difficult to do because of this change?

Easier:

Scalability: Due to its non-blocking and event-driven architecture, Node.js can manage many tasks at the same time making it very scalable and capable of handling high volumes of traffic. Apart from this, Node.js’ scalability also makes it an ideal choice for international expansion (one of the company’s future goals) and can support integration with localization libraries due to its modular structure. 

Rapid Prototyping and Development: Node.js can provide developers with a large library ecosystem through npm (Node Package Manager), which allows them to incorporate pre-built solutions. Combining this with Node.js’ non-blocking architecture and server-side JavaScript environment improves overall integration and accelerates the development process by enabling swift iterations and changes. 

Difficult:

Lack of Conventions: Node.js does not have a standardized structure to organize code which can cause inconsistencies in projects and make overall maintenance and collaboration difficult for developers, as different developers may approach and understand code differently. 

Inconsistent Library Quality: While Node.js’ npm ecosystem contains many useful libraries and modules, their quality and stability can vary greatly. A key reason for this is that some libraries/modules may be in the early stages of development, leading to instability and possibly security concerns if developers are not careful.

