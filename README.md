# Knockk : Project Portfolio
*A social networking applcation*

## Overview
### What is Knockk?
Knockk is a project aimed to create a network for residents of a building complext... **but why**?

At present, *no* social network exists for apartment building residents, leaving neighbors strangers to one another.  Knockk is here to solve that. 
> Mark 12:30-31 says, “Love the Lord your God with all your heart and with all your soul and with all your mind and with all your strength.’31 The second is this: ‘Love your neighbor as yourself.’ There is no commandment greater than these” (New International Version, 1973/2011, Mark 12:30-31).

The bible commands us to love your neighbor as yourself, but most people do not know their neighbors. With Knockk, residents can get to know who lives around them and connect to form Godly relationships that will benefit God’s kingdom.

### To solve this...
Two user facing applications (and one API) was developed. Phase 1 of creating this network invloved implementing these features:

| Admin     | Resident |
| ----------- | ----------- |
| Account creation | Verify residents |
View units (above, below, and to the sides) | Manage residents |
View residents of a unit | |
View a resident | |
Connect with a resident | |
Edit profile  |  |

A non-functional requirement of `not storing passwords [in the database] as clear text` by implementing the BCryptPasswordEncoder in the Spring Boot Application. 


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
I did

### Deployed in the cloud? CI/CD

### What'd you learn? Why?
Proof of concepts where developed LIST PROOF OF CONCEPTS


And I learned a few dad jokes along the way... <br>
<br> Knock Knock... <br>
*Who's there?* <br>
Boo. <br>
*Boo who?* <br>
Don't cry - it's just a joke! <br>
### What technical approach did you take? Include a variety of design diagrams, class diagrams, etc. to support the technical aspects of your project.

### What risks and challenges did you have? How did you overcome these and what resources did you use?  What risk management approaches did you take?
There were three main challenges I overcame.
1. **Time**: The first semester focused on designing and architecting, while the second semester involved coding, testing, and debugging.

2. **Team size**: Knockk was developed by a single developer, resulting in slower sprint velocity compared to what a larger team might accomplish.

3. **Techincal debt**: A lone developer learned all areas of the project and thus could not specialize. This favored MVP development over code optimization. The guiding principle was, “make it work, make it pretty, make it fast”.

#### Risks
To mitigate risks, a risk management plan was assembled. None of these risks turned into issues. A few risks included:
| **Event Risk** | **Risk Probability** | **Risk Impact** | **Risk Mitigation** | **Contingency Plan** |
| -------------- | ---- | -------------- | ------------------ | ------------------- |
| Figma starts incurring charges. | <span style="color: green"> Low </span> | The team would have to pay $20 a month. | The team will keep up to date with Figma policies and charges. | Word will be used for wireframing. |
| The admin application is not fully functioning. | Low | Users will not be able to use the mobile application because the admin must verify the user before their account becomes activated. | Create the admin application at the first few stages of the application. | The project would be placed in jeopardy of completion. Minimal functionality will be completed with a basic UI design. |
| The team has little experience with React Native. | Medium | The team would not be able to build the front-end applications. | Research and create a proof of concept using React Native by 10/14/2024. | If React Native is not the best choice, Flutter will be pursued. |
| The team has no experience with JWTs. | Medium | API will not be secured appropriately giving anyone access to the endpoints. | If all features in scope are completed before 5/3/2025, real-time databases will be researched, and a proof of concept will be developed. | Initially out of scope. |
| The team has no experience deploying to the App or Google Play stores. | Medium | The mobile application will not be deployed to the App or Google Play stores. | If all features in scope are completed before 5/3/2025, research will be done on how to deploy to the stores. | Initially out of scope. |


### What outstanding issues do you have?
To develop this into a production ready network, I would like a few more features to be implemented... but I also don't want to waste my - and potential co-founders - time(s) by planning, designing, and coding new features *if* no one will even use the application. I want to ensure sales, before further development is made. So, I plan on reworking the UI and pitching it to a few clients before continuing to phase two... more details soon!

### AI awknowledgement
While I did utilize ChatGPT 4.0 mini and Grok for creating JUnit tests, they were *not* used for code generation.
