---
slug: /
sidebar_position: 1
---

# Introduction
Welcome to the official API documentation for Discend.

## Official Instances
Discend's Official instance for the api is `https://derailed.one/api` and eventually `wss://gateway.derailed.one` for the gateway.

## Security and Encryption
Discend's Official Services, like our Gateway, API, App, etc. require you to use TLS 1.2.


## Type Structures
In certain objects, you might find symbols before or after a type, this is the index for them:

| symbol        | description                                         |
| ------------- | --------------------------------------------------- |
| ?string       | Specifies this string is nullable                   |
| field?        | Specifies this field can be exempt from the object  |
| ?timestamp    | Specifies this timestamp is nullable                |

## Snowflake IDs
Discend uses twitter's snowflake id algorithm to generate all of its IDs,
since snowflake ids are big integers they are converted from integers (python representation) to strings.

For languages which can handle big integers, you should convert snowflake strings to them.

For more detail on what snowflakes are, we recommend looking at the [Discord Documentation](https://discord.com/developers/docs/reference#snowflakes-snowflake-id-broken-down-in-binary).


### Snowflake Epoch
Discend's Snowflake Epoch is `1641042000000`, or the first second of 2022.
