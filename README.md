ServiceNow Project: Incident Auto-Assignment via Flow Designer
## Overview

This ServiceNow Flow Designer project automatically assigns incidents to the appropriate assignment group based on the **Category** field. The goal is to eliminate manual assignment using ServiceNow's no-code Flow Designer in the **Xandu** version.

---

##  Objective

Auto-assign incidents when created, based on selected Category values such as `Software`, `Hardware`, or `Network`.

---

##  Tools Used

-  ServiceNow Flow Designer (Xandu release)
-  Personal Developer Instance (PDI)
-  No-code conditions and update actions
-  GitHub for documentation and portfolio sharing

---

##  Steps to Implement

1. **Create a new Flow**
   - Table: `Incident [incident]`
   - Trigger: `Created`
2. **Add If Conditions** for `Category`
   - Example:
     - If Category = `Software` → Assign to Software Support group
     - If Category = `Hardware` → Assign to Hardware Support group
3. **Add Actions**
   - Use `Update Record` to set the **Assignment Group** and optionally **Assigned To**
4. **Save & Activate**
5. **Test**
   - Create new Incidents and verify auto-assignment

---


**Author**
   - **Rajlakshman T**  
-  Tokyo, Japan  
- Bilingual ITSM Technical Lead | ServiceNow Developer | Flow Designer Enthusiast 

