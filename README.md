`jiok` is a very small CLI to check [Jira's status](https://jira-software.status.atlassian.com/) and incidents from the terminal.

Based on Aaron Bennet's [ghok](https://github.com/abennett/ghok#readme) which does the same for Github. All I did was change the URL because they have identical APIs.

### Example Output
```
=== Components as of 11 Apr 22 15:34 UTC ===
Viewing content                    ✅
Create and edit                    ✅
Authentication and User Management ✅
Search                             ✅
Notifications                      ✅
Administration                     ✅
Marketplace                        ✅
Mobile                             ✅
Purchasing & Licensing             ✅
Signup                             ✅
Automation for Jira                ✅

=== Incidents ===
Name:         Multiple sites showing down/under maintenance
Impact:       🔴 critical
Status:       identified
Details:      A small number of Atlassian customers continue to experience service outages and are unable to access their sites. Our global engineering teams are working 24/7 to make progress on this incident. At this time, we have rebuilt functionality for over 35% of the users who are impacted by the service outage, with no reported data loss. The rebuild stage is particularly complex due to several steps that are required to validate sites and verify data. These steps require extra time, but are critical to ensuring the integrity of rebuilt sites. We apologize for the length and severity of this incident and have taken steps to avoid a recurrence in the future.
Link:         https://stspg.io/qvyflkjsl57b
Last Updated: 11 Apr 22 15:34 UTC
```

### Building from source

`go build -o jihok main.go`

Then place the resulting `jihok` executable in your PATH.
