# Project Overview

The Health and Behavioral Monitoring System (HBMS) is an intelligent healthcare solution focused on monitoring newborns in real-time.  
It combines physiological and behavioral data from sensors to provide a holistic view of the infant’s health.  
Through secure authentication, live data streaming, AI-powered alerts, and detailed analytics, HBMS ensures early detection of health issues.  
The system is designed to improve neonatal outcomes by empowering healthcare providers with accurate, live, and predictive insights.

---

## 📌 Project Description

HBMS collects key behavioural and physiological parameters such as heart rate, temperature, physical activity, and sleep duration.  
These features are processed through a trained **Random Forest algorithm**, which classifies the user's current health condition and helps detect patterns that may require attention.

The system integrates:

- **Flask backend** for API handling, model execution, and server logic  
- **HTML, CSS, JavaScript frontend** for a user-friendly interface  
- **Firebase authentication & cloud storage** for secure login and data management  
- **Google Gemini API chatbot** for interactive explanations and intelligent support  

The application delivers real-time predictions, personalized insights, a secure user experience, and consistent storage of health records.

---

## 🎯 Key Features

### **1. AI-Based Health Prediction**
Uses a Random Forest machine learning model trained on structured behavioural and physiological inputs to generate:
- Health condition classification  
- Probability and confidence factors  
- Data-driven explanations  
- Feature-based interpretations  

### **2. Flask Backend Architecture**
The backend:
- Loads and serves the ML model  
- Manages API requests and user interactions  
- Connects the frontend with Firebase and Gemini API  
- Processes prediction requests securely and efficiently  

### **3. Gemini Chatbot Integration**
Gemini AI enhances the platform by:
- Explaining model predictions in simple terms  
- Answering user queries  
- Guiding new users  
- Offering personalized health-related suggestions  
- Providing interactive Q&A support  

### **4. Firebase Authentication**
Ensures that:
- Only authorized users can access the system  
- Login and registration are securely handled  
- User identity is validated through Firebase tokens  
- Session management is safe and reliable  

### **5. Firebase Cloud Firestore & Storage**
Used to store:
- User detection history  
- Feedback  
- Health logs  
- Data snapshots  
- Application metadata  

This ensures a scalable, fast, and secure backend storage system.

### **6. Responsive Frontend**
The UI is built with:
- **HTML** for layout  
- **CSS** for styling  
- **JavaScript** for communication with the backend  

The frontend includes:
- Login/Register pages  
- Health input forms  
- Prediction results display  
- User history section  
- Chatbot interface  

---

## 🧠 Machine Learning Algorithm Overview

The HBMS prediction engine uses a **Random Forest model**, chosen because:
- It is highly reliable for tabular health data  
- Works well with nonlinear relationships  
- Handles missing/noisy values  
- Provides better generalization than single decision trees  
- Offers feature importance for interpretability  

The model is trained on a structured dataset, evaluated, saved, and deployed through the backend.

---

## 🏗 System Architecture

The system follows a modular architecture:

1. **User Interface (Frontend)**
   - Collects user inputs  
   - Displays predictions & responses  
   - Hosts chatbot UI  

2. **Flask Backend**
   - Handles all logic  
   - Loads ML model and performs inference  
   - Verifies Firebase tokens  
   - Sends/receives data from Gemini API  
   - Manages communication between all components  

3. **Firebase Services**
   - Authentication for user access  
   - Firestore for history & feedback  
   - Storage for user-related data  

4. **Gemini AI Chatbot**
   - Provides interactive assistance  
   - Explains results  
   - Supports natural language queries  

---

## 1. Sign Up Page

- Offers a secure and simple user registration process.
- Captures essential details like full name, email, mobile number, and password.
- Validates inputs in real-time to prevent errors and ensure data integrity.
- Includes secure password handling and form error messages.
- Ensures that only verified users are allowed to create an account on the platform.
- Provides feedback on successful registration and redirects to the login page.

