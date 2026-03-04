# splunk-impossible-travel
Splunk SIEM lab demonstrating detection of impossible travel authentication events using login log analysis and SPL queries.
Impossible travel occurs when a user appears to log in from geographically distant locations within an unrealistic time window.
The lab simulates authentication logs and uses Splunk SPL queries to identify suspicious login behavior and generate a detection alert.

## Environment
Impossible travel occurs when a user appears to log in from geographically distant locations within an unrealistic time window.
The lab simulates authentication logs and uses Splunk SPL queries to identify suspicious login behavior and generate a detection alert.

## Detection Logic
The detection identifies users logging in from multiple geographic locations within a short time window. This behavior may indicate:
Account compromise
Credential theft
Session hijacking
VPN or proxy abuse

## Initial Query Results
This query was ran prior to the creation of the alert.
![Initial Query Results](screenshots/initial_query_results_r2.png)

## Log Ingestion
Authentication logs were ingested into the Splunk main index.
![Log Ingestion](screenshots/log_ingestion_index_main_r2.png)

## Detection Query Results
This query identifies users logging in from multiple locations.
![Detection Query Results](screenshots/impossible_detection_results_r2.png)

## Alert Configuration
A scheduled alert was created to automatically detect impossible travel activity.
![Alert Configuration](screenshots/impossible_travel_alert_configuration.png)

## Security Impact
Impossible travel detection helps identify potential account compromise or credential misuse by analyzing login patterns across geographic locations.
Organizations commonly deploy this detection as part of:
Security Operations Center (SOC) monitoring
Identity threat detection
User behavior analytics

## Skills Demonstrated
Impossible travel detection helps identify potential account compromise or credential misuse by analyzing login patterns across geographic locations.
Organizations commonly deploy this detection as part of:
Security Operations Center (SOC) monitoring
Identity threat detection
User behavior analytics
