# Guild
Discend Guild's (sometimes called Servers) are communities of members, channels, roles, bots, etc.
They are an essential part of Discend's core features and are implemented into the bulk of our features.


## Guild Object

| name                                | type              | description                                           |
| ----------------------------------- | ----------------- | ----------------------------------------------------- |
| id                                  | snowflake         | unique snowflake id                                   |
| name                                | string            | guild name                                            |
| icon                                | ?string           | icon id                                               |
| splash                              | ?string           | splash id                                             |
| discovery_splash?                   | ?string           | discovery splash id                                   |
| owner_id                            | snowflake         | user id of guild owner                                |
| default_permissions?                | string/integer    | @everyone permission bitset                           |
| afk_channel_id?                     | ?snowflake        | channel id where afk members go                       |
| afk_timeout?                        | integer           | timeout needed to pass for afk members to be moved    |
| default_message_notification_level? | integer           | message notification level integer                    |
| explicit_content_filter?            | integer           | explicit content filter integer                       |
| mfa_level?                          | integer           | MFA Level for moderators                              |
| system_channel_id?                  | ?snowflake        | the moderator announcement channel                    |
| system_channel_flags?               | ?integer          | the system channels flags                             |
| rules_channel_id?                   | ?snowflake        | the rules channel this guild set                      |
| max_presences?                      | ?integer          | the maximum number of presences this guild can hold   |
| max_members?                        | integer           | the maximum number of members this guild can hold     |
| vanity_url_code                     | string            | this guild's vanity url                               |
| description                         | ?string           | the guild description                                 |
| banner                              | ?string           | the guild banner                                      |
| preferred_locale?                   | string            | owner's locale or guild set locale                    |
| guild_updates_channel?              | ?snowflake        | guild's feature updates channel                       |
| nsfw_level                          | integer           | NSFW enumeration level                                |
| verification_level                  | integer           | member join verification level                        |


## Level Enumerations

### Notification Levels

| name      | number |
| --------- | ------ |
| ALL       | 0      |
| MENTIONS  | 1      |

### Content Filter Levels

| name                  | numbers |
| --------------------- | ------- |
| DISABLED              | 0       |
| MEMBERS_WITHOUT_ROLES | 1       |
| ALL                   | 2       |

### Verification Levels

| name                  | numbers |
| --------------------- | ------- |
| NONE                  | 0       |
| LOW                   | 1       |
| MEDIUM                | 2       |
| HIGH                  | 3       |
| VERY_HIGH             | 4       |

### NSFW Levels

| name                  | numbers |
| --------------------- | ------- |
| UNKNOWN               | 0       |
| SAFE                  | 1       |
| EXPLICIT              | 2       |
| AGE_RESTRICTED        | 3       |

### MFA Levels

| name                  | numbers |
| --------------------- | ------- |
| NONE                  | 0       |
| ELEVATED              | 1       |

