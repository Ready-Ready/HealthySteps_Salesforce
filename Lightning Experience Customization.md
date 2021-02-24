# Lightning Experience Customization

### Set Up Your Org

#### 1. Create a custom Object

Salesforce provides standard objects and fields for common business record types, such as accounts, leads, and contacts. But every organization is unique and needs a different way to store the data. Custom objects and fields is a way to manage and store data to best fit their needs.

To create custom object follow these steps:

* From the Object Manager in Setup, click Create | Custom Object
* Enter "Example lable name" as label
* Select the box to indicate that it starts with a vowel sound
* In the Search Status section, select Allow Search
* Select Launch New Custom Tab Wizard after saving this custom object
* Leave the rest of the values as they are, and click Save

#### 2. Create a Custom Object Tab

Custom object tab, makes it easy for user to access the object. This is an important step as without custom tab user cannot add a custom object to an app. If you have selected "Launch New Custom Tab Wizard after saving this custom object", you will be directed to New custom object tab page.

* Click the Tab Style lookup icon, and select the color scheme and icon for the custom tab
* Click Next, then Next again
* Choose the custom apps that you want the new custom tab to be available in. Select to which users this tab will be visible and Deselect Include Tab, and select only which type of user this should be visible
* Click Save

#### 3. Create Custom Fields
The new object needs some custom fields added so the user can enter some information related to this object. The first thing to consider when creating a custom field is figuring out what type of field you need. Below are the steps to create a field

* Click Fields & Relationships, then click New
* Choose Picklist as the field type and click Next [there are many data types to choose from]
* Give it a label: "Example lable name"
* Select Enter values, with each value separated by a new line
* Enter the picklist values, making sure to enter each one on a new line
* Select Use first value as default value, and then click Next
* Leave the field-level security settings as they are, and click Next
* Leave default layout selected, and click Save

You can always go back and modify an existing custom field based on the needs

#### 4. Create Records

An object has  records to fill it out.The admin can enter the records into Salesforce. Inorder to create record follow these steps:

* From the App Launcher (App Launcher icon), find and select the object
* Click on New
* Add a record with the parameters listed For Example:
First Name: "Example Name"
Last Name : "Example Last Name"
Address: "Example Address"
Phone:  "Example Phone"
* After filling out these parameter, Click on save and new to add few more records

---

### Create and Customize Lightning Apps

### What Is a Lightning App?
An app is a collection of items that work together to serve a particular function. In Lightning Experience, Lightning apps gives the users access to sets of objects, tabs, and other items all in one convenient bundle in the navigation bar.Lightning apps let to brand the apps with a custom color and logo. User can even include a utility bar and Lightning page tabs in your Lightning app. Members of the org can work more efficiently by easily switching between apps. Choose the object which are used frequently  for example: Accounts, events, and organizations.Each Lightning app has a navigation bar at the top of the page, that lets the users to :

- Find what they need using item names for easy recognition
- Complete actions and access recent records and lists with a single click
- Personalize the navigation bar to suit the unique way they work

Navigation bar is basically a container for a set of items and functionality. The structure is always present just the contains or items within it keeps on changing based on the app usage. The elements are listed below:

- The app name displays on the left side of the navigation bar and custom colors and branding make each app unique and easy to identify
- Users can access other items and apps by clicking the App Launcher icon
- Users can create records and access recent records and lists directly from the navigation bar for items like Opportunities

List of things that can be addded to lightning app are:

- Most standard objects, including Home, the main Chatter feed, Groups, and People
- Org's custom objects
- Visualforce tabs
- Lightning component tabs
- Canvas apps via Visualforce tabs
- Web tabs
- Lightning page tabs
- Lightning Voice

If the org uses utility features, then utility bar can be enabled in your app that allows instant access to productivity tools, like integrated voice, in the Lightning Experience footer.You can also build your own on-demand apps by grouping items into new custom apps.

To switch between apps, users can use the App Launcher (App Launcher icon). This makes it easy for users to switch contexts and still have access to the items, objects, and pages most needed.

---

### Meet the Lightning Experience App Manager

The App Manager is your go-to place for managing the apps for Lightning Experience. It shows all your connected apps and Salesforce apps.
Use the Lightning Experience App Manager to:
- View all your Salesforce apps
- Create Lightning apps or connected apps
- See which apps are visible in Lightning Experience
- Easily manage apps 

---

### What does that “Visible in Lightning” column mean?

In the App Manager there are two types of apps: Classic and Lightning. A checkmark in the Visible in Lightning Experience column means that the app is accessible in Lightning Experience via the App Launcher and is fully functional.

Classic apps that don't have a check mark in the Visible in Lightning column are enabled only for our Salesforce Classic UI. If working in Lightning Experience, Classic-only apps cannot be found in the App Launcher. Classic apps marked as visible in Lightning Experience are fully usable in Lightning Experience, but they don't have the advantage of the app enhancements that Lightning Experience offers.

---

### Create a Lightning App

