# Service planning checklist

These questions are intended to help in thinking through the implementation of a new service.

- **How will the service be deployed?** Default: Docker/Convox.
- **How will the service be tested?** Will the service have any behavior that automated tests can't capture?
- **Will continuous integration be set up for the service?** Default: Codeship.
- **Will the service have a staging environment?** If not, why not? Are there any complications involved in setting up a staging environment for this service?
- **How will the service be monitored?** Default: Honeybadger.
- **How will developers be alerted of errors?** Default: All Honeybadger errors are automatically reported in `#exceptions` channel in Slack.
