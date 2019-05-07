# ![LOGO](logo.png) TaskQueue **flow**ground Connector

## Description

A generated **flow**ground connector for the TaskQueue API (version v1beta2).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/taskqueue/v1beta2/swagger.json<br/>
Generated at: 2019-05-07T17:42:03+03:00

## API Description

Accesses a Google App Engine Pull Task Queue over REST.

## Authorization

Supported authorization schemes:
- OAuth2
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Get detailed information about a TaskQueue.

*Tags:* `taskqueues`

#### Input Parameters
* `getStats` - _optional_ - Whether to get stats. Optional.
* `project` - _required_ - The project under which the queue lies.
* `taskqueue` - _required_ - The id of the taskqueue to get the properties of.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### List Tasks in a TaskQueue

*Tags:* `tasks`

#### Input Parameters
* `project` - _required_ - The project under which the queue lies.
* `taskqueue` - _required_ - The id of the taskqueue to list tasks from.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Insert a new task in a TaskQueue

*Tags:* `tasks`

#### Input Parameters
* `project` - _required_ - The project under which the queue lies
* `taskqueue` - _required_ - The taskqueue to insert the task into
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Lease 1 or more tasks from a TaskQueue.

*Tags:* `tasks`

#### Input Parameters
* `groupByTag` - _optional_ - When true, all returned tasks will have the same tag
* `leaseSecs` - _required_ - The lease in seconds.
* `numTasks` - _required_ - The number of tasks to lease.
* `project` - _required_ - The project under which the queue lies.
* `tag` - _optional_ - The tag allowed for tasks in the response. Must only be specified if group_by_tag is true. If group_by_tag is true and tag is not specified the tag will be that of the oldest task by eta, i.e. the first available tag
* `taskqueue` - _required_ - The taskqueue to lease a task from.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Delete a task from a TaskQueue.

*Tags:* `tasks`

#### Input Parameters
* `project` - _required_ - The project under which the queue lies.
* `task` - _required_ - The id of the task to delete.
* `taskqueue` - _required_ - The taskqueue to delete a task from.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Get a particular task from a TaskQueue.

*Tags:* `tasks`

#### Input Parameters
* `project` - _required_ - The project under which the queue lies.
* `task` - _required_ - The task to get properties of.
* `taskqueue` - _required_ - The taskqueue in which the task belongs.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Update tasks that are leased out of a TaskQueue. This method supports patch semantics.

*Tags:* `tasks`

#### Input Parameters
* `newLeaseSeconds` - _required_ - The new lease in seconds.
* `project` - _required_ - The project under which the queue lies.
* `task` - _required_
* `taskqueue` - _required_
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

### Update tasks that are leased out of a TaskQueue.

*Tags:* `tasks`

#### Input Parameters
* `newLeaseSeconds` - _required_ - The new lease in seconds.
* `project` - _required_ - The project under which the queue lies.
* `task` - _required_
* `taskqueue` - _required_
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters. Overrides userIp if both are provided.
* `userIp` - _optional_ - IP address of the site where the request originates. Use this if you want to enforce per-user limits.

## License

**flow**ground :- Telekom iPaaS / googleapis-com-taskqueue-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
