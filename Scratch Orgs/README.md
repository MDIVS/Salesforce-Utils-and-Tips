# [Back to HOME](../README.md)  

# Commands table
**Create a scratch org:**  
sfdx force:org:create -f project-scratch-def.json -a \<MyScratchOrg> --setdefaultusername </br>
| PARAM | NEEDED | TYPE | DESCRIPTION |
| - | - | - | - |
| --json     | false | boolean | Format output as JSON |
| --loglevel | false | enum | The logging level for this command invocation. Logs are stored in $HOME/.sfdx/sfdx.log. Permissible values are: trace, debug, info, warn, error, fatal, TRACE, DEBUG, INFO, WARN, ERROR, FATAL. Default value: warn. |
| -v \| --targetdevhubusername | false | string | A username or alias for the target Dev Hub org. Overrides the default Dev Hub org.
| -u TARGETUSERNAME
| --apiversion APIVERSION
| -t TYPE
| -f DEFINITIONFILE
| -n
| -c
| -i CLIENTID
| -s
| -a SETALIAS
| -w WAIT
| -d DURATIONDAYS

**Authorize an org** </br>
sfdx auth:web:login -a aliasdaorg 

**Display all orgs:** </br>
sfdx force:org:list

**Opening an org:** </br>
sfdx force:org:open -u \<orgusername>

**Deleting an org:** </br>
sfdx force:org:delete -u \<orgusername>

**Install CPQ package:** </br>
sfdx force:package:install --package 04t4N000000szN1QAI -w 1 -u PJ1126_Sprint1