# TA-cisco_acs
Splunk TA for Cisco ACS Data


## ToDo:

* Props needs specific timestamp and line breaking configs
* The primary field extractions need some more work, but most fields are being extracted correctly

## Note

ACS data has many mostly useless fields with the same field names:
* Step=<something>
* StepData=<something>

The SEDCMD commands in props.conf will remove these fields prior to indexing if the TA is installed on the first full Splunk instance on the way to the indexer(s).  
