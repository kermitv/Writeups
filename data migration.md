## Good links regarding SF data migration
* Good discussion https://success.salesforce.com/answers?id=9063A000000e2WLQAY
* Good article https://hub.appirio.com/tech-blog/salesforce-data-migration-best-practices

## DX
Handy commands
* lists all commands with short description
  * sfdx force:doc:commands:list
* lists all connected orgs
  * sfdx force:org:list

Must use a Dev Hub org to spin off scratch orgs
* Can be a dev org, playground/hands-on org or Prod org
* Authorize with sfdx force:auth:web:login -d -a DevHub
* only indicate -d for Dev Hub org
* can't creat scratch orgs until Dev Hub correctly identified config:set

### A quick project
On the CLI based on 
  [Get Ready to Create an App](https://trailhead.salesforce.com/content/learn/modules/sfdx_app_dev/sfdx_app_dev_create_app?trail_id=sfdx_get_started)
* CD to desired directory
* create project
  * sfdx force:project:create -n geolocation
  * alter config/project-scratch-def.json accordingly
* Create scratch org
  * cd to geolocation project directory
  * sfdx force:org:create -s -f config/project-scratch-def.json -a GeoAppScratch
  * using its alias, GeoAppScratch, in future commands that accept the -u parameter

