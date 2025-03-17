## About Me

I am a people-oriented computing student at the university of Zurich in my masters degree. I am especially interested in human-computer interaction, software development, user experience, HCI in AI, digital solutions in (women's) health and always enthusiastic to hear about other topics!

- 🔭 I’m currently working on building my own website
- 🌱 I’m currently learning more on frontend development, sustainable HCI & HCI in AI
- 💬 Ask me about React, JS, Java, HTML, CSS
- 😄 Pronouns: She/her
- ⚡ Fun fact: I like to go camping during the summer

## Projects

### Supply Manager 🧑‍⚕️
For my Master's Project, I, along with four other students, developed the prototype that I designed for my Bachelor's Thesis. This Master's Project was a part of a broader initiative dedicated to halting the spread of non-communicable diseases (NCDs) in sub-Saharan Africa, where healthcare resources are limited. In this endeavor, Chronic Care Workers (CCWs) assume a critical role, responsible for the screening, diagnosis, and treatment of NCDs such as diabetes and hypertension within local communities. However, there a supply management system is lacking, which could provide immense value to CCWs in efficiently handling their medical resources.

This master's project aimed to address this gap by implementing a Supply-Manager to support CCWs in their essential work. The Supply-Manager consists of a Worker-Frontend and an Admin-Panel, serving as interfaces for CCWs and administrators, respectively. The Worker-Frontend focuses on helping CCWs manage their supplies and facilitating their interaction with the Supply-Manager, offering an appealing user experience.The Admin-Panel retrieves essential data from an existing application, serving as a bridge between this application and the Worker-Frontend. Extensive user interviews have been conducted to evaluate the Supply-Manager, allowing participants to actively engage with the Worker-Frontend and Admin-Panel interfaces. 

The developed Supply-Manager empowers CCWs and administrators with effective tools for streamlined supply management. By integrating user-centered design and evaluation, this work contributes to the project's success in improving healthcare delivery and addressing the challenge of NCDs.

<div style="display: flex; justify-content: space-between;">
  <img src="https://github.com/StefanieKrohmann/StefanieKrohmann/assets/71380307/6617d071-b4c2-4aa1-878b-020612ab0b76" alt="MyStock" style="width: 48%;" />
  <img src="https://github.com/StefanieKrohmann/StefanieKrohmann/assets/71380307/889ab418-d5ff-4dd8-8d42-58a0f32d978f" alt="Order" style="width: 48%;" />
</div>

<div style="display: flex; justify-content: space-between;">
  <img src="https://github.com/StefanieKrohmann/StefanieKrohmann/assets/71380307/3c566548-261c-4339-b343-185b6f56e5c0" alt="Pack My Bag" style="width: 48%;" />
  <img src="https://github.com/StefanieKrohmann/StefanieKrohmann/assets/71380307/d49fba86-06f5-4e28-950c-5596746cb2bf" alt="Order" style="width: 48%;" />
</div>

#### Implementation & Architecture
The Worker-Frontend and Admin-Panel serve as the primary components of the Supply-Manager. The Worker-Fronted was build as a PWA using Typescript and React. Given the requirement for proper offline mode functionality, each CCW is equipped with its own dedicated CouchDB. In offline mode, the front end leverages PouchDB to store the current state locally, which is subsequently synchronized with the corresponding CouchDB once an online connection is established. This architecture allows direct communication between the Worker-Frontend and the multiple CouchDBs, enabling seamless data management and supporting individual CCWs with their dedicated databases. Due to the Worker-Frontend’s capability to save and synchronize its local states upon
regaining an online connection, the Admin-Panel refrains from making direct modifications to the CouchDBs. Instead, the primary role of the Admin-Panel in relation to CouchDB revolves around managing the creation and deletion of CouchDBs, specifically generating a new CouchDB for each new CCW and removing the corresponding CouchDB upon CCW deletion. Besides that, the Admin-Panel solely relies on read access to each CouchDB associated with individual CCWs. As for the Admin-Panel’s internal operations, it leverages a relational database named MySQL. This database serves as a repository for storing essential components crucial for the utilization of the Supply-Manager.

  <img src="https://github.com/StefanieKrohmann/StefanieKrohmann/assets/71380307/b1a13540-00c2-446f-b569-d35fda7e90b7" alt="Architecture MP" style="width: 48%;" />


### ICU Connect 🟢
ICU Connect serves as a social network exclusively for UZH / IFI students, enabling them to gain valuable insights into course content and quality through ratings, shared files, posts, and interactive discussions. Collaboration among students from various courses fosters knowledge sharing, ensuring the transfer of valuable information from year to year. Additionally, for those without personal connections to previous course takers, a forum with supplementary information proves highly beneficial.

- 📚 Learn more: https://github.com/The-Agile-Avengers/icu-connect-frontend/wiki

![communities](https://github.com/StefanieKrohmann/StefanieKrohmann/assets/71380307/8f50dfba-a3d8-45e3-b9b1-47305eec8cea)

#### Implementation & Architecture
Our web application consists of a Java backend, a React frontend, a MySQL database and leverages AWS services as for example the S3 service for storing and managing documents. The architecture follows a client-server model, with the backend serving as the server-side component and the frontend running in the client's browser. 

- 📚 Learn more: https://github.com/The-Agile-Avengers/icu-connect-frontend/wiki

![architecture](https://github.com/StefanieKrohmann/StefanieKrohmann/assets/71380307/09391d6f-d734-4585-a48b-de2d256709ec)


### BROLAT 📅

As part of the module "Software Computer Engineering Lab" I and four other students created an application that facilitates the organization of a student's life and collaboration among peers. 

In the life of a student it is often overwhelming to get a hold of all the deadlines from the different modules. All this energy spent on organizing and planning a semester can be simplified. Therefore, we built an interactive application, where users can communicate with each other in small groups and handle all their personal or shared tasks in a simple and intuitive way. Information about various modules, tasks you need to work on and collaborations with other students is centralized in one application. A well designed homepage delivers all the information you need to know about the current week lectures, tasks, exercises, deadlines and meetings that are coming up.

- 📚 Learn more: https://github.com/sopra-fs21-group-09/sopra-fs21-group-09-client

![Home](https://user-images.githubusercontent.com/71380307/145211269-629f98da-c2c9-4b91-a8f3-36e6ec8a424b.png)
![Home_Overlay](https://user-images.githubusercontent.com/71380307/145211791-1d02b95f-4b90-4e91-ba1d-2d5c9b010a75.png)
![Group Details](https://user-images.githubusercontent.com/71380307/145211741-5ba59a3f-efbf-4093-9771-fc7775fbd1ea.png)
![Kopie von SOPRA Component diagram](https://user-images.githubusercontent.com/71380307/112836531-06012100-909b-11eb-9229-60ce1b352361.png)



### CLOUDLOCK 🔒

During a three-month internship, I and another informatics student from UZH developed an IoT concept that enables the control of lockers via the cloud. This is done via the user's smartphone, resulting in low complexity, low cost and ease of use. A lot of emphasis was put on usability and compatibility with different apps (application agnostic). Finally, we designed and programmed a prototype (full-stack web application & REST API) that works via QR codes, that are placed on each compartment of a locker. Along the way, I was also able to gain insight into a market study that explored the various possible applications of the app.

### MY WEBSITE 👩
Currently I am building my own website, which will be available under: https://stefaniekrohmann.github.io/. Stay tuned!


