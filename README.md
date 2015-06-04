# api.dosomething.org

Below are all links specifying the endpoint on our platforms.


## Platform 

- [Northstar Endpoints](https://github.com/DoSomething/api/tree/master#northstar-endpoints)
- [Drupal Endpoints](https://github.com/DoSomething/api/tree/master#drupal-endpoints)


### Northstar Endpoints

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
`/users/:_id/avatar`                 | POST | [Creating a User's Profile IMage](https://github.com/DoSomething/northstar/wiki/Spec#creating-a-users-profile-image)
`/users/:term/:identifier/campaigns` | GET | [Retrieving a User's Campaigns](https://github.com/DoSomething/northstar/wiki/Spec#retrieving-a-users-campaigns)
`/user/campaigns/:campaign_id`       | GET | [Retrieving a User's Activity on a Single Campaign](https://github.com/DoSomething/northstar/wiki/Spec#retrieving-a-users-activity-on-a-single-campaign)
`user/campaigns/:campaign_id/signup` | POST | [Submitting a Campaign Sign Up](https://github.com/DoSomething/northstar/wiki/Spec#submitting-a-campaign-sign-up)
`user/campaigns/:campaign_id/reportback`| POST/PUT | [Submitting a Campaign Report Back](https://github.com/DoSomething/northstar/wiki/Spec#submitting-a-campaign-report-back)
`/keys`                              | POST | [Creating an API Key](https://github.com/DoSomething/northstar/wiki/Spec#creating-an-api-key)
`/keys`                              | GET | [Retrieving All API Keys](https://github.com/DoSomething/northstar/wiki/Spec#retrieving-all-api-keys)


***


### Drupal Endpoints

`https://www.dosomething.org/api/v1`

URL | HTTP Verb | Functionality
--- | --------- | -----------
`/auth/login`               | POST | [Logging in](https://github.com/DoSomething/dosomething/wiki/API#user-login)
`/auth/logout`              | POST | [Logging out](https://github.com/DoSomething/dosomething/wiki/API#user-logout)
`/auth/token`               | POST | [Retrieve the X-CSRF Token for the logged in user](https://github.com/DoSomething/dosomething/wiki/API#get-authentication-token)
`/campaigns`                | GET  | [Retrieve all active campaigns](https://github.com/DoSomething/dosomething/wiki/API#retrieve-all-active-campaigns)
`/campaigns/:id`            | GET  | [Retrieve a specific campaign](https://github.com/DoSomething/dosomething/wiki/API#retrieve-a-campaign)
`/campaigns/:id/signup`     | POST | [Creates a User Signup for the given Campaign nid](https://github.com/DoSomething/dosomething/wiki/API#campaign-signup)
`/campaigns/:id/reportback` | POST | [Creates or updates a User Reportback for the given Campaign nid](https://github.com/DoSomething/dosomething/wiki/API#campaign-reportback)
`/campaigns/:id/gallery`    | GET  | [Retrieves approved Reportback Files for the given Campaign nid](https://github.com/DoSomething/dosomething/wiki/API#campaign-gallery)
`/reportbacks/:id`          | GET | [Retrieve a specific reportback](https://github.com/DoSomething/dosomething/wiki/API#retrieve-a-specific-reportback)
`/reportback-items`         | GET | [Retrieve a collection of reportback items](https://github.com/DoSomething/dosomething/wiki/API#retrieve-a-collection-of-reportback-items)
`/reportback-items/:id`     | GET | [Retrieve a specific reportback item](https://github.com/DoSomething/dosomething/wiki/API#retrieve-a-specific-reportback-item)
`/system/connect`           | POST | [Retrieves session info for a user](https://github.com/DoSomething/dosomething/wiki/API#connection-status)
`/system/set_variable`      | POST | [Set a system variable](https://github.com/DoSomething/dosomething/wiki/API#set-a-variable)
`/users`                    | GET  | [Get a user](https://github.com/DoSomething/dosomething/wiki/API#find-a-user)
`/users`                    | POST | [Create a drupal user](https://github.com/DoSomething/dosomething/wiki/API#create-a-user)
`/users/get_member_count`   | POST | [Retrieve member count](https://github.com/DoSomething/dosomething/wiki/API#get-member-count)


The following endpoints will be deprecated:

URL | HTTP Verb | Functionality
--- | --------- | -----------
`/content/:nid`                 | GET  | [Retrieve a campaign](https://github.com/DoSomething/dosomething/wiki/API#retrieve-a-campaign)
`/reportback_files/:fid/review` | POST | [Review a Reportback File](https://github.com/DoSomething/dosomething/wiki/API#review-a-reportback-file)
