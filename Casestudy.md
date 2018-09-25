Development Environment (sinatra api) (shared workforce) (scala) (blazemeter) (buildpack api)

●Developers use this environment to do unit testing

○Developers write code

○Check in code to be included in next Build

○Build will be added to Development Environment

○Developer will unit test


QA Environment (rainforest qa) (blaze meter) (elasticsearch?)

●After code/build has been successfully built in development environment, code/build will be released to QA environment

○Smoke Test

○Test New Features or Fixes

○Regression Test


Staging / Pilot Environment (heroku beta features) (heroku CI:browswer and user aceptance testing uat)(heroku uat via 3rd party providers)(the headless chrome buildpack)(selenium)(springboot?)(piplines??)


●After code is validated in QA, code is moved to the Staging environment also known as Pilot or Pre-Production environment

○User Validation 

○Training

○Holding Area

●Also called a Pre-Production environment


Production Environment (edge)(realemail)(productioncheck)(chatOps-slackintegration)(symfony)


●After software has passed acceptance testing, code is moved to where the application or system will reside and host actual / real data (as opposed to test data) or is available on a publicly accessible network or server.



