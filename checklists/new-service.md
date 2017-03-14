# Service planning checklist

These questions are intended to help in thinking through the implementation of a new service.

The "defaults" below are our standard tools. If you choose not to use a default, there should be a good reason why it doesn't work for your use case.

- **How will the service be deployed?** Default: Docker/Convox.
- **How will the service be tested?** Will the service have any behavior that automated tests can't capture?
- **Will continuous integration be set up for the service?** Default: Codeship.
- **Will the service have a staging environment?** If not, why not? Are there any complications involved in setting up a staging environment for this service?
- **How will the service be monitored?** Default: Honeybadger.
- **How will developers be alerted of errors?** Default: All Honeybadger errors are automatically reported in `#exceptions` channel in Slack.
- **What should the documentation for the service cover?** At a minimum, the documentation should explain the motivation for the creation of the service, how it works at a high level, how it fits into existing VHX infrastructure, and how to deploy the service (including where to find relevant credentials). Is there anything else that the documentation for this particular service should cover?