➔ **The Sign Up page initiates user onboarding, ensuring authorized access to HBMS services.**
![image](https://github.com/user-attachments/assets/510f6b6b-263b-4e1d-8207-2980307a34d7)


---

## 2. Login Page

- Allows existing users to authenticate securely using email and password.
- Includes validation for incorrect credentials with user-friendly error messages.
- Supports session handling for secure login and logout functionality.
- Implements encryption to protect password data during authentication.
- Provides links to reset password if users forget their login credentials.

➔ **The Login page acts as a secure gateway for users to access the monitoring system.**
![image](https://github.com/user-attachments/assets/754bf329-fd51-4fa7-8af7-4d606f54c43a)



---

## 3. Change Password Page

- Allows authenticated users to change their password securely.
- Verifies the old (current) password before accepting the new password.
- Enforces strong password rules (like minimum length and complexity).
- Updates the password safely in the backend database after verification.
- Notifies users about successful password updates for transparency.

➔ **The Change Password page strengthens user account protection and encourages regular security updates.**
![image](https://github.com/user-attachments/assets/58bc5768-70e6-489b-b525-c7a102494f50)


---

## 4. Reset Password Page

- Helps users easily recover their accounts if they forget the password.
- Sends a secure reset link or code to the registered email address.
- Provides a form to create a new password after verification.
- Ensures the reset process is secure, preventing unauthorized password changes.
- Guides users step-by-step through the recovery flow for better user experience.

➔ **The Reset Password page ensures continuous user access with strong account recovery protocols.**

---

## 5. Dashboard Page

- Serves as the central hub for monitoring and management within the system.
- Displays summarized real-time statistics like active users, newborns under monitoring, and system alerts.
- Provides quick navigation links to different modules like Live Monitoring, Analytics, Notifications, and Reports.
- Shows visual insights through graphs, pie charts, and recent activities.
- Maintains a clean, user-friendly design for easy information access.

➔ **The Dashboard offers a comprehensive overview, making system management efficient and intuitive.**
![image](https://github.com/user-attachments/assets/75365b32-5903-4b20-8386-bd6aa3f9d877)


---

## 6. Live Monitoring Page

- Displays live health metrics collected from multiple sensors.
- Parameters include heart rate, oxygen saturation (SpO₂), temperature, and sound levels (crying).
- Continuously updates graphs and data points to reflect real-time changes.
- Alerts caregivers visually when any vital sign crosses critical thresholds.
- Provides options to view individual baby data or overall NICU health status.
- Enables healthcare providers to act quickly based on live health data.

➔ **The Live Monitoring page provides real-time, life-saving insights for neonatal healthcare management.**
![image](https://github.com/user-attachments/assets/e14eaf89-f9fb-45fb-b205-80040b3984a8)


---

## 7. Analytics Page

- Provides historical analysis of vital signs and behavioral patterns.
- Displays charts, graphs, and predictive trends based on sensor data.
- Highlights abnormal patterns like repeated oxygen dips or temperature spikes.
- Uses AI models to generate insights and suggest potential risks early.
- Allows healthcare staff to make data-driven decisions and plan treatments proactively.

➔ **The Analytics page transforms raw data into meaningful insights for smarter neonatal care.**
![image](https://github.com/user-attachments/assets/e1a7cb9a-3e1b-4dfb-af26-e196e529c7de)

---

## 8. Reports Page

- Generates detailed health reports at regular intervals.
- Includes vitals trend graphs, incident summaries, and alert logs.
- Allows exporting reports in formats like PDF for medical records.
- Helps in documenting patient history for analysis, handovers, or parental communication.
- Supports compliance with medical record-keeping standards.

➔ **The Reports page ensures easy documentation and sharing of vital health information.**
![image](https://github.com/user-attachments/assets/04f14203-0956-4f8a-a20d-b1d5c7aa8b00)


---

## 9. Doctor Appointment Page

- Facilitates scheduling of appointments with pediatric doctors and specialists.
- Allows selecting preferred dates, times, and available doctors.
- Stores appointment data securely for in-hospital or post-discharge checkups.
- Reduces waiting time and improves organization of patient follow-ups.
- Sends appointment confirmation and reminder notifications to users.

➔ **The Doctor Appointment page ensures timely medical reviews and organized healthcare delivery.**
![image](https://github.com/user-attachments/assets/52d81c97-3045-427d-bfaf-f2f6f0638d6a)


---

## 10. AI Chat Assistance Page

- Provides 24/7 support to users through a smart chat interface.
- Answers common questions about system usage, neonatal care, and health tips.
- Uses natural language processing (NLP) to understand and respond intelligently.
- Reduces dependency on hospital staff for basic queries.
- Helps new parents and caregivers with quick advice and system guidance.

➔ **The AI Chat Assistance page offers instant help, making the system more user-friendly and supportive.**
![image](https://github.com/user-attachments/assets/d5fd30c0-a239-4167-9f22-09a52bbc3d37)


---

## 11. Health Education Page

- Offers curated articles, videos, and tips on newborn health and care.
- Covers topics like nutrition, vaccination schedules, sleep safety, and emergency signs.
- Designed to increase awareness among parents, nurses, and caregivers.
- Promotes preventive healthcare by educating users proactively.
- Continuously updated with trusted medical information.

➔ **The Health Education page empowers users with knowledge for better infant care.**
![image](https://github.com/user-attachments/assets/15fb8a52-413b-401f-8017-7daf4dbedeb4)

---

## 12. User Management Page

- Allows administrators to manage all user accounts and roles.
- Supports role-based access control (doctor, nurse, admin, etc.).
- Enables creating, editing, activating, or deactivating users securely.
- Tracks user activities for accountability and system security.
- Ensures only authorized personnel access sensitive health data.

➔ **The User Management page strengthens system security and organized access control.**
![image](https://github.com/user-attachments/assets/25d59fa3-cae6-4c1b-b2a8-a07b7b2ba08f)

---

## 13. Sensor Management Page

- Monitors the status and performance of all connected sensors.
- Provides tools to calibrate sensors and check for faults in real-time.
- Displays sensor health status, data accuracy, and connectivity strength.
- Supports easy troubleshooting and sensor replacement if required.
- Ensures reliable and continuous data collection from newborns.

➔ **The Sensor Management page guarantees system accuracy and high-quality monitoring.**
![image](https://github.com/user-attachments/assets/6e6be050-7721-4cac-a9c3-f6029605683d)

---

## 14. Feedback Page

- Collects feedback, ratings, and suggestions from users.
- Allows reporting issues, requesting features, and sharing experiences.
- Helps developers and administrators identify improvements for future updates.
- Encourages active participation and continuous system refinement.
- Maintains a feedback log for analyzing user satisfaction trends.

➔ **The Feedback page drives system improvement through user engagement and insights.**
![image](https://github.com/user-attachments/assets/04daa409-4a38-4e71-b7b2-4f275806db91)


---

## 15. Notification Page

- Sends real-time alerts to users when critical health thresholds are crossed.
- Displays notifications for abnormal heart rate, oxygen levels, temperature, or behavior patterns.
- Categorizes notifications based on severity (e.g., Warning, Critical).
- Supports future extensions like email or SMS notifications.
- Helps healthcare providers react quickly to emergencies, minimizing risks.

➔ **The Notification page ensures timely awareness of critical health events for immediate medical action.**
![image](https://github.com/user-attachments/assets/8aecd463-93da-4a4c-a8b1-ba94d578c1e0)


---

## 16. Logout Page

- Allows users to safely end their session after use.
- Clears authentication tokens and session data to protect user privacy.
- Redirects users to the login page after successful logout.
- Prevents unauthorized access to the system from shared devices.
- Ensures overall security and maintains best practices in session management.

➔ **The Logout page protects sensitive information by ensuring secure session termination.**

---

## 👨‍💻 About Me

Hi, I’m **Rohith Boppana** — a passionate and driven **final-year B.Tech student** in **Computer Science and Engineering** with a specialization in **Artificial Intelligence & Machine Learning**.

I'm deeply interested in building real-world tech solutions that combine data, intelligence, and intuitive design. My academic journey and hands-on projects reflect a strong foundation in both theory and practical application.

### 👇 My Core Interests
- 🤖 Artificial Intelligence & Machine Learning  
- 🔍 Data Science & Analytics   
- 📊 BI Dashboards & Predictive Modeling  
- 💡 Problem-Solving with Scalable Technologies

I enjoy translating business needs and data insights into impactful software solutions that solve real problems and enhance user experiences.

---

## 🔗 Let’s Connect

📫 **LinkedIn**  
Let’s connect and grow professionally:  
[linkedin.com/in/rohith-boppana-39ab57279](https://www.linkedin.com/in/rohith-boppana-39ab57279/)

🌐 **Portfolio**  
Explore my latest work, skills, and projects here:  
[rohith-boppana.vercel.app](https://rohith-boppana.vercel.app)

---


> 💡 _“Final-year student, forever learner — building the future, one project at a time.”_

Feel free to explore my repositories and reach out for **collaborations**, **internships**, or to discuss **innovative ideas**!
