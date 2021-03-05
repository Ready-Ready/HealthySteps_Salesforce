# HealthySteps_Salesforce

## HS User Stories for Tier design

This document contains the user stories for tier design [Healthy Steps user stories for tier design.xlsx](https://docs.google.com/spreadsheets/d/1Q1oL22wHUOB-HAUIbnVGz8z4E7R4S-XAE6wOGSvMeFs/edit?usp=sharing)

---

## Salesforce User Creation Document

- When a new user is to be added in Salesforce, new user creation request for the CHS org will be raised by Brianna White [HS Supervisor]
- Brianna will add the details of the user to the “Users 2021.02.01.xlsx” google sheet
- Once the user details are added, Coastal Cloud and Ready for School, Ready for Life teams will be notified through an email for adding new user 
- The email will be received by Renell Carpenter [System Administrator] from Coastal Cloud and Karthik Dhakshanamoorthy [System Administrator] from Ready for School, Ready for Life
- Before new user is created please make sure final approval is received from Sebrina Cooke-Davis [HS Supervisor] 
- After the approval is received Karthik Dhakshanamoorthy [System Administrator] from Ready for School, Ready for Life is responsible to create new user in salesforce
- While user is created user needs to be assiged to a **Public Group**, this information is present in **User google sheet** in **Column H**
- Later Costal team and CHS team will be notified via email for user being sucessfully added to salesforce

[Users 2021.02.01.xlsx](https://drive.google.com/file/d/1xtjNl_JpCd3_q6VKzQqQvx9oshu2eCDW/view?usp=sharing)

### Steps to add a user in Salesforce:

* From Setup, enter Users in the Quick Find box, then select Users.
* Click New User to add a single user.
* Enter the user's name, email address, mobile, Profile and Role information by referring the Google sheet.
* Enter a unique username in the form of an email address. By default, the username is the same as the email address, but you can overwrite this.
* Select Generate passwords and notify user via email to email a login name and temporary password to each new user and save the record.

After creating the user, look for **column H: Assigned Site(s)** in the user creation google sheet. The column will display the “Public Groups” information the user needs to be added to.

### Steps to add a user to the public group:

* From Setup, enter Public Groups in the Quick Find box.
* Select the appropriate Public Group from the list and click on “Edit”.
* In the search bar, enter the name of the new user you created and add the user to the “Selected Members” column and click Save.

---


## Reporting Process for CHS Org

* Reporting changes for the CHS Org will be present in the “[Healthy Steps Training Questions and Issues](https://docs.google.com/spreadsheets/d/1OAtKurnNtY1CRnZjzmncgD871txoP8UfCS30avWsr3s/edit?usp=sharing)” file under “**Report Priorities**” tab.
* The report which needs to be modified will be marked as “**1**” on the “**Priority Ranking**” column.
* The details regarding the modifications will be present in the “Notes” column.
* An issue will be created for each reporting requirement on the “**HealthySteps_Salesforce**” repository in GitHub.
* The issue will be pulled under the “In Progress” column in the “HealthySteps Salesforce” Project.
* The reports will then be created/modified in Salesforce and saved under the respective Report folders.
* Once done, the task card will be moved to the “Done” column.

---

## List of Roles, Profile and public group for active users in Salesforce org

* **Profile: Prenatal Navigation**

    - Role : Prenatal Navigation Supervisor
        - Active Users
            * Jacqueline Pippens
            * Mary Connor-Hill

* **Profile: HS Data Analyst (R/O)**

    - Role : Healthy Steps Staff
        - Active Users
            * Carli Miller

* **Profile: HS Specialist**

    - Role :
        - Active Users
            * Catherine Warner

   - Role : HSS Specialist - Bri's Team
        - Active Users
            * Rickisha Parrott [TAPM - Wendover]
            * Maggie McGaw [Wake Forest - Quaker Lane]
            * Meghann Wilkens [Wake Forest - Premier]
            * Cara Medina [Wake Forest - Greensboro]
            * Jenny Sellars [TAPM - Commerce,TAPM - Wendover]

    - Role : HSS Specialist - Lori's Team
        - Active Users 
            * Quirina Vallejos [Cone]
            * Farkhanda Hussain [Cone]
            * Robin Hartzman [GRO Peds]
            * Melissa Garrison [GRO Peds]
            * Ilene Fisher [Carolina Peds]
            * Jennifer Byrd [Pied Peds]

* **Profile: HS Supervisor**

    - Role :
        - Active Users 
            * Stella Lewallen [Wake Forest - Greensboro]
            * Sebrina Cooke-Davis [Wake Forest - Premier,Wake Forest - Quaker Lane]

    - Role : HSS Supervisor - Bri
        - Active Users
            * Brianna White [TAPM - Commerce, TAPM - Wendover,Wake Forest - Greensboro, Wake Forest - Premier,Wake Forest - Quaker Lane]

    - Role : HSS Supervisor - Lori
        - Active Users
            * Lori Pelletier [Carolina Peds, Cone, GRO Peds, Pied Peds]

* **Profile: System Administrator**
    - Role : 
        - Active Users
            * Lonnie Richardson
            * Tyler Toomes
            * Karthik Dhakshanamoorthy
            * Nicole Garcia
            * Leonard Lawson
            * Diana Peacock

    - Role : Healthy Steps Staff
        - Active Users
            * Renell Carpenter        

* **Profile: Chatter Free User**
    - Role : 
        - Active Users
            * Chatter Free User

---

## Object Permissions based on Profile


* **Profile: Prenatal Navigation**

   - Object : Consent  (Prenatal) [Read, Create, Edit]
   - Object : Navigation [Read, Create, Edit]
   - Object : Persons [Read, Create, Edit]
   - Object : Programs [Read, Create, Edit]
   - Object :Referrals (Prenatal) [Read, Create, Edit]
   - Object :Screenings (Prenatal) [Read, Create, Edit]
   - Object :Touchpoints [Read, Create, Edit]
   - Object :Needs (Navigation Person) [Read, Create, Edit]




* **Profile: HS Data Analyst (R/O)**

    - Object : Children [Read, View All]
    - Object : HS Consents [No Access]
    - Object : Needs [No Access]
    - Object : HS Referrals [Read]
    - Object : HS Screenings [No Access]
    - Object : Tier [Read]
    - Object : Topics [No Access]
    - Object : Visit [Read]
    - Object : Visit Caregivers [No Access]



* **Profile: HS Specialist**

    - Object : Children [Read, Create, Edit]
    - Object : HS Consents [Read, Edit]
    - Object : Needs [Read, Create, Edit, Delete]
    - Object : HS Referrals [Read, Create, Edit]
    - Object : HS Screenings [Read, Create, Edit, Delete]
    - Object : Tier [Read, Create, Edit]
    - Object : Topics [Read, Create, Edit, Delete]
    - Object : Visit [Read, Create, Edit]
    - Object : Visit Caregivers [Read, Create, Edit]

* **Profile: HS Supervisor**
 
    - Object : Children [Read, Create, Edit, Delete]
    - Object : HS Consents [Read, Edit]
    - Object : Needs [Read, Create, Edit, Delete]
    - Object : HS Referrals [Read, Create, Edit, Delete]
    - Object : HS Screenings [Read, Create, Edit, Delete]
    - Object : Tier [Read, Create, Edit, Delete]
    - Object : Topics [Read, Create, Edit, Delete]
    - Object : Visit [Read, Create, Edit, Delete]
    - Object : Visit Caregivers [Read, Create, Edit, Delete]




