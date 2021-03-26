# Steps Involved in Release Deployment Process

## Pre-Deployment Steps

1. Identify all the changes and updates made for the release and add all the components to the Outbound Change Set created for the Release in the Sandbox environment.
2. Use the Salesforce Change Set Helper extension to identify all possible updates made for the release.
3. Note if any manual changes or data updates need to be done.
4. Test if all the changes are working as expected by creating test records in sandbox.
5. Test if all the changes made to the Form Assembly forms are working as expected in sandbox.
6. Document all the changes made in Salesforce and Form Assembly in the Release Notes.
7. Validate and push changes to production.


## Post-Deployment Steps

1. Validate and Deploy Salesforce changes into production.
2. Validate and Deploy Form Assembly changes to production.
3. Make any manual changes or data updates if applicable.
4. Activate any process builders/ workflow rules/ validation rules that were part of the deployment.
5. Check if all the changes have been successfully deployed in production by comparing the Release notes.
6. Check if the page layouts and field level security of any newly created custom fields are as expected.
7. Delete any fields or deactivate validation rules/ workflow rules if applicable.
8. Log in as users and check if they can see the expected changes.
9. Create few test records and check if everything works as expected.
10. Check if the Form Assembly changes are working as expected.
11. Delete any test records created in production.
