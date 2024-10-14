Testing in Production Approach
===================================

Testing in production is vital and critical in making decisions that can drive product success.

Let's look at ways to conduct testing in production environments.

✔️ **Canary Test**:  
Distribute traffic between the new version alongside the production version deployed. Test and evaluate the latest version of the application by routing some amount of traffic to the canary version.

✔️ **A/B Test**:  
Route a subset of users to a new version based on rules (like geolocation, selected users, browser version, and other criteria) and carry out testing.

✔️ **Rolling Test**:  
The team releases a new version by updating subsets of servers group by group while conducting testing during the rollout process.

✔️ **Blue-Green Test**:  
Two exactly similar environments running the application. Deploy a new version on one environment, test, and switch over traffic so end users get to use the latest version.

✔️ **Tap Compare Test**:  
Record the response traffic from existing and recently launched environments. Analyze and compare the outcomes based on predefined evaluation criteria used for testing purposes.

✔️ **Synthetic Test**:  
Automated tests, including UI, SSL, and performance, are regularly conducted to evaluate the production environment's functionality, performance, page loading speed, 404 errors, and other critical aspects, ensuring proper operation.

✔️ **Chaos Test**:  
Tests that are carried out to evaluate how the system behaves when there are outages or failures in the production environment. Tests are devised to simulate many of these failure conditions on the production environment.

✔️ **Feature Flag Test**:  
Feature flags allow you to turn features on and off. Features are tested in production using this under various conditions to evaluate correctness, risk, performance, and other aspects.

✔️ **Observability-Based Test**:  
Traces, logs, and metrics provide vital information, and testing can also benefit from this traceability. Captured traces can be asserted, tests can be generated based on these traces, and many other validations can be carried out.

✔️ **Dog Fooding Test**:  
This is a strategy to have internal employees test the new version of the product, diverting 50% of employee traffic to a few production instances so that the product can be evaluated before being turned over to customers.

✔️ **Shadow Test**:  
Traffic is captured and replayed across environments to test for correctness, functioning, performance, etc. Production traffic is captured and replayed on the new version of the release for testing and evaluation.

✔️ **Distributed Test**:  
Mimicking everything in QA environments as the production environment is challenging; hence, running some tests like integration tests, scalability tests, and devising disaster recovery tests becomes vital in the production environment.
