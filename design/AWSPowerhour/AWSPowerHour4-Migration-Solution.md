**S1 E4 Homework:**
Select ONE phase of the migration process AND one of the seven “R”s of the migration workflow. Describe how you would use the phase and “R” to solve a scenario of your choice.

**Solution:** 

Out of the three phases of Migration Process:
1.	Assess
2.	Mobilize/Readiness and Planning
3.	Migrate & Modernize

**I would choose phase 3 of “Migrate & Modernize” for the use case.**

I am taking an assumption of a medium scale web application of an Event ticket booking company who wants to migrate their application to AWS cloud after initial business success while using an on-premises infrastructure.

Before we have reached the phase 3 of Migrate & Modernize, we understand that “Assess”phase has been completed with Migration Readiness Assessment, TCO, Discovery and other detailed business case documentation.

Also, the second phase of “Mobilize” has been executed with “Application Discovery”, “Landing zone”, “Control Tower” setup and various Governance processes.

For Migrate & Modernize phase, I would distribute the migration in various “Wave” – wave1, wave2, … and so on with specific milestone.

**I would choose “Replatform” out of the “7R”s.**

Will start with AWS Migration Hub to centrally track all the migration activity.

For various layer of application, will leverage various AWS tools –

Application layer: AWS Application Migration Service(MGN) to migrate to AWS Compute services.

Database layer: AWS Database Migration Service(DMS) with Schema conversion Tool to Migrate to AWS RDS or other AWS DB.

Data layer: AWS DataSync(along with AWS Transfer Family if needed) to transfer data from On-Prem Data center Filesystems to AWS S3, AWS EFS File System and others . For bigger chunk of data which can’t be quickly migrated via Direct Connect or VPN, AWS Snow Family can be utilized.

![AWSPowerHour4-Migration-SolutionDiag.svg](..%2F..%2F..%2F..%2FDownloads%2FAWSPowerHour4-Migration-SolutionDiag.svg)

Once, the waves of the migration are successful on shifting the applications to AWS, the cloud mature team can proceed to next waves of Cloud Native applications migration(and new development) with “Refactor” phase. 
