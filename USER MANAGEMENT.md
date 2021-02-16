# User Management

## What is a User?
<p> A user is anyone who logs into Salesforce. Users can be employees at your company, sales reps, managers and IT specialist, who needs access to
company's records. New user will perform user management task like: </p>

* Creating and editing users
* Resetting passwords
* Granting permissions
* Configuring data access

<p> Every user in Salesforce has user account. The user account identifies the user, and user account settings to determine what features and records the user can access. Each user account contains at least the following:</p>

- Username
- Email Address
- User's First and Last Name
- License
- Profile 
- Role (Optional)

<p> To view and manage the users in your organization, from Setup, enter Users in the Quick Find box, then select Users. The user list shows all the users in your organization. From the list, admin can:</p>

- Create one or more users
- Reset passwords for selected users
- View a user's detail page by clicking the name, alias, or username
- Edit a user's details
- Log in as any user if the system permission is enabled or if the user has granted you system administrator login access

---

## Key Terms

### Usernames

<p> Each user has both a username and an email address. The username must be formatted like an email address and must be unique across all Salesforce organizations. It can be the user's email address, as long as it is unique.

### User Licenses
<p> A user license determines which features the user can access in Salesforce. For example, you can allow users access to standard Salesforce features and Chatter with the standard Salesforce license. But, if you want to grant a user access to only some features in Salesforce, you have a host of licenses to choose from. For example, if you have to grant a user access to Chatter without allowing them to see any data in Salesforce, you can give them a Chatter Free license. </p>

### Profiles
<p> Profiles determine what users can do in Salesforce. Profile come with a set of permissions which grant access to particular objects, fields, tabs, and records. Each user can have only one profile. Select profiles based on a user’s job function (the Standard User profile is the best choice for most users). Don’t give a user a profile with more access than the user needs to do their job. You can grant access to more items the user needs with a permission set.</p>

### Roles
<p> Roles determine what users can see in Salesforce based on where they are located in the role hierarchy. Users at the top of the hierarchy can see all the data owned by users below them. Users at lower levels can't see data owned by users above them, or in other branches, unless sharing rules grant them access. Roles are optional but each user can have only one. If you have an org with many users, you may find it easier to assign roles when adding users. However, you can set up a role hierarchy and assign roles to users at any time. Roles are only available in Professional, Enterprise, Unlimited, Performance, and Developer editions of Salesforce. </p>

### Alias
<p> An alias is a short name to identify the user on list pages, reports, or other places where their entire name doesn't fit. By default, the alias is the first letter of the user's first name and the first four letters of their last name. </p>

---

### Guidlines to add new users

- Username: Each user must have a username that is unique across all Salesforce organizations
- Username Format: Users must have a username in the format of an email address (that is, example@domain.com), but don't have to use a real   email address. The email can be used as long as its unique accross all salesforce org
- Email: Users can have the same email address across organizations.
- Passwords: Users must change their password when login for the first time
- Login Link: Users can only use the login link in the sign–up email once. If a user follows the link and does not set a password, the admin have to reset the password before user can log in.

---

### Adding Users

<p> The maximum number of users you can add is determined by your Salesforce edition and the number of user licenses purchased.</p>

To add users follow these steps:

- From Setup, enter Users in the Quick Find box, then select Users
- Click New User to add a single user or click Add Multiple Users to add up to 10 users at a time
- Enter each user's name, email address, and a unique username in the form of an email address. By default, the username is the same as the email address, but this can be changed
- Select the user license you want to associate with the users you create (the license determines which profiles are available for each user)
- Select a profile
- Select Generate passwords and notify user via email to email a login name and temporary password to each new user
- Click Save

---

### Access user management

<p> Access to user management is not limited to desktop, to setup Salesforce on mobile for iOS and Android mobile devices. Download SalesforceA from the App Store™ or Google Play™. Salesforce mobile app can help to perform admin task like: </p>

- Resetting passwords
- Freezing users
- View current system status from mobile device

---

### Logging In to the Salesforce Mobile App

<p> It's easy to login to salesforce app, following elements are needed to log in sucessfull to salesforce app: </p>

- Username
- Super secret password
- Corrent Instance (Instance can vary from production or sandbox or custom domain.By default the mobile app will connect to production enviornment)

#### Steps to sign in mobile app:

- Open the Salesforce mobile app
- Tap Sign In
- To log in to sandbox or a custom domain, iOS users tap Settings Icon to select the correct environment. Android users tap Overflow Icon to elect the correct environment
- Enter the username and password
- Tap Log In

---

### Monitor the trust status

<p> After you log in to SalesforceA, the Overview page shows the recent system status and recently viewed users.The Recent System Status section shows information from trust.salesforce.com about instance's system performance over the last 24 hours. Trust.salesforce.com is Salesforce's website to provide transparency around service availability, performance, security, privacy, and compliance. Trust status gives you a quick and easy way to see if org performance has been affected so you can let your users know of any changes. </P>

### Freeze a user