Creating and editing a Lightning app is a cinch. As a admin, an app that puts everything about customer at their fingertips. In a few simple steps, user can give an app a name, set its primary color, upload a logo, specify which items appear in the app's navigation bar, and assign the app to user profiles. For creating new app follow these steps:

- From the Home tab in Setup, enter App in the Quick Find box, then select App Manager
- Click New Lightning App
- Walk through the Lightning App Wizard, creating an app with some parameters
- Click Save and Finish to exit the wizard
- From the App Launcher (App Launcher icon), find and select new app
- The new app will have the custom branding you gave it: a custom icon in the upper left and the custom color you assigned to it. Home is first in the navigation bar, it becomes the first page your users see when they open the app.

---

### Tips for Creating Apps in Lightning Experience

Deciding how to set up Lightning apps for your users. Some of the tips for planning Lightning apps for the org :

- Talk to your users. Ask them what their priorities are. Customizing tabs in apps this gives a unique opportunity to engage with the users. Each group of users has its own priorities. Find out which objects and items represent their highest priorities
- Ask users to post feedback to a Chatter group
- Publish polls
- Schedule lunch sessions. Everyone likes a free lunch, and nearly everybody is happy to express their opinion.
- Create a master list of objects that everyone in your org wants
- Then trim down the list for each group—sales reps, sales managers, execs, and so on. 
- The menus for every user group share some common objects, like Home, Tasks, and Feed. Keep the high-priority items for each group at the top
- Put low-priority items at the bottom, or remove them altogether
- Users can always go to the App Launcher to get the items they use less often

---

### Create and Customize List Views

### Create a list view

Create list views is a easy task, For example a user wants to set up a custom list view so as to  see only certain types of accounts, follow these steps:

- From the App Launcher, find and select the app and select the Accounts tab
- From the list view controls (List View Controls), select New
- Name the list view
- Select All users can see this list view
- Click Save
- The list view will show all the accounts, regardless of their type or location, to filter based on type and location
- Click Add Filter 
- From the Field dropdown menu, select Type (Here Type filter is added as example)
- Select the equals operator
- For Value, select "some value", then click Done and Save

This will result in list view with selected type of accounts

---

### Customize a List View

After adding a custom list view, if user doesn't want to see certain columns and add missing column. Follow following steps to add and drop columns from the list view

- From the list view controls (List View Controls), select "Select Fields to Display"
- To drop columns(fields) from the list view, select and move them out of visible column
- To add columns(fields) to the list view, select and move them in the visible section 
- Click save

Records can be sorted by clicking on the arrow header to sort that column.The arrow indicates how the list is sorted: from the column’s first record (Up Sort) (alphanumerically) or its last (Down Sort).

---

### Create a List View Chart

List view charts helps to visualize the list view data. For example if user wants to see which accounts represent the most overall pipeline value, so add a chart to the All Opportunities list view. Follow these steps to add the chart

- From the app, click the Opportunities tab, and select the All Opportunities list view
- Click list view charts icon
- In the Charts panel that appears, click list view charts gear icon and select New Chart
- Name the chart, then select chart parameters (Chart Type, Aggregate Type, Aggregate Field, Grouping Field)
    * The aggregate type specifies how the field data is calculated: by sum, count, or average
    * The aggregate field specifies the type of data to calculate
    * The grouping field labels the chart segments
- Click save

When  creating a list view chart for an object, the chart is associated with the object. The chart is available for any list view that has the permission to see object, except for the Recently Viewed list.

---
### Customize Record Highlights with Compact Layouts

### What Do Compact Layouts Do?

Compact layouts control which fields the users can see in the highlights panel at the top of a record. They also control the fields that appear in the expanded lookup card when user hover over a link in record details, and in the details section when an activity is expanded in the activity timeline.

Compact layouts help in more productive work by presenting only the key record information so that work can be easily manage. For example, on account showing phone numbers and regions. With compact layouts, user can highlight whatever they need to see at a glance when looking at a record.

With in page layouts, there are separate compact layouts for each object. Compact layouts also control how records is displayed in the Salesforce mobile app. If the company uses the Salesforce mobile app, users see what they need on mobile screens, where space is limited and quick recognition of records is important.

---

### Create a Compact Layout

After creating a custom object, it is automatically assigned to a system default compact layout, which has only one field on it: the object name. Follow these steps to create a custom compact layout for the custom object:

- First, find and open the compact layouts node in Setup for Custom Object
- From Setup, click Object Manager
- Click on custom obejct to open the object and then click Compact Layouts
- You can see that the System Default compact layout is assigned as the primary compact layout right now.This can be changed
- Click New
- Give the compact layout a label: Object Name Compact Layout
- Add the fields to the compact layout
- Click Save
- Set the compact layout that is created as the primary compact layout for the object. This step will make the compact layout the new default for the custom object.
- Click Compact Layout Assignment and then Edit Assignment
- Select custom object Compact Layout and click Save

 To see the fields that are included in the primary compact layout for the custom object. 
 
-  Create a object record type and assigns it to the profiles of the users on the team
-  Then creates a different custom compact layout for the object, which includes the fields requested by the team
-  Finally, edit the compact layout assignment for the  object to assign the new compact layout to the record type 
-  Then design team members can see the highlights that they need

