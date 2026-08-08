# blogsphere-application
Android Application, using Android Studio in Java, which functions as an offline blogging and social media client.

# 1. Introduction 

This “Blogsphere” app is created to be used as a social media and blogging site offline that enables clients to make, share and manage text-based posts attached with media. The app developed using Android Studio and Java that facilitate important technologies like SQLite for local storage, Android Intents for sharing post and Camera API for capturing photos. Clients be able to attach images from the gallery or camera, delete, write & edit posts offline and upload the post to public online platforms such as Instagram, Facebook or Twitter. This application assures performances without network, making it strong and media-friendly. 

# 2. Software Design Plan 

<img width="558" height="436" alt="Screenshot 2026-08-08 at 11 37 55" src="https://github.com/user-attachments/assets/bd08563f-a794-4de7-b9a9-fdf76ee06285" />

Figure 01: Flow Chart 


<img width="658" height="698" alt="Screenshot 2026-08-08 at 11 42 15" src="https://github.com/user-attachments/assets/8d525c22-3484-4839-a796-b711f5106212" />

Figure 02: Figma UI Design


# 3. Implementation Summary

The app was created utilizing Android Studio and integrated with SQLite local database that allows offline Create, Read, Update and Delete functionalities. Clients be able to make posts by adding a tittle and post content, then a custom “DBHelper” class saved it locally. Contextual action modes and list item selection are assisted to edit and delete multiple or individual posts.

Android Camera and Gallery APIs are supported to carry out photo attachments. Clients be able to capture images directly or select existing photos from the device, and those data also  saved in SQLite with their file paths. Attached photos are showed in post previews and entire views utilizing “ImageView”.

SQL “search” queries are used to implement search feature that facilities clients to search posts by keywords. Those search outputs are dynamically showed in a “RecyclerView”.

The Blogosphere app has ability to group deletion, which means the clients can choose many messages from the post list and delete selected items in single action. Additionally, clients can see full view of post details with attached photo through tapping on a post.

The app utilized Android Intents to share posts including text and photo via email, messaging or social media applications. Public API is used to online publishing which enables uploading post to a linked account. 

Input confirmation to avoid blank posts, relevant authorization handling for camera access and secure database activities to prevent SQL injection are considered as security considerations.

# 4. Testing Summary

The app tested through emulator to assure stable performance around implementations. The main functionality of the application including create, read, update and delete are well proven by using the SQLite database. Those functionalities are effectively perform in offline. Search function also tested with several keywords to validate its searching accuracy. 

Camera and gallery both are well performed during the image attachment with runtime permission. Posts successfully shared through WhatsApp, Messenger and Emails verifying Android Intents sharing function. Uploading feature tested by using Facebook and it validated  the performance of post uploading to the social media platform. 

Camera permission and image file storage handling are some of challenges that faced during the app implementation. Those challenges are solved by using permission checks and “FileProvider”. Finally,  some database problems are solved by modifying SQL queries and assuring primary key constancy.

# 5. Reflection

The main challenges that faced during the app developing is image attachments. It’s little bit difficult to handle storage and camera permissions around various Android versions. Incorporating SQLite for offline data storage needed delicate preparation of database schema and query managing. As well as got full knowledge about Android Intents usage. 

# 7. Screenshots

<img width="398" height="631" alt="Screenshot 2026-08-08 at 11 45 22" src="https://github.com/user-attachments/assets/09866cd8-d8a1-41af-8203-53164a56c5e5" />

Figure03: Main UI

<img width="386" height="671" alt="Screenshot 2026-08-08 at 11 46 58" src="https://github.com/user-attachments/assets/f04f7af4-6e37-48cb-b644-b869dbb230bb" />

Figure04: Post creation

<img width="778" height="673" alt="Screenshot 2026-08-08 at 11 47 51" src="https://github.com/user-attachments/assets/24e50001-e6c9-4545-b5d3-e1486924b6d5" />

Figure05: Image attachment 

<img width="383" height="676" alt="Screenshot 2026-08-08 at 11 48 43" src="https://github.com/user-attachments/assets/a9b8b569-e1b3-4d03-bab5-37f46be833b4" />

Figure06: Search Function 

<img width="384" height="687" alt="Screenshot 2026-08-08 at 11 49 18" src="https://github.com/user-attachments/assets/cd0741eb-0077-4ad0-b7fd-9fbeaeb01a7d" />

Figure07: Delete function 

<img width="634" height="576" alt="Screenshot 2026-08-08 at 11 49 50" src="https://github.com/user-attachments/assets/e6a703b2-1d62-4154-ace3-800c6c747ac6" />

Figure08: Upload Post 

<img width="637" height="601" alt="Screenshot 2026-08-08 at 11 52 27" src="https://github.com/user-attachments/assets/02a7c76f-b1c7-41f4-b49d-e5382a2d0603" />

Figure09: Share Post 

# Video Demonstration 

Please note that a 4-5 minutes video is included to the zip file for your reference and prove the application implementation.
