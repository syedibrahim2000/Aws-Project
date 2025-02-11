Project Abstract:
The project focused on setting up a robust monitoring and logging system for a web application deployed on AWS for client XYZ. The application was hosted on an Apache web server within an EC2 instance, with supporting infrastructure using Amazon S3, EBS. The web server in EC2 accessed files stored in S3, with an additional EBS volume for persistent data processing, Key metrics were collected from each AWS resource, forming the basis for a comprehensive dashboard for continuous monitoring and alerts. Additionally, AWS CloudTrail was configured to track API calls and user activity, while AWS Config monitored resource configuration changes to enhance compliance and governance.
Services Used:
•	Amazon EC2 for hosting the Apache web server.
•	Amazon S3 for storing and syncing main files required by the web server.
•	Amazon EBS for persistent storage attached to EC2 for processing files..
•	Amazon CloudWatch for collecting metrics, creating dashboards, and setting up alarms.
•	AWS CloudTrail for monitoring API calls and user activity tracking.
•	AWS Config for tracking configuration changes to enhance resource governance and compliance.
Project Details Steps (as Completed by Me):

1.	Infrastructure Setup:

o	Deployed an Apache web server on an EC2 instance for the web application.
o	Configured S3 for file storage, where the main files were synced to the EC2 instance.
o	Attached an EBS volume to the EC2 instance for processing files that required persistent storage.
o	Set up Amazon RDS and integrated it with the EC2-hosted web server for database functionality using JavaScript.

2.	Monitoring Configuration:
o	Configured Amazon CloudWatch to collect key metrics for EC2, EBS, S3, and RDS, including CPU utilization, memory usage, disk read/write, and network performance.
o	Built a centralized CloudWatch dashboard displaying real-time performance metrics and utilization data for each resource.
o	Enabled AWS CloudTrail to capture and log all API calls and user interactions for auditing purposes.
o	Implemented AWS Config to monitor changes in resource configurations and ensure compliance with predefined policies.

3.	Alert and Notification Setup:
o	Defined CloudWatch alarms for critical thresholds, such as high CPU utilization, excessive latency in RDS, or low storage space in EBS.
o	Configured notifications through Amazon SNS to alert the operations team for any alarm triggers.

4.	Log Management and Analytics:
o	Enabled CloudWatch Logs for each resource to store and analyze logs, including application logs from the web server on EC2.
o	Implemented log analytics to gain insights into performance bottlenecks, request patterns, and error frequency.
o	Leveraged CloudTrail and Config logs for detailed analysis of API usage, user activity, and resource changes.

5.	Testing and Optimization:
o	Conducted load testing on the EC2 instance and monitored responses from the integrated RDS to validate performance.
o	Fine-tuned alarm thresholds and dashboard metrics based on observed performance during testing.
o	Verified that CloudTrail and Config captured all relevant events and configuration changes for enhanced monitoring.

