# splunk-impossible-travel
Splunk SIEM lab demonstrating detection of impossible travel authentication events using login log analysis and SPL queries.

## Intial Query Results
This query was ran prior to the creation of the alert.
![Detection Query Results](screenshots/detection_query_results_r2.png)

## Log Ingestion
Authentication logs were ingested into the Splunk main index.
![Log Ingestion](screenshots/log_ingestion_index_main_r2.png)

## Detection Query Results
This query identifies users logging in from multiple locations.
![Detection Query Results](screenshots/impossible_travel_detection_query_results_r2.png)

## Alert Configuration
A scheduled alert was created to automatically detect impossible travel activity.
![Alert Configuration](screenshots/impossible_travel_alert_configuration_r2.png)
