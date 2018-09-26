# Case Study: Heroku
## The various ways you could use Heroku to implement a CI solution

#### Development Environment > GitHub Integration

●Developers use this environment to do unit testing

For the development environment, Heroku integrates with GitHub to make it easy to deploy code living on GitHub to apps running on Heroku. When GitHub integration is configured for a Heroku app, Heroku can automatically build and release (if the build is successful) pushes to the specified GitHub repo.



#### QA Environment > Heroku Private Spaces

●After code/build has been successfully built in development environment, code/build will be released to QA environment

Private Spaces are dedicated environments for running dynos and certain types of add-ons within an isolated network. Access to apps in a Private Space can be controlled at the network level. Outbound requests from apps in a Private Space originate from a set of stable IP addresses, which allows you to securely communicate with IP white-listed services on-premise or on other networks. Private Spaces enable you to build and run Heroku apps that meet strict requirements for data protection and change control, as commonly required by corporate and regulatory governance standards.



#### Staging / Pilot Environment > Heroku CI

●After code is validated in QA, code is moved to the Staging environment also known as Pilot or Pre-Production environment



Heroku CI provides support for browser testing, or “user acceptance testing” (UAT) by providing a options for installing browsers in your test run dyno. Users can choose between Google Chrome stable, beta, and unstable release channels supported by either the new --headless flag or Xvfb.




#### Production Environment > Release Phase

●After software has passed acceptance testing, code is moved to where the application or system will reside and host actual / real data (as opposed to test data) or is available on a publicly accessible network or server.

Release phase enables you to run certain tasks before a new release of your app is deployed. Release phase can be useful for tasks such as:

Sending CSS, JS, and other assets from your app’s slug to a CDN or S3 bucket
Priming or invalidating cache stores
Running database schema migrations
If a release phase task fails, the new release is not deployed, leaving the current release unaffected.




