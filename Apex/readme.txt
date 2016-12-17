https://uat-api.apexclearing.com/

https://api.apexclearing.com/atlas/docs/

Important Links:
Getting started: https://github.com/apexclearing/getting-started
Legit – Authentication  https://github.com/apexclearing/api-documentation/tree/master/legit
Atlas – Account Management https://github.com/apexclearing/api-documentation/tree/master/atlas
Snap – Image Service https://github.com/apexclearing/api-documentation/tree/master/snap
Sketch -  CIP, Do not do business & critical alerts  https://github.com/apexclearing/api-documentation/tree/master/sketch
Sentinel – Cash Management  https://github.com/apexclearing/api-documentation/tree/master/sentinel
Herodotus – Trades  https://github.com/apexclearing/api-documentation/tree/master/herodotus
Pypex – Sample Code https://github.com/apexclearing/pypex
 
 
New account diagram:
https://github.com/apexclearing/api-documentation/blob/master/atlas/img/atlas_acct_req_workflow.jpg
 
 
**Release Notes:  we post all of our release notes for UAT and Production.  Please become a watcher and you will be notified by email when changes are made.
https://github.com/apexclearing/release-notes
 
Account type and forms required for opening:
Individual
direct_new_account_form
 
Joint
direct_new_account_form
Choose 1:
  joint_tenants_in_common_form
  joint_rights_of_survivorship_form
  joint_community_property_form
  joint_tenants_by_entirety_form
 
Resident Alien - Individual
direct_new_account_form
 
Resident Alien - Joint
direct_new_account_form
Choose 1:
  joint_tenants_in_common_form
  joint_rights_of_survivorship_form
  joint_community_property_form
  joint_tenants_by_entirety_form
 
 
IRA - Roth
direct_new_account_ira_form
roth_ira_adoption_agreement_form
 
retirement_account_beneficiaries_form  (optional on account creation)
 
IRA – IRA/SEP/Rollover
direct_new_account_ira_form
ira_sep_rollover_adoption_agreement_form
 
retirement_account_beneficiaries_form  (optional on account creation)
 
IRA – Simple
direct_new_account_ira_form
simple_ira_participant_adoption_agreement_form
 
retirement_account_beneficiaries_form  (optional on account creation)

---------------------------------------------------------------------------------------
From: "Christie Pittman" <cpittman@apexclearing.com>
---------------------------------------------------------------------------------------

I have attached the following items to get you started in our UAT environment.  Please let me know if we need to talk over any of the details.
 
Credentials - this included access to Atlas, Sentinel, Sketch and Snap
UAT CIP fixture data to use with your Atlas requests – this will make sure you get your desired responses.
Sample account
 
Link to our new getting started page - https://github.com/apexclearing/getting-started
 
 
Ale topics:
Atlas Credentials Topics:
atlas-account_request-status
sketch-investigation-status
 
Sentinel Credential Topics:
sentinel-ach-relationship-status
sentinel-ach-transfer-status
sentinel-ach-micro-deposit-transfer-status
 
 
Please send all tech issues/questions (API’s, SOD reports, etc) directly to techintegration@apexclearing.com and we will get them answered. The UAT environment will go down Monday – Friday from 6pm central – 2am central during batch processing*.  All requests will queue up during this timeframe and be processed when the system comes back online.
 *This also happens in production during batch hours of 6pm central – 2am central.
 
 
**Release Notes:  we post all of our release notes for UAT and Production.  Please become a watcher and you will be notified by email when changes are made.
https://github.com/apexclearing/release-notes
 
 
Atlas and Sentinel certification criteria:
 
Atlas – Account Management
Apex will need to see 25 successful account creations (spanning pertinent customer and account types) and 10 successful account updates before certifying the consumer for production access.
1.       Create 25 accounts for all customer types relevant to business model (Individual, Custodian, Joint or IRA) 
2.       Create accounts using the ACTION_REQUIRED SSN range and successfully APPROVE all actions using Sketch 
3.       Create accounts using the REJECT SSN range and successfully APPEAL all actions using Sketch 
4.       Upload image to Snap for a Sketch appeal and Appeal investigation
5.       Update 10 accounts successfully (should contain an update to account name and address)

Sentinel  - Cash Management
Apex will need to see 10 successful ACH deposits and withdrawals before certifying the consumer for production access.
1.       Create 10 successful ACH relationships via relevant approval methods (e.g., micro deposits, Yodlee, Plaid, etc.) 
2.       Successfully complete 10 ACH deposits
3.       Successfully complete 10 ACH withdraws (potentially includes withdrawal approval via simulation endpoint) 
4.       Cancel an ACH relationship
5.       Cancel an ACH Transfer
6.       Simulate an ACH return 
7.       Simulate a NOC (notice of change)
