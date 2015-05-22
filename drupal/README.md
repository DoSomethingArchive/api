# Drupal Endpoints

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



***



The following endpoints will be deprecated:

URL | HTTP Verb | Functionality
--- | --------- | -----------
`/content/:nid`                 | GET  | [Retrieve a campaign](https://github.com/DoSomething/dosomething/wiki/API#retrieve-a-campaign)
`/reportback_files/:fid/review` | POST | [Review a Reportback File](https://github.com/DoSomething/dosomething/wiki/API#review-a-reportback-file)