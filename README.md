# SEPM 14 Content Pack
Content pack for Symantec Endpoint Protection Manager 14.2

# Includes
* Grok patterns for SHA256 and MD5 hashes
* Grok pattern for MAC addresses
* Symantec Endpoint Protection stream
* Symantec Endpoint Protection pipeline
* Symantec Endpoint Protection pipeline rules for:
  * SEPM Authentication Events
  * SEPM Server logs
  * SEP Application Control Logs
  * SEP Client Logs
  * SEP Device Manager Logs
  * SEP IPS Logs
  * SEP Traffic Logs

# Requirements
Logging for related functionality must be configured on the Symantec Endpoint Protection Manager, and logs must be sent via syslog to Graylog.

# Note
Some default firewall rules include a comma (e.g., Allow ping, pong and tracert).  This comma causes quotes to be placed around the rule name, causing issues with processing.  If this occurs, the easiest solution is to remove the comma from the rule name (e.g., Allow ping pong and tracert).
