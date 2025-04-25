<h3>Knockk : Project Portfolio</h3>

*A social networking application*

![gif](https://github.com/user-attachments/assets/0cda61b5-61ee-443a-a431-bcfbbda627c0)

### What is Knockk?
Knockk is a project aimed to create a network for residents of a building complext... **but why**?

At present, *no* social network exists for apartment building residents, leaving neighbors strangers to one another.  Knockk is here to solve that. 
> Mark 12:30-31 says, “Love the Lord your God with all your heart and with all your soul and with all your mind and with all your strength.’31 The second is this: ‘Love your neighbor as yourself.’ There is no commandment greater than these” (New International Version, 1973/2011, Mark 12:30-31). [^1]
[^1]: New International Version. (20011). Bible Gateway. https://www.biblegateway.com/versions/New-International-Version-NIV-Bible (Original work published 1973)

The bible commands us to love your neighbor as yourself, but most people do not know their neighbors. With Knockk, residents can get to know who lives around them and connect to form Godly relationships that will benefit God’s kingdom.

### To solve this...
Two user facing applications, and one API, were developed. Phase 1 of creating this network invloved implementing the following features:

| Resident     | Admin |
| ----------- | ----------- |
| Account creation | Verify residents |
View units (above, below, and to the sides) | Manage residents |
View residents of a unit | |
View a resident | |
Connect with a resident | |
Edit profile  |  |

A non-functional requirement of `not storing passwords [in the database] as clear text` by implementing the BCryptPasswordEncoder in the Spring Boot Application. 

> [!TIP]
> Please visit [demos](https://github.com/gradlund/knockk-knockk/tree/main/demo) for demonstrations of the applications.


### Technologies Chosen

| **Technology** | **Version** | **Purpose** | **Chosen** |
| -------------- | ----------- | ----------- | ---------- |
| Draw.io | v27.7.17 | Tool for technical diagramming. | Lots of shapes for different diagramming uses. |
| Expo | v51.0.0 | Accelerates development. | Recommended framework in the React Native documentation. Companies like Pizza Hut, codeacademy, and Insider all chose to integrate Expo within their apps. |
| Figma | v16.13.3 | Tool for wireframing. | Commonly used in the industry. Sleek user interface that makes wireframing enjoyable and easy. |
| GitHub | v3.4.6 | Version control in the cloud. | Commonly used in the industry. Allows developers to store code in repositories and track changes in the cloud. |
| Jira | v9.17.0 | Tool for project management. | Commonly used in the industry. Will help the team deliver code faster by managing tasks and tracking progress. |
| MacBook Pro M1 Chip Ventura | 13.5.2 | Development environment. | Developers’ current computer. |
| Node.js | v20.18.0 | Runtime environment that will execute the Expo applications. | Needed for Expo Development Builds. |
| PostgreSQL | v15.6 | Database to store data. | Database instance that Supabase provides. |
| React Native | v0.74 | Framework to build mobile and web applications. | Popular framework with large community support. Selected over Flutter because JavaScript is a popular programming compared to Dart; selected over React because React is not cross-platform. |
| Sentry | v6.1.0 | Capture reporting and performance issues for Expo. Crash reporting, performance monitoring, error tracking, gathering user feedback related to errors. | Can easily integrate into Expo project and provides great interface for reporting, monitoring, and error tracking. |
| Spring Boot | v3.1.4 | To develop the backend REST API. | Commonly used in the industry. Utilizes object-oriented principles, which is unlike other frameworks like Express (which uses a non-OOP language, JavaScript). |
| Supabase | v1.204.4 | Cloud service provider that hosts PostgreSQL databases. Alternative to Firebase. | Relational database provider in the cloud. Provides monitoring and reporting of the Postgres instance. |
| TypeScript | v5.6.3 | JavaScript superset used in React Native, strongly typed. | Offers additional safety to JavaScript which allows for more readable and maintainable code. |
| Visual Studio Code | v1.9134 | Tool for code development. | Commonly used in the industry. Lightweight IDE with a simple user interface and rich extensions. |
| Word | v16.80 | Tool for documentation. | Team is familiar with Word. Easy to create documents. |

### Best Practices
I owe a lot of thanks to my mentor, Mark Reha, for instilling best practices that will set me apart when I transition to the work place. For example, I did not utilizing the API Supabase provides because it would lock in my frontend applications, i.e., it would not be interoperable. If the database is shifted to AWS, the API would need to be rewritten.

### How I decided upon the tech stack
Upon completing the project proposal, proof of concepts were developed. <br />

Proof of concepts of React, React Native, Flutter, Expo, Express, and Supabase were all developed. From these, a tech stack was decided. Everything has pros and cons, and software is no exception - but as the saying goes, you have to pick your poison. The rational for the tech stack can be found below:

<h5>Frontend</h3>
<ul><bold>React Native</bold> was chosen for developing the cross-platform front-end applications. Initially, React was going to be used for developing the admin application, but it was decided that learning two different frameworks for two frontend applications would be a lot of work. Before React Native was decided upon, Flutter was also pursued. Flutter’s common struggle with “nesting h*ll” and the use of Dart, which is Flutter specific, ultimately led to choosing React Native. Expo is the framework of choice for building the React Native application - this framework is the recommended choice of React Native developers and speeds up the development process of React Native applications.</ul>

<h5>Backend</h5>
<ul>Spring Boot was chosen for developing the REST API. REST was chosen over GraphQL, simply because the team is more familiar with it and there are already other technologies that need to be learned. Building the API with Express was pursued as an option, but the lack of object-oriented principles because of the use of JavaScript led to Spring Boot being selected. Spring Data JDBC will be used for querying the database.</ul>

<h5>Database</h5>
<ul>Supabase was chosen as the cloud provider for the Postgres database. Not only was it chosen because it has a cool name, but because it hosts the database in the cloud, making it accessible. Postgres was decided because of the relational database advantages – creating relationships between tables.</ul>

> [!NOTE]
> I had *no* prior experience with Expo or Supbase. 
<br />

> [!WARNING]
> And I learned a few dad jokes along the way... <br>
> <br> Knock Knock... <br>
> *Who's there?* <br>
> Boo. <br>
> *Boo who?* <br>
> Don't cry - it's just a joke! <br>


### Technical Approach

Agile and the scrum methodology where implemented in this project. It is important to remember that this project is a marathon, not a sprint – figuratively speaking - so, sprints where broken into two weeks. Jira was used to manage these tasks.
Two frontend applications, a backend, and a database where designed and development. The front-end applications  utilized Expo, a React Native framework. The frontend communicates to the REST API backend, which utilized Spring Boot. The API communicates with the Postgres database, hosted on Supabase. And of course, mentorship was key to ensure that best practices are being implemented.


**Logical:** <br /><br />
<img src="https://github.com/gradlund/knockk-knockk/blob/main/artifacts/Logical%20Solution%20Design.png" alt="logical solution design" width="50%" align="center" /> <br />
This design provides a high-level overview of the project utilizing Expo, Spring Boot, and Supabase.
The two client applications, Knockk-Admin and Knockk-Resident will be built with Expo. React has a twist to N-layer architecture and combines the presentation and business layer together. This presentation and business layer contains the app and components folders. Utilizing the expo-router library, file-based routing will be used to manage screens. Subfolders inside of the app folder will have files that define the screens of the application. To abstract components from the screens, there is a separate component folder to where these components will reside. The presentation layer will contain the assets folder which will include stylesheets (utilizing NativeWinds), fonts, images, etc. The business layer will make use of state, and util. State will utilize Zustand, which is a lightweight state management library, and will eliminate excess prop drilling. The util folder will have services that make requests to the database - axios will be used for making network calls. Securing the API is an out-of-scope feature (high on the list) which means that the connection – for now – will not be secure. BCrypt will be used to hash passwords, making it harder for a hacker to steal credentials because they aren’t in plain text. The response between the Expo application and Spring Boot API will be transmitted with JSON, using HTTP. <br />
The Server, built with Spring Boot, adheres to the standard N-layer architecture. The presentation class includes the REST controllers, which utilize business services (apart of the business layer). The business services will utilize data services, which will utilize repositories to communicate to the Postgres database. Models will be passed between controllers and business services, and entities will be passed between services and between data services and repositories. <br /><br />


**Physcial:** <br /><br />
<img src="https://github.com/gradlund/knockk-knockk/blob/main/artifacts/Physical%20Solution%20Design.png" width="50%" alt="physical solution design" /> <br />
Expo Deployment Builds will be used for building the front-end applications. The Knockk-Admin application will be opened in the web on port 8081. For development, Google Chrome will be used, however Expo also supports other browsers like Edge and Safari. The Knockk-Resident application can be run on Android or iOS using an Android Emulator (using Android Studio) or iOS Simulator (using XCode). Expo SDK 51 supports iOS 13.4+ and Android 6+, so the devices and their operating systems versions could be changed by the developer if necessary. Both the admin and resident applications will make requests to the API using HTTP, port 3000. The REST API will connect to Supabase using port 6543, with HTTPS. Port 6543 is Supabase’s session port which supports prepared statements, unlike Supabase’s transaction port. <br />


The uml is a little to big to include, but you can visit it [here](https://github.com/gradlund/knockk-knockk/blob/main/artifacts/API%20UML.pdf).

### Risks and Challenges
There were three main challenges I overcame.
1. **Time**: The first semester focused on designing and architecting, while the second semester involved coding, testing, and debugging.

2. **Team size**: Knockk was developed by a single developer, resulting in slower sprint velocity compared to what a larger team might accomplish.

3. **Techincal debt**: A lone developer learned all areas of the project and thus could not specialize. This favored MVP development over code optimization. The guiding principle was, “make it work, make it pretty, make it fast”.

> [!NOTE]
> A risk management plan was also prepared during the proposal of this project, which ensured risks wouldn't turn into *issues*. View the table below for a few examples.


#### Risks
To mitigate risks, a risk management plan was assembled. None of these risks turned into issues. A few risks included:
| **Event Risk** | **Risk Probability** | **Risk Impact** | **Risk Mitigation** | **Contingency Plan** |
| -------------- | ---- | -------------- | ------------------ | ------------------- |
| Figma starts incurring charges. | $${\color{green}Low}$$  | The team would have to pay $20 a month. | The team will keep up to date with Figma policies and charges. | Word will be used for wireframing. |
| The admin application is not fully functioning. | $${\color{green}Low}$$ | Users will not be able to use the mobile application because the admin must verify the user before their account becomes activated. | Create the admin application at the first few stages of the application. | The project would be placed in jeopardy of completion. Minimal functionality will be completed with a basic UI design. |
| The team has little experience with React Native. | $${\color{orange}Medium}$$ | The team would not be able to build the front-end applications. | Research and create a proof of concept using React Native by 10/14/2024. | If React Native is not the best choice, Flutter will be pursued. |
| The team has no experience with JWTs. | $${\color{orange}Medium}$$ | API will not be secured appropriately giving anyone access to the endpoints. | If all features in scope are completed before 5/3/2025, real-time databases will be researched, and a proof of concept will be developed. | Initially out of scope. |
| The team has no experience deploying to the App or Google Play stores. | $${\color{orange}Medium}$$ | The mobile application will not be deployed to the App or Google Play stores. | If all features in scope are completed before 5/3/2025, research will be done on how to deploy to the stores. | Initially out of scope. |

*Refer to the project proposal for more risks.*

### What outstanding issues do you have?
To develop this into a ready to use network, I would like a few more features to be implemented... but I also don't want to waste my - and potential co-founders - time(s) by planning, designing, and coding new features *if* no one will even use the application. I want to ensure sales, before further development is made. So, I plan on reworking the UI and pitching it to a few clients before continuing to phase two... more details soon!

### AI acknowledgement
While I did utilize ChatGPT 4.0 mini and Grok for creating JUnit tests, they were *not* used for code generation.

### Code Repositories
Please visit the following repositories for code as well as code drop functionality videos. <br />
> <a href="https://github.com/gradlund/knockk-admin">Admin</a> : repo for the web admin application <br />
> <a href="https://github.com/gradlund/knockk-resident">Resident</a> : repo for the mobile resident application <br />
> <a href="https://github.com/gradlund/knockk-api">API</a> : repo for the api <br />

### Special Thanks
To **Mark Reha** and **James Sparks**.
