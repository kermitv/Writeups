## Good links regarding SF data migration
* Good discussion https://success.salesforce.com/answers?id=9063A000000e2WLQAY
* Good article https://hub.appirio.com/tech-blog/salesforce-data-migration-best-practices

DX
Handy commands
* sfdx force:doc:commands:list
** lists all commands with short description
*sfdx force:org:list
** lists all connected orgs

Must use a Dev Hub org to spin off scratch orgs
* Can be a dev org, playground/hands-on org or Prod org
* Authorize with sfdx force:auth:web:login -d -a DevHub
* only indicate -d for Dev Hub org
* can't creat scratch orgs until Dev Hub correctly identified config:set


