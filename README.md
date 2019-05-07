# ![LOGO](logo.png) Contribly **flow**ground Connector

## Description

A generated **flow**ground connector for the Contribly API (version 1.0.0).

Generated from: https://api.apis.guru/v2/specs/contribly.com/1.0.0/swagger.json<br/>
Generated at: 2019-05-07T17:40:07+03:00

## API Description



## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Artifact formats

> List the available artifact formats

*Tags:* `info`

### List assignments

*Tags:* `assignment`

#### Input Parameters
* `ownedBy` - _optional_ - Restrict results to assignments owned by this user.
* `page` - _optional_ - Pagination page
* `pageSize` - _optional_ - Pagination page size
* `q` - _optional_ - Restrict results to assignments whose name or description matches this keyword.
* `urlWords` - _optional_ - Select an assignment by urlWords.
* `open` - _optional_ - Select open or closed assignments
* `alwaysOpen` - _optional_ - Select assignments with no closing date.
* `tag` - _optional_ - Restrict results to assignments which are tagged with this tag.
* `name` - _optional_ - Restrict results to the assignment (or potentially assignments) with this exact name

### Create a new assignment

*Tags:* `assignment`

### Delete this assignment and all of it's contributions

*Tags:* `assignment`

#### Input Parameters
* `id` - _required_ - Id of the assignment to return

### Get a single assigment by id

*Tags:* `assignment`

#### Input Parameters
* `id` - _required_ - Id of the assignment to return

### Recent changes

> The Contribly change log.

*Tags:* `info`

### List valid contribution refinement types

*Tags:* `contribution`

### List contribution refinement options

> Given a contribution list query determine the available filter options. Can be used to generate the UI to refinement a filter.

*Tags:* `contribution`

#### Input Parameters
* `assignment` - _optional_ - Restrict results to contributions submitted to this assignment.
* `country` - _optional_ - Limit results to contributions which have a publicly visible location within the given country (specified by two letter country code).
* `createdBefore` - _optional_ - Limit results to contributions created before this date time.
* `createdAfter` - _optional_ - Limit results to contributions created after this date time.
* `geohash` - _optional_ - Restrict results to contributions which have specified a location which falls within this geohash (or comma seperated list of multiple geohashes)
* `hasLocation` - _optional_ - Restrict results to contributions which have a publicly visible location.
* `latLong` - _optional_ - Limit results to contributions with location near this latitude and longitude (comma seperated lat/long pair). Also see radius
* `radius` - _optional_ - When limiting result by location with the latLong parameter, specify the radius in kilometers.
* `mediaType` - _optional_ - Restrict results to contributions which include a media file of the given type (ie. image / video)
* `ownedBy` - _optional_ - Restrict results to contributions which are fall under the jurisdiction by this user.
* `q` - _optional_ - Restrict results to contributions whose headline text matches this keyword.
* `urlWords` - _optional_ - Locate a specific contribution by URL words
* `user` - _optional_ - Restrict results to contributions by this user identified by id.
* `refinements` - _optional_ - Comma seperated list of refinement names.
* `refinementSize` - _optional_ - Number of refinement options to return.

### List contributions

> Retrieve contributions.

*Tags:* `contribution`

#### Input Parameters
* `assignment` - _optional_ - Restrict results to contributions submitted to this assignment.
* `country` - _optional_ - Limit results to contributions which have a publicly visible location within the given country (specified by two letter country code).
* `createdBefore` - _optional_ - Limit results to contributions created before this date time.
* `createdAfter` - _optional_ - Limit results to contributions created after this date time.
* `geohash` - _optional_ - Restrict results to contributions which have specified a location which falls within this geohash (or comma seperated list of multiple geohashes)
* `hasLocation` - _optional_ - Restrict results to contributions which have a publicly visible location.
* `latLong` - _optional_ - Limit results to contributions with location near this latitude and longitude (comma seperated lat/long pair). Also see radius
* `radius` - _optional_ - When limiting result by location with the latLong parameter, specify the radius in kilometers.
* `mediaType` - _optional_ - Restrict results to contributions which include a media file of the given type (ie. image / video)
* `ownedBy` - _optional_ - Restrict results to contributions which are fall under the jurisdiction by this user.
* `q` - _optional_ - Restrict results to contributions whose headline text matches this keyword.
* `urlWords` - _optional_ - Locate a specific contribution by URL words
* `user` - _optional_ - Restrict results to contributions by this user identified by id.
* `ids` - _optional_ - Restrict results to a list of specific contributions identified by a comma seperated list of ids.
* `format` - _optional_ - Select output format. 'json' or 'rss'. Defaults to JSON.

### Create a new contribution

*Tags:* `contribution`

### Delete this contribution

*Tags:* `contribution`

#### Input Parameters
* `id` - _required_ - Id of the contribution to delete

### Get a single contribution by id

*Tags:* `contribution`

#### Input Parameters
* `id` - _required_ - Id of the contribution to return

### Raise a flag against this contribution

> Allows end users to bring potential issues with publicly visible content to the attention of moderators.

*Tags:* `contribution`

#### Input Parameters
* `id` - _required_ - Id of the contribution to flag

### Allows a user to mark a contribution as liked

*Tags:* `contribution`

#### Input Parameters
* `id` - _required_ - Id of the contribution

### List users who have liked this contributions

> Returns a list of user ids of users who have liked this conribution

*Tags:* `contribution`

#### Input Parameters
* `id` - _required_ - Id of the contribution

### Perform a moderation action on this contribution

> Allows the contribution to approved of rejected.

*Tags:* `contribution`

#### Input Parameters
* `id` - _required_ - Id of the contribution to moderate

### List the credentials associated with the authenticated user.

*Tags:* `auth`

### Event types

> List available notification event types

*Tags:* `info`

### Export contributions.

> Begin an export job. Returns a export job which can be polled to follow the progress of an export.

*Tags:* `contribution`

#### Input Parameters
* `assignment` - _optional_ - Restrict results to contributions submitted to this assignment.
* `country` - _optional_ - Limit results to contributions which have a publicly visible location within the given country (specified by two letter country code).
* `createdBefore` - _optional_ - Limit results to contributions created before this date time.
* `createdAfter` - _optional_ - Limit results to contributions created after this date time.
* `geohash` - _optional_ - Restrict results to contributions which have specified a location which falls within this geohash (or comma seperated list of multiple geohashes)
* `hasLocation` - _optional_ - Restrict results to contributions which have a publicly visible location.
* `latLong` - _optional_ - Limit results to contributions with location near this latitude and longitude (comma seperated lat/long pair). Also see radius
* `radius` - _optional_ - When limiting result by location with the latLong parameter, specify the radius in kilometers.
* `mediaType` - _optional_ - Restrict results to contributions which include a media file of the given type (ie. image / video)
* `ownedBy` - _optional_ - Restrict results to contributions which are fall under the jurisdiction by this user.
* `q` - _optional_ - Restrict results to contributions whose headline text matches this keyword.
* `urlWords` - _optional_ - Locate a specific contribution by URL words
* `user` - _optional_ - Restrict results to contributions by this user identified by id.
* `tagged` - _optional_ - Should exported media files be tagged with metadata. Deprecated; use format instead.
* `combined` - _optional_ - Included a combined file with all contribution text.
* `individual` - _optional_ - Include individual text files for each contribution.
* `format` - _optional_ - Media format to export; fullsize, tagged or original.
* `json` - _optional_ - Include raw JSON for each contribution.

### Export contributions preflight summary.

> Provide a preflight summary of an export request.

*Tags:* `contribution`

#### Input Parameters
* `assignment` - _optional_ - Restrict results to contributions submitted to this assignment.
* `country` - _optional_ - Limit results to contributions which have a publicly visible location within the given country (specified by two letter country code).
* `createdBefore` - _optional_ - Limit results to contributions created before this date time.
* `createdAfter` - _optional_ - Limit results to contributions created after this date time.
* `geohash` - _optional_ - Restrict results to contributions which have specified a location which falls within this geohash (or comma seperated list of multiple geohashes)
* `hasLocation` - _optional_ - Restrict results to contributions which have a publicly visible location.
* `latLong` - _optional_ - Limit results to contributions with location near this latitude and longitude (comma seperated lat/long pair). Also see radius
* `radius` - _optional_ - When limiting result by location with the latLong parameter, specify the radius in kilometers.
* `mediaType` - _optional_ - Restrict results to contributions which include a media file of the given type (ie. image / video)
* `ownedBy` - _optional_ - Restrict results to contributions which are fall under the jurisdiction by this user.
* `q` - _optional_ - Restrict results to contributions whose headline text matches this keyword.
* `urlWords` - _optional_ - Locate a specific contribution by URL words
* `user` - _optional_ - Restrict results to contributions by this user identified by id.

