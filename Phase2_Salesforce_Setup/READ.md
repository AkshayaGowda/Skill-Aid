# SkillAid – Phase 2: Salesforce Org Setup & Configuration

This phase documents the Salesforce Org setup and configuration for **SkillAid**, a Salesforce-based platform that matches volunteers’ skills with real-time disaster/emergency needs.

---

## 📌 Overview

- **Project Name:** SkillAid  
- **Description:** A Salesforce platform that enables NGOs and government agencies to post disaster/emergency requirements and quickly match them with volunteers having relevant skills.  

---

## 📝 Phase 2 Tasks

### 1. Salesforce Developer Edition Setup
- Sign up at [https://developer.salesforce.com/signup](https://developer.salesforce.com/signup) with valid details.  
- Verify your email to activate the account.  
- Log in at [https://login.salesforce.com](https://login.salesforce.com).  

### 2. Create a New Lightning App
- **Path:** Setup → App Manager → New Lightning App.  
- **App Name:** SkillAid  
- **Description:** Volunteer & Disaster Response Hub  
- **Navigation Items Added:** Home, Volunteer Profile, Disaster Event, Volunteer Assignment, Reports, Dashboards, Chatter.  
- Assigned to System Administrator profile.  

### 3. Custom Objects Created

| Object Name        | Purpose                            |
|-------------------|------------------------------------|
| Volunteer Profile | Store volunteer details and skills |
| Disaster Event    | Store disaster/emergency info      |
| Volunteer Assignment | Links volunteers to events     |

---

### 4. Fields Added

**Volunteer Profile**  
- Email (Email)  
- Phone (Phone)  
- Skills (Multi-Select Picklist: First Aid, Food Distribution, Search & Rescue, Medical, Logistics, Other)  
- Availability (Checkbox)  

**Disaster Event**  
- Event Type (Picklist: Flood, Fire, Earthquake, Cyclone, Other)  
- Location (Text)  
- Date (Date)  
- Needed Skills (Multi-Select Picklist)  

**Volunteer Assignment**  
- Volunteer (Lookup to Volunteer Profile)  
- Event (Lookup to Disaster Event)  
- Status (Picklist: Assigned, Completed, Cancelled)  

---

### 5. Tabs Created

- **Volunteer Profile** (Icon: People)  
- **Disaster Event** (Icon: Alert)  
- **Volunteer Assignment** (Icon: Checklist)  

All tabs assigned visibility to **System Administrator**.

---

### 6. Profiles & Permissions

- Verified that the System Administrator profile has Read/Create/Edit permissions.  
- Permission Sets can be created for other user types if needed.  

---

### 7. Documentation & Screenshots

- A folder named `/Phase2_Salesforce_Setup/` is added to this repo.  
- Screenshots included:  
  - Dashboard after login  
  - App creation  
  - Each custom object’s Fields & Relationships page  
  - Tabs page  
  - Any Permission Set created  

---



