`Hi`
To any Operations Team, Key Performance Indicators (KPIs) play an essential role in keeping the applications running and stakeholders happy.
There were a lot of metrics and reports which flow along timely-mails and in-house dashboards. But what was really lacking is: ‘Intelligence’. We needed to empower and enable the user view these reports to predict, analyze trends and draw conclusions. We came across a rich open source tool from Apache: Superset. It still being in its incubating phase, it does offer a solution to what we were looking at. For folks looking a dockerized version, it is available too.
We then started evaluating on how well we can fit in Superset to our day-to-day operational activities.
Activity 1: A Cost Analysis solution (Infrastructure Cost dashboard)
To keep our budgets in check, we hosted a Superset dashboard which displayed our cost consumption for our infrastructure. We rely on AWS indirectly. Meaning, we get our AWS components provisioned by Philips HealthSuite Digital Platform (HSDP). From HSDP’s bill, we configured the dashboard categorizing it into: Overall summary, EC2, S3, RDS & Cloud foundry runtime.
Result? We have now made static numbers speak more. Our management now not only get a high level view on the billing summary, but also the cost consumed by a single Project ‘per’ Environment ‘per’ AWS component.
Activity 2: Monitoring Dashboards (E2E device monitoring)
Operations Team is responsible to combat any downtime or bottlenecks in the platform/infrastructure end-to-end. By not investing much time to build a customized in-house dashboard tool, we were able construct complex queries and embed them in Superset instead. With Redis integrated into Superset, caching was also taken care, which did not burden the database engine. So now, we have production ready dashboards used to monitor bottlenecks in our infrastructures. Superset was also able to nicely fit in Single-Sign-On. This enabled us to onboard federated users.
These were just few scenarios where we have used Superset.
Conclusion: Superset can be a better alternative to any licensed business intelligence tool on a small scale. Note that this tools is fits our use case, it may vary for others. I would suggest people to have the security officer check this before your introduce this tool in your organization.

```
hello
```
