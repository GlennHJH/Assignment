# Assignment

# Task 1a
To run this script, save it as a file (e.g. apache_log_alert.sh) which i had done so, and make it executable (chmod +x apache_log_alert.sh). 
Then run it with the log file name as the argument (./apache_log_alert.sh apache_logs). 
You can set up a cron job to run this script periodically.

# Task 1b
A possible solution would be to archive the logs that are older than 3 months to a separate storage system or service, such as Amazon S3 or a tape backup system. The archived logs can be compressed and encrypted for security, and can be retrieved if needed for troubleshooting or audits. The remaining logs can be deleted or moved to a lower-cost storage system, such as a network attached storage (NAS) or a cloud-based storage service with infrequent access tiers. This can help to free up space on the machine and avoid running out of storage. It's important to ensure that the logging system is configured to rotate logs regularly and delete old logs to avoid accumulating too many logs in the future.

# Task 2
You will need to configure the email plugin in Jenkins to send email alerts. Additionally, you'll need to set up environment variables for the container registry and cloud instance credentials.
