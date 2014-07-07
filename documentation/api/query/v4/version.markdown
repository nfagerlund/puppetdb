---
title: "PuppetDB 2.1 » API » v4 » Querying PuppetDB Version"
layout: default
canonical: "/puppetdb/latest/api/query/v4/version.html"
---

[curl]: ../curl.html#using-curl-from-localhost-non-sslhttp

The `/version` endpoint can be used to retrieve version information from the PuppetDB server.

> **Note:** The v4 API is experimental and may change without notice. For stability, we recommend that you use the v3 API instead.

## Routes

### `GET /v4/version`

This query endpoint will return version information about the running PuppetDB
server.

#### Examples

[Using `curl` from localhost][curl]:

    curl -X GET http://localhost:8080/v4/version

    {"version": "X.Y.Z"}

## Response Format

The response will be in `application/json`, and will return a JSON map with a
single key: `version`, whose value is a string representation of the version
of the running PuppetDB server.

    {"version": "X.Y.Z"}
