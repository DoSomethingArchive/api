# Northstar Endpoints

`https://northstar.dosomething.org`

URL | HTTP Verb | Functionality
--- | --------- | -------------
`/login`                             | POST | [Logging In](https://github.com/DoSomething/northstar/wiki/Spec#logging-in)
`/logout`                            | POST | [Logging Out](https://github.com/DoSomething/northstar/wiki/Spec#logging-out)
`/users`                             | POST | [Registering a User](https://github.com/DoSomething/northstar/wiki/Spec#registering-a-user)
`/users`                             | GET | [Retrieve All Users](https://github.com/DoSomething/northstar/wiki/Spec#retrieve-all-users)
`/users/:term/:identifier`           | GET | [Retrieving a User](https://github.com/DoSomething/northstar/wiki/Spec#retrieving-a-user)
`/users/:_id`                        | PUT | [Updating a User](https://github.com/DoSomething/northstar/wiki/Spec#updating-a-user)
`/users/:_id`                        | DELETE | [Deleting a User](https://github.com/DoSomething/northstar/wiki/Spec#deleting-a-user)
`/users/:term/:identifier/campaigns` | GET | [Retrieving a User's Campaigns](https://github.com/DoSomething/northstar/wiki/Spec#retrieving-a-users-campaigns)
`/campaigns/:nid`                    | GET | [Retrieving a User's Activity on a Single Campaign](https://github.com/DoSomething/northstar/wiki/Spec#retrieving-a-users-activity-on-a-single-campaign)
`/campaigns/:nid/signup`             | POST | [Submitting a Campaign Sign Up](https://github.com/DoSomething/northstar/wiki/Spec#submitting-a-campaign-sign-up)
`/campaigns/:nid/reportback`         | POST/PUT | [Submitting a Campaign Report Back](https://github.com/DoSomething/northstar/wiki/Spec#submitting-a-campaign-report-back)
`/keys`                              | POST | [Creating an API Key](https://github.com/DoSomething/northstar/wiki/Spec#creating-an-api-key)
`/keys`                              | GET | [Retrieving All API Keys](https://github.com/DoSomething/northstar/wiki/Spec#retrieving-all-api-keys)