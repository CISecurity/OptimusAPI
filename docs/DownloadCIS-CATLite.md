# Download CIS-CAT Lite (by version)

## Endpoint

```
/cis-cat/lite/{version}

```

## Request Type
GET

## Description
The “CIS-CAT Lite” endpoint allows both members and non-members to obtain any released “lite” version of CIS-CAT.

## Visibility
Public

Request Payload/Parameters
URL Parameter(s)

| Parameter Name      | Description |
| ----------------------|------------ |
| version | The version number identifier for the CIS-CAT Assessor bundle to be downloaded, i.e. “4.1.0”

Example URL:
/cis-cat/lite/4.1.0 |

## Response Payload
### Media Type

```

application/zip

```

The response payload will be the zip bundle representing the requested CIS-CAT Lite release version.