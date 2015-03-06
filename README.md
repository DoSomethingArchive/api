# api.dosomething.org

Below are the enpoints all in both the northstar api and the drupal api

### Northstar Endpoints

`https://northstar.dosomething.org`

URL | HTTP Verb | Functionality
--- | --------- | -------------
`/login`                             | POST  | [Logging In](https://github.com/DoSomething/northstar/wiki/Spec#logging-in)
`/logout`                            | POST  | [Logging Out](https://github.com/DoSomething/northstar/wiki/Spec#logging-out)
`/users`                             | POST  | [Registering a User](https://github.com/DoSomething/northstar/wiki/Spec#registering-a-user)
`/users`                             | GET   | [Retrieve All Users](https://github.com/DoSomething/northstar/wiki/Spec#retrieve-all-users)
`/users/:term/:identifier`           | GET   | [Retrieving a User](https://github.com/DoSomething/northstar/wiki/Spec#retrieving-a-user)
`/users/:_id`                        | PUT   | [Updating a User](https://github.com/DoSomething/northstar/wiki/Spec#updating-a-user)
`/users/:_id`                        | DELETE| [Deleting a User](https://github.com/DoSomething/northstar/wiki/Spec#deleting-a-user)
`/users/:term/:identifier/campaigns` | GET   | [Retrieving a User's Campaigns](https://github.com/DoSomething/northstar/wiki/Spec#retrieving-a-users-campaigns)
`/campaigns/:nid/signup`             | POST  | [Submitting a Campaign Sign Up](https://github.com/DoSomething/northstar/wiki/Spec#submitting-a-campaign-sign-up)
`/campaigns/:nid/reportback`         | POST  | [Submitting a Campaign Report Back](https://github.com/DoSomething/northstar/wiki/Spec#submitting-a-campaign-report-back)
`/campaigns/:nid/reportback`         | PUT   | [Updating a Campaign Report Back](https://github.com/DoSomething/northstar/wiki/Spec#updating-a-campaign-report-back)
`/keys`                              | POST  | Generate new api key


### Drupal Enpoints

`https://www.dosomething.org/api/v1`

URL | HTTP Verb | Functionality
--- | --------- | -----------
`/auth/login`                    | POST | [Logging in](https://github.com/DoSomething/dosomething/wiki/API#user-login)
`/auth/logout`                   | POST | [Logging out](https://github.com/DoSomething/dosomething/wiki/API#user-logout)
`/auth/token`                    | POST | [Retrieve the X-CSRF Token for the logged in user](https://github.com/DoSomething/dosomething/wiki/API#get-authentication-token)
`/content/:nid`                  | GET  | [Retrieve a campaign](https://github.com/DoSomething/dosomething/wiki/API#retrieve-a-campaign)
`/campaigns`                     | GET  | [Retrieve all active campaigns](https://github.com/DoSomething/dosomething/wiki/API#retrieve-all-active-campaigns)
`/campaigns/:nid/signup`         | POST | [Creates a User Signup for the given Campaign nid](https://github.com/DoSomething/dosomething/wiki/API#campaign-signup)
`/campaigns/:nid/reportback`     | POST | [Creates or updates a User Reportback for the given Campaign nid](https://github.com/DoSomething/dosomething/wiki/API#campaign-reportback)
`/campaigns/:nid/gallery`        | GET  | [Retrieves approved Reportback Files for the given Campaign nid](https://github.com/DoSomething/dosomething/wiki/API#campaign-gallery)
`/reportback_files/:fid:/review` | POST | [Review a Reportback File](https://github.com/DoSomething/dosomething/wiki/API#review-a-reportback-file)
`/system/connect`                | POST | [Retrieves session info for a user](https://github.com/DoSomething/dosomething/wiki/API#connection-status)
`/system/set_variable`           | POST | [Set a system variable](https://github.com/DoSomething/dosomething/wiki/API#set-a-variable)
`/users`                         | GET  | [Get a user](https://github.com/DoSomething/dosomething/wiki/API#find-a-user)
`/users`                         | POST | [Create a drupal user](https://github.com/DoSomething/dosomething/wiki/API#create-a-user)
`/users/get_member_count`        | POST | [Retrieve member count](https://github.com/DoSomething/dosomething/wiki/API#get-member-count)
 

***

## Proposed Endpoints

### Drupal Endpoints (suggested)

URL | HTTP Verb | Functionality
--- | --------- | -----------
`/reportbacks`                                              | GET | Retrieve all reportbacks
`/reportbacks/:rbid`                                        | GET | Retrieve a specific reportback
`/reportbacks/campaign/:nid`                                | GET | Retrieve all reportbacks for a specific campaign
`/reportbacks/campaign/:nid?status=promoted,approved`       | GET | Retrieve all reportbacks for a specific campaign filtered by parameters
`/reportbacks/campaign?nids=:nid,:nid,:nid`                 | GET | Retrieve all reportbacks for multiple specified campaigns
`/reportbacks/campaign?nids=:nid,:nid,:nid&status=approved` | GET | Retrieve all reportbacks for multiple specified campaigns filtered by parameters


URL | HTTP Verb | Functionality
--- | --------- | -----------
`/campaigns/:nid/reportbacks`                          | GET | For a specific campaign, retrieve all reportbacks
`/campaigns/:nid/reportbacks/:rbid`                    | GET | For a specific campaign, retrieve a specific reportback
`/campaigns/:nid/reportbacks?status=promoted,approved` | GET | For a specific campaign, retrieve all reportbacks filtered by parameters


URL | HTTP Verb | Functionality
--- | --------- | -----------
`/users/:uid/reportbacks`                       | GET | For a specific user, retrieve all reportback *files*
`/users/:uid/reportbacks/:rbid`                 | GET | For a specific user, retrieve all reportback *files* for a specific reportback
`/users/:uid/reportbacks/:rbid?status=promoted` | GET | For a specific user, retrieve all reportback *files* for a specific reportback filtered by parameters