---
### Customize Record Details with Page Layouts

### Page Layouts

 Page Layouts can be used customize and personalize many things on a given object record page.There are two ways to customize a page in Lightning Experience. First user can customize a page's layout, or customize its contents. These are done with separate tools.

Lightning pages are a collection of Lightning components arranged in regions on the page. User can customize the structure of the page and the position of its components with the Lightning App Builder.

User can customize a page's contents, such as the fields and buttons that appear on the page, by using a different tool called the page layout editor. The page layout editor, also known as page layouts, helps you manage the content of pages in both our Classic UI and in Lightning Experience. Salesforce lightning allows dual-UI page layout editor tool to help customize page content in Lightning Experience as Lightning App Builder can't customize buttons, actions, and fields on pages.

The page layout editor lets user to do following task:

- Control which fields, lists of related records, and custom links users see
- Customize the order that the fields appear in the page details
- Determine whether fields are visible, read only, or required
- Control which standard and custom buttons appear on records and related lists
- Control which quick actions appear on the page

Parts of a page that user can customize using page layouts, to create a personalized view for different teams and processes in your org

- The Related tab contains related lists, which are lists of other records that are associated with the record user is viewing. For example, an account can have related contacts, opportunities, and other custom records. Related lists make it easy to find and manage related information.
- Details tab shows information about a record. For example, a contact record detail page shows the name, address, owner, account, and other fields that are used to store information about the contact and other related records. 
- To change the content of the fields on a related or detail page, user can click on Edit button 

---

### Customize the Fields in Your Record Details

Customizing the fields on your record pages is easy, and usesr can do it with just a few clicks. The Enhanced Page Layout Editor is the go-to place for customizing a Lightning Experience record page's fields and related lists. It's called "enhanced" because there's an earlier version of it. 

The page layout editor contains two basic parts: a palette on the upper portion of the screen and the record's page layout on the lower portion of the screen. The palette contains the basic elements—such as fields, actions, buttons, links, and related lists that user can add and arrange on your page. You can think of the upper part as the buffet table and the lower part as the plate of food being assembled.

Follow these step to add or change the page layout editor for a object:

- First, we need to find and open the object page layout
- From Setup, click Object Manager
- Click on the object to open the object and then click Page Layouts
- Click object Layout
- Now that object page layout is opened, make an update by adding or removing fields or changing the position of some of the fields
- Drag the field off the page layout to remove it and back onto the palette
- To mark a field as required, hover over the Mobile field, then click the wrench icon
- Click Required and then click OK
- Click Quick Save to save your changes without closing the page layout editor

Meaning of some of the icon which can be marked for a field

- Missing Value in Field icon―The field must have a value to save the record, but isn’t required on the page layout itself
- Field Must be Included icon―The field must be included on the page layout because an admin configured the field as universally required or Salesforce automatically requires the field
- Controlling Field icon―The field is a controlling field
- Dependent Field icon―The field is a dependent field
- Read-only icon―The field is read-only

User can assign page layouts to different user profiles. For example, user can create a customized page layout for managers and another page layout for standard users. To change page layout assignments, click Page Layout Assignment and then click Edit Assignment.

---

### Create a Page Layout

 To create an new page layout for some of the team member to the necessary field and related list information at their fingertips when they view the object records.Follow these steps

- From Setup, click Object Manager
- Click on the object, then Page Layouts
- User will be able to see the system default object layout
- Click New
- User will have two options at this point. To create a page layout from scratch, or user can choose an existing page layout to clone
- If user chooses to clone then, Select object Layout, Name the new layout 
- Click Save
- Scroll down to the Detail section, compare the two layouts fix the field order based on needs of the team
- User can move the field to change its position and also remove some of the fields which are not required to them
- Click Quick Save
- To add related list, scroll down to the Related Lists section
- In the palette, click Related Lists, and drag the object team needs in related list down to the Related Lists section. With the related list, team members can add the record and see a list of related object details associated with the record
- Click Quick Save again, then click Yes.

---

### Assign a Page Layout to Profiles

User wants it's team members  to see this new page layout. To do so user needs assign page layout to team's user profile so when they view Object  records, they will be able to see the revised view of the fields and the new related list. Follow these steps to assign the page layouts to a profile:

- Click on Setup, click Object Manager | Object
- Click Page Layouts, then Page Layout Assignment. User can see the list of profiles and the page layout assigned to each one
- Click Edit Assignment
- Select the Custom: selct the profile user wants to assign in Profile row
- From the Page Layout To Use field, select new page Layout
- Select the System Administrator row. Normally, user would select only the Custom: profile row, If the user is admin then select new profile too so that you can check out how the new page layout looks
- From the Page Layout To Use field, select new Layout, then click Save
- From the App Launcher, find and select object, then open an the record. Look at the Details tab. The new changes will be reflected there

Using the page layout and page layout editor it make it easy for user to store and manage the important data by arranging fields in logical section.