<p> From SalesforceA mobile app, go to the user's profile page for the user which needs to be freezed, then tap and select Freeze. </p>

---

### Data Security

<p>Salesforce includes simple configuration security controls that make it easy to specify which users can view, create, edit, or delete any record or field in the app. Configuration can be done to access record at the level of the organization, objects, fields, or individual records. By combining security controls at different levels, right level of data access can be provided to thousands of users without having to specify permissions for each user individually.</p>

### Levels of data access

There are four main levels to configure access of data in Salesforce:

1. Organization
Organization is the highest level, where admin can secure access to your organization by maintaining a list of authorized users, setting password policies, and limiting login access to certain hours and certain locations.

2. Objects
Object level security provides the easy way to control which users have access to which data. By setting permissions on a particular type of object, admin can prevent a group of users from creating, viewing, editing, or deleting any records of that object. For example, admin can use object permissions to ensure that interviewers can view positions and job applications but not edit or delete them.

3. Fields
Using field level security to restrict access to certain fields, even for objects a user has access to. For example, you can make the salary field in a position object invisible to interviewers but visible to hiring managers and recruiters

4. Records
To control data with greater precision, particular users  can be allowed to view an object, but then restrict the individual object records they are allowed to see. For example, record–level access allows interviewers to see and edit their own reviews, without exposing the reviews of other interviewers. Record–level access can be managed in the following ways:

* Organization–wide defaults 
Organization–wide defaults specify the default level of access users have to each other's records. Using organization–wide sharing settings to lock down the data to most restrictive level, and then use the other sharing tools to selectively give access to other users. For example, you can give all employees access to an object called Candidate to allow anyone to add a candidate to the database. But you can restrict access to Positions so that anyone can see the jobs available but only the employees with the proper permissions can edit them.

* Role hierarchies 
Role hierarchies open up access to those higher in the hierarchy so as to inherit access to all records owned by users below them in the hierarchy. Role hierarchies don't have to match the organization chart exactly. Instead, each role in the hierarchy represents a level of data access that a user or group of users needs. For example, you can restrict access to Candidates by setting the organization–wide default to Private, but allow recruiters to view and edit the candidate records that they own. Recruiters can't see candidate records they don't own because recruiters are all at the same level in the role hierarchy. However, hiring managers can be given read/write access to all candidate records because they are at a higher level in the role hierarchy than recruiters.

* Sharing rules 
Sharing rules enables to make automatic exceptions to organization–wide defaults for particular groups of users, to give them access to records they don't own or can't normally see. Sharing rules, like role hierarchies, are only used to give more users access to records—they can't be stricter than your organization–wide default settings. For example, all employees are allowed to view Positions, but use sharing rules to grant full editing access to employees in a role or group called Hiring Managers.

* Manual sharing 
Manual sharing allows owners of particular records to share them with other users. Although manual sharing isn't automated like organization–wide sharing settings, role hierarchies, or sharing rules, it can be useful in some situations, for example, if a recruiter going on vacation needs to temporarily assign ownership of a job application to another employee.

---

### Set Organization-Wide Sharing Defaults

To set Organization-Wide Sharing Defaults follow these steps:

1. From Setup, enter Sharing Settings in the Quick Find box, then select Sharing Settings
2. Click Edit in the Organization-Wide Defaults area
3. For each object, select the default access you want to use
4. To allow employees at higher levels in the role hierarchy to access records automatically, select Grant Access Using Hierarchies for any custom object that does not have default access of Controlled by Parent

<p> In environments where the organization-wide sharing setting default for an object is set to Private or Public Read Only, record access can be  grant to users by setting up a role hierarchy or defining sharing rules. Just remember, you can only use sharing rules to grant more access.Record access cannot be restricted beyond what was originally specified with the organization–wide sharing defaults.

By default, Salesforce uses hierarchies, like a role hierarchy, to automatically grant record access to users above the record owner in the hierarchy. Setting an object to Private makes those records visible only to record owners and users above them in the role hierarchy. If you want to disable access to records for users above the record owner in the hierarchy for custom objects, use the Grant Access Using Hierarchies checkbox. If you deselect this checkbox for a custom object, you restrict record access to only the record owner and users granted access by the organization–wide default.

If you deselect Grant Access Using Hierarchies, users that are higher in the role hierarchy don't receive automatic access. However, some users can still access records they don't own by default—such as users with the "View All" and "Modify All" object permissions and the "View All Data" and "Modify All Data" system permissions.

When the update is made to organization-wide defaults, there will be sharing recalculation to run automatically and apply any access changes to the records. When the recalculation completes nofication email will be received and after refreshing the Sharing Settings page you can observe the changes. To view the updated status, from Setup, enter View Setup Audit Trail in the Quick Find box, then select View Setup Audit Trail.

Once the data is  secured with organization-wide defaults, the resulting settings might be too restrictive for some users. For those user you can  open up record access using remaining record-level security controls: role hierarchies, sharing rules, and manual sharing  only to those specific users who need it. </p>