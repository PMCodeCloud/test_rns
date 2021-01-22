- [DB Upgrade Service Configuration](#_DB_Upgrade_Service)
  - [DBUS Configuration: 1.0.188](#_DBUS_Configuration:_1.0.188)
  - [DBUS Configuration: 1.0.164](#_DBUS_Configuration:_1.0.164)
  - [DBUS Configuration: 1.0.147](#_DBUS_Configuration:_1.0.147)
  - [DBUS Configuration: 1.0.146](#_DBUS_Configuration:_1.0.146)
  - [DBUS Configuration: 1.0.140](#_DBUS_Configuration:_1.0.140)
  - [DBUS Configuration: 1.0.136](#_DBUS_Configuration:_1.0.136)
  - [DBUS Configuration: 1.0.132](#_DBUS_Configuration:_1.0.132)
  - [DBUS Configuration: 1.0.132](#_DBUS_Configuration:_1.0.132)
  - [DBUS Configuration: 1.0.128](#_DBUS_Configuration:_1.0.128)
  - [DBUS Configuration: 1.0.108](#_DBUS_Configuration:_1.0.108)
  - [DBUS Configuration: 1.0.80](#_DBUS_Configuration:_1.0.80)
  - [DBUS Configuration: 1.0.73](#_DBUS_Configuration:_1.0.73)
  - [DBUS Configuration: 1.0.59](#_DBUS_Configuration:_1.0.59)
  - [DBUS Configuration: 1.0.51](#_DBUS_Configuration:_1.0.51)
  - [DBUS Configuration: 1.0.46](#_DBUS_Configuration:_1.0.46)
  - [DBUS Configuration: 1.0.22](#_DBUS_Configuration:_1.0.22)
- [DB Upgrade Service](#_DB_Upgrade_Service_1)
  - [DBUS Version: 1.0.224](#_DBUS_Version:_1.0.224)
  - [DBUS Version: 1.0.222](#_DBUS_Version:_1.0.222)
  - [DBUS Version: 1.0.214](#_DBUS_Version:_1.0.214)
  - [DBUS Version: 1.0.207](#_DBUS_Version:_1.0.207)
  - [DBUS Version: 1.0.189](#_DBUS_Version:_1.0.189)
  - [DBUS Version: 1.0.181](#_DBUS_Version:_1.0.181)
  - [DBUS Version: 1.0.164](#_DBUS_Version:_1.0.164)
  - [DBUS Version: 1.0.157](#_DBUS_Version:_1.0.157)


|<h1>**DB Upgrade Service Configuration**</h1>|
| :- |
|<p><h2>DBUS Configuration: 1.0.188</h2></p><p>**December 15, 2020**</p>|
|**Agile Studio reference**|**Enhancement**|
|*US-387268*|Unify DBUS deployment|
|*US-375517*|Remove RDS CA Certificate update|
|<p><h2>DBUS Configuration: 1.0.164</h2></p><p>**July 3, 2020**</p>|
|**Agile Studio reference**|**Change or enhancement**|
|*BUG-554926*|Changed flow to execute rolling restart after upgrade|
|<p><h2>DBUS Configuration: 1.0.147</h2></p><p>**January 28, 2020**</p>|
|**Agile Studio reference**|**Change or enhancement**|
|*US-342791*|Modified exceptions handling raised by get-instances lambda|
|<p><h2>DBUS Configuration: 1.0.146</h2></p><p>**January 21, 2020**</p>|
|*US-342407*|Modify timeout to 5s for curl in docker-check-health |
|*US-338670*|Refactor subflow versioning|
|<p><h2>DBUS Configuration: 1.0.140</h2></p><p>**January 7, 2020**</p>|
|*ISSUE-70975*|A dry run doesn’t check Pega environment health|
|*US-341368*|Introduced 5 retries on Pega health check verification after ASG has been enabled|
|*US-341368*|Minor timeout changes |
|<p><h2>DBUS Configuration: 1.0.136 </h2></p><p>**December 25, 2019**</p>|
|*US-330553*|Reducing the number of AWS API calls to the AWS autoscaling API|
|<p><h2>** DBUS Configuration: 1.0.132</h2></p><p>` `**December 16, 2019**</p>|
|*US-337246*|Modified pega-health subflow to perform additional checks |
|<p><h2>DBUS Configuration: 1.0.128</h2></p><p>**December 12, 2019**</p>|
|*BUG-528250*|**Bugfix**: Fixed script for PostGIS check/removal|
|*BUG-527559*|**Bugfix**: Improved Pega Health check script|
|<p><h2>DBUS Configuration: 1.0.108</h2></p><p>**December 5, 2019**</p>|
|*US-336869*|Support for an upgrade to PG 11.5 from PG 9.4.20,9.6.11,11.1,11.4 |
|*-*|Upgrades to PG 11.5 were extended for change of the RDS certificate|
|*-*|<p>Dry run functionality for PG 11.5 has been extended to verify if the environment has ForceSSL set and if true if the version is at least 2.14 ( **Note that the service is unable to distinguish between 2.14.1 and 2.14.3** )</p><p></p>|
|*-*|<p>Dry run has been extended to perform actual Pega Ping to verify the health of the environment before the upgrade</p><p></p>|
|*US-321554*|All upgrade flows have been divided into a collection of smaller flows (subflows)|
|*-*|<p>Extended error reporting by marking failed subflows in a service API response</p><p></p>|
|*-*|<p>Even after a failed upgrade, the Autoscaling processes are enabled</p><p></p>|
|*-*|<p>Additional verification has been implemented that verity’s if the enabled autoscaling processes (and the instance replacement potentially caused by it) did not move the environment into a healthy state</p><p></p>|
|*-*|<p>With the introduction of subflows logging streams in CloudWatch logs have been reorganized</p><p></p>|
|As part of *SR-D66017*|<p>**Bugfix:** Creating downtimes in DD monitoring has been deployed</p><p></p>|
|DBUS Configuration: 1.0.85<br>**November 22, 2019**|
|*BUG-521280*|**Bugfix:** Log sending from script failed|
|*BUG-527559*|**Bugfix:** DBUS marks the instance as unhealthy after upgrade too soon|
|<p><h2>** DBUS Configuration: 1.0.80</h2></p><p>**November 6, 2019**</p>|
|*US-330556*|Kafka's health is verified after DB Upgrade |
|<p><h2>** DBUS Configuration: 1.0.73</h2></p><p>` `**November 1, 2019**</p>|
|*US-329902*|Block DB upgrades to Postgres 11.4 from PG 9.4.20 and 9.6.11 on cloud infrastructure 2.12|
|*US-329902*|Upgrades to Postgres 11.4 from PG 9.4.20 and 9.6.11 available on cloud infrastructure 2.13|
|*US-329924*|Checking RDS version after every upgrade|
|*US-330557*|Improved pega health-check on post-DB upgrade actions|
|*BUG-518262*|**Bugfix:** "Check if Postgis plugin installed" returns accurate exit code|
|<p><h2>DBUS Configuration: 1.0.59</h2></p><p>**October 1, 2019** </p>|
|*US-326328*|Added support of PG11 for Pega 7.2 and Pega 7.3|
|*ISSUE-66494*|Correction of Data sync pipeline|
|<p><h2>DBUS Configuration: 1.0.51</h2></p><p>**September 6, 2019**<br> </p>|
|**-**|<p>Added support for Hong Kong Region </p><p></p>|
|*ISSUE-65221*|Pg stat statements added after upgrade to 11.1 in upgrade flow 9.4.20 to 11.4 and 9.6.11 to 11.4|
|*ISSUE-65221*|Added new fail state for failing PG plugin update in upgrade 9.4.20 to 11.4|
|<p><h2>** DBUS Configuration: 1.0.46</h2></p><p>**August 15, 2019**</p>|
|*ISSUE-64474*|Moved flow integration tests execution from a pipeline to a script|
|*ISSUE-64704*|**Bugfix**: Fix "invalid option name" message in SSM script|
|<p><h2>DBUS Configuration: 1.0.22	</h2></p><p>**August 13, 2019**</p>|
|*ISSUE-64633*|Added production deployment pipeline|
|*ISSUE-64472*|Added timeouts to Jenkins pipelines|
|*ISSUE-64053*|Send email notification when a master build fails|
|*ISSUE-63912*|Changed version to 1.0.x|


|<h1>**DB Upgrade Service**</h1>|
| :- |
|<p><h2>**CC-104863</h2><br>` `DBUS Version: 1.0.264**</h2></p><p>**December 30, 2020 -** </p>|
|Agile Studio reference|**Change or enhancement**|
|***US-387268***|Unify DBUS deployment|
|***US-375517***|Remove RDS CA Certificate update|
|<p><h2>` `**CC-88711 DBUS Version: 1.0.236**</h2></p><p>**July 3 2020** </p>|
|***BUG-554926***|Added PeRollingRestart lambda to allow rolling restarts of tiers + fixing Sonar issues|
|<p><h2>**DBUS Version: 1.0.224**</h2></p><p>**February 12, 2020 SR-D78308**</p>|
|<p>***US-342791***</p><p></p>|Added instances state filtering to get-instances lambda |
||Error statuses replaced with exceptions raised|
|***US-342773)***|Introduce new deliveryTimeout variable|
|<p><h2>**DBUS Version: 1.0.222**</h2></p><p>**January 20, 2020**</p>|
|***ISSUE-70647***|Log info about unhealthy instances and set healthy state just before resuming autoscaling processes |
|***US-341437***|Validate if each of environment's SCE is healthy before starting the DB upgrade|
|***US-338670***|Refactor subflow versioning|
|<p><h2>` `**DBUS Version: 1.0.214**</h2></p><p>**December 25, 2019**</p>|
|***US-330553***|Reducing the number of AWS API calls to the AWS autoscaling API|
|***BUG-527140***|**Bugfix**: Read correct cause and error for UpgradeStatusEvent, when execution timed out|
|***BUG-527065***|**Bugfix**: Pass dryRun parameter as a boolean to AWSStepFunctions to detect unhealthy environments|
|***BUG-525141***|**Bugfix**: Wait until RDS becomes available before cleanup in integTests|
|<p><h2>**DBUS Version: 1.0.207**</h2></p><p>**December 9, 2019**</p>|
|***US-321565***|Added support of sub-flows to db-upgrade lambda|
|***US-321554***|Use sub-flows in db-upgrade service |
|***ISSUE-69427***|Integrate US-320945 (replace instances by ASG) into new subflows|
|***US-336869***|DB Upgrade service changes the certificate during an upgrade to 11.5|
|***BUG-521275***|**Bugfix**: Wrong script logging in restart pega web containers task|
|***BUG-492548***|**Bugfix**: Retain logs in case of PE build failure |
|***BUG-520373***|**Bugfix**: Email notifications are not sent when new PE is built|
|<p><h2>**DBUS Version: 1.0.189**</h2></p><p>**November 6, 2019**</p>|
|***US-328334***|Set minimal access rights set on all db-upgrade service lambdas|
|***US-329924***|Check database version directly from RDS |
|***ISSUE-65480***|Added SonarQube to db-upgrade service |
|<p><h2>**DBUS Version: 1.0.181**</h2></p><p>**September 24, 2019**</p>|
|**	|Added support for Hong Kong Region|
|***ISSUE-65786***|Move the SOP document from git to Pega Box|
|***ISSUE-65970***|Corrected validation service bucket name in research|
|<p><h2>**DBUS Version: 1.0.164**</h2></p><p>**August 13, 2019**</p>|
|***ISSUE-64482***|Log to stdout using AWS's Lambda appender instead of CloudWatchAppender|
|***ISSUE-64053***|Send email notification when a master build fails|
|***US-312998***|Added CFN to supported-db-target lambda, added SupportedDbTargets to outputs of SCE|
|***ISSUE-63912***|Changed version to 1.0.x|
|***BUG-503990***|**Bugfix**: Throttling exception handling fixed|
|***BUG-503703***	|**Bugfix**: Lambda upgradeDb creates logs in an incorrect region|
|<p><h2>` `**DBUS Version: 1.0.157**</h2></p><p>**August 7, 2019**</p>|
|***US-314129***|Improved UpgradeEnvironmentDbStatus error messages|
|***ISSUE-63852***|Improved throttling handling|
|***ISSUE-63762***|Added configurationVersion to flow parameters and UpdateStatus|
|***ISSUE-63204***|Added State Machnie ARN logging|
|***BUG-499419***|**Bugfix**: UpgradeEnvironmentDbStatus API not returning flowErrorCause |

