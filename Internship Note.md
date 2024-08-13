
#### Name: Archisman Midya
#### Roll: 23bcs10027
#### Startup: Dukaan / Bot9Ai


#### Task assigned: 
I worked on a comprehensive module designed to manage and interact with voice agents. This module, integrated into a dashboard layout, allows for the creation, management, and utilization of voice agents. The key components I developed are critical for ensuring a smooth user experience in managing various aspects of voice agents, including creating new agents, developing custom voice models, update existing voice-models and managing a library of voice recordings.

#### **Summary of Tech Stacks Used**
- **NextJS:** Primary framework used for developing the UI components, ensuring a dynamic and responsive interface.
- **Context API:** Used extensively for managing the state across different components, separating the data layer from the UI layer ensuring data consistency and ease of access and long-term support for re-designing UI in the future.
- **Tailwind CSS:** Utilised for styling components, with a focus on responsive design and smooth animations.
- **Next Router:** Implemented for navigation within the application, ensuring a seamless user experience.
- ****

#### Implementation of the Assigned Task:
1. **Dashboard Component(PRIMARY TASK 1)**
- **Task:** Develop a Dashboard for the voice platform to get various insights like `Active calls`, `Agent Performance`, `Customer Sentiments`, `Top Intents` and so on. Also provide the backend API to get insights data.
- **Implementation:**
    - Created the `VoiceDashBoard` component that displays various kinds charts for different types of insights dynamically. 
    - Handled UI components carefully to ensure that if some insights is scrapped in the future other insights fill the place dynamically.
    - Separated UI layer and Data Layer using Context API.
    - Scrapped Data from the `Call Logs` and `Phone Numbers` Table and calculated various metrics for required for the DashBoard API.
    - Implemented a Fallback Mechanism in the frontend to handle edge cases that happens when there is a backend error or data from the Backend API is Empty.
    - Also created a Global Dashboard component so that other developer can reuse the same components to show other analytics for other platforms like chat, agents.
- **Tech Stack:**
    - `React.js` for creating the UI.
    - Next Router for navigation.
    - `recharts` for charts and  `tailwind` for responsive design.
    - `Node.js` for creating a Backend Service to calculate Analytics Data.


2. **Create an ERD for all the models and their relationships that will be used to create the backend(PRIMARY TASK 2)**
- **Task:**  Design the ERD(Schema)(Entity Relationship Diagram) for the backend database
- **Implementation:**
    - Brainstormed With other Senior developers to understand different use cases and drafted a final schema diagram for the Backend Database. 

#### (Other Secondary Tasks)
1. **VoiceAgent Component**
- **Task:** Develop a page for the voice platform to list all the voice agents created by the user and get the details of a single chatbot and update the settings of a single chatbot 
- **Implementation:**
    - Created the `VoiceAgents` component that lists all the voice bots from the BackendAPI.
    - Separated UI layer and Data Layer using Context API.
    - Handled the route changes carefully while displaying a new page.
    - Took care of the UX by adding Shimmers on loading state.
    - Created the `VoiceAgentSettings` page to check and update the current state of a single bot.
- **Tech Stack:**
    - `React.js` for creating the UI.
    - Next Router for navigation.
    - `nuqs` for URL state management and  `tailwind` for responsive design.

2. **Buy Number From Twilio**
- **Task:** Develop a component to let the user buy numbers from Twilio service.
- **Implementation:**
	- Create a form that lets user put in necessary details which hits a Twilio REST API to get all the different Numbers that the user can choose from.
	- Create a Form for where the user chooses a number and hits another Twilio REST API to subscribe the user to that number.

3. **Voice Library:**
- **Task:** Develop a page to display all the Voice models that are available to the user. The user can hear the voice and accent of each agent so that he/she can choose the specific model according to use case.
- **Implementation:**
    - Created the `VoiceLibrary` component that lists all the voice bots from the BackendAPI.