### Get a single export job; poll to follow export progress.

*Tags:* `contribution`

#### Input Parameters
* `id` - _required_ - Id of the export job to return

### List form responses

*Tags:* `form`

#### Input Parameters
* `user` - _optional_ - Restrict results to responses submitted by this user.
* `form` - _optional_ - Restrict results to responses submitted to this form.
* `contribution` - _optional_ - Restrict results to responses relating to this contribution.

### Submit a response to a form

*Tags:* `form`

### Get a single form response by id

*Tags:* `form`

#### Input Parameters
* `id` - _required_ - Id of the assignment to return

### List forms

*Tags:* `form`

#### Input Parameters
* `ownedBy` - _required_ - Restrict results to forms owned by this user.

### Create a form

*Tags:* `form`

### Delete this form and all of it's responses.

*Tags:* `form`

#### Input Parameters
* `id` - _required_ - Id of the form to delete

### Get a single form by id

*Tags:* `form`

#### Input Parameters
* `id` - _required_ - Id of the form to return

### Submit a new media file

*Tags:* `media`

### get_notifications_contributions__id__preview

*Tags:* `notifications`

#### Input Parameters
* `id` - _required_ - Id of the contribution to preview a notification for
* `message` - _required_ - Type of message to preview.

### Scopes

> List available token scopes

*Tags:* `auth`

### Subscription types

> List available subscription types

*Tags:* `subscriptions`

### List subscriptions for the authorised user.

*Tags:* `subscriptions`

### Delete a subscription.

*Tags:* `subscriptions`

#### Input Parameters
* `id` - _required_ - Id of the subscription to delete

### List tags

> Retrieve tags.

*Tags:* `tag`

#### Input Parameters
* `ownedBy` - _optional_ - Restrict results to those owned by this user.
* `tagSet` - _optional_ - Restrict results to tags belonging to this tag set.
* `urlWords` - _optional_ - Restrict results by urlWords. Should be used with ownedBy when searching for one of your own tags.

### Create a new tag

*Tags:* `tag`

### Retrieve a single tag by id

*Tags:* `tag`

#### Input Parameters
* `id` - _required_ - Id of the tag to return

### List tag sets

> Retrieve tag sets.

*Tags:* `tag`

#### Input Parameters
* `ownedBy` - _optional_ - Restrict results to those owned by this user.
* `urlWords` - _optional_ - Restrict results by urlWords. Should be used with ownedBy when searching for one of your own tag sets.

### Create a new tag set

*Tags:* `tag`

### Retrieve a single tag set by id

*Tags:* `tag`

#### Input Parameters
* `id` - _required_ - Id of the tag set to return

### List users

*Tags:* `user`

#### Input Parameters
* `assignment` - _optional_ - Restrict results to the users who have contributed to this assignment.
* `country` - _optional_ - Restrict results to the users who have submitted a contribution with a public location located within this country.
* `minimumContributions` - _optional_ - Restrict results to the users who have submitted at least this many contributions.
* `linkedProfile` - _optional_ - Restrict results to the users who a linked profile of this type.
* `ownedBy` - _optional_ - Restrict results to the users who are owned by of this owner.
* `submittedBefore` - _optional_ - Limit results to users who have submitted at least one contribution before this date time.
* `submittedAfter` - _optional_ - Limit results to users who have submitted at least one contribution after this date time.
* `username` - _optional_ - Restrict results to the user with this username.

### Retrieve a single user by id

*Tags:* `user`

#### Input Parameters
* `id` - _required_ - Id of the user to return

### Retrieve a users linked profile by type

*Tags:* `user`

#### Input Parameters
* `id` - _required_ - Id of the user to return
* `type` - _required_ - Type of the linked profile to fetch

### Verify token and return details of the owning user

*Tags:* `auth`

## License

**flow**ground :- Telekom iPaaS / contribly-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
