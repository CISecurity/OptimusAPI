# List Available Versions

## Description
As the name of this page suggests, this API endpoint responds with the list of currently available CIS-CAT versions.

## Visibility
Public

## Endpoint

```
/cis-cat/versions
```

## Request Type
GET

## Request Payload/Parameters
None

## Response Payload
### Media Type

```
application/json
```

## Description/Fields
The response payload is simply a JSON array of strings representing the versions of CIS-CAT available for download.

| Container/Field       | Description |
| ----------------------|------------ |
| full | A JSON array containing entries which name the full (member-only) versions of CIS-CAT available for download |
| name | The name of the CIS-CAT release |
| path | The path, relative to the base URL (https://sbp-api.cisecurity.org) which can be used to download the specific version |
| lite | A JSON array containing entries which name the lite (publicly available) versions of CIS-CAT available for download |

## Response Example

```
{
  "full": [
    {
      "name": "CIS-CAT Pro Assessor v4.0.0",
      "path": "/cis-cat/full/4.0.0"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.1",
      "path": "/cis-cat/full/4.0.1"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.2",
      "path": "/cis-cat/full/4.0.2"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.3",
      "path": "/cis-cat/full/4.0.3"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.4",
      "path": "/cis-cat/full/4.0.4"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.5",
      "path": "/cis-cat/full/4.0.5"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.10",
      "path": "/cis-cat/full/4.0.10"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.11",
      "path": "/cis-cat/full/4.0.11"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.12",
      "path": "/cis-cat/full/4.0.12"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.13",
      "path": "/cis-cat/full/4.0.13"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.14",
      "path": "/cis-cat/full/4.0.14"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.15",
      "path": "/cis-cat/full/4.0.15"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.16",
      "path": "/cis-cat/full/4.0.16"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.17",
      "path": "/cis-cat/full/4.0.17"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.18",
      "path": "/cis-cat/full/4.0.18"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.19",
      "path": "/cis-cat/full/4.0.19"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.20",
      "path": "/cis-cat/full/4.0.20"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.21",
      "path": "/cis-cat/full/4.0.21"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.22",
      "path": "/cis-cat/full/4.0.22"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.23",
      "path": "/cis-cat/full/4.0.23"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.24",
      "path": "/cis-cat/full/4.0.24"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.6",
      "path": "/cis-cat/full/4.0.6"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.7",
      "path": "/cis-cat/full/4.0.7"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.8",
      "path": "/cis-cat/full/4.0.8"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.0.9",
      "path": "/cis-cat/full/4.0.9"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.1.0",
      "path": "/cis-cat/full/4.1.0"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.2.0",
      "path": "/cis-cat/full/4.2.0"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.3.0",
      "path": "/cis-cat/full/4.3.0"
    },
    {
      "name": "CIS-CAT Pro Assessor v4.4.0",
      "path": "/cis-cat/full/4.4.0"
    }
  ],
  "lite": [
    {
      "name": "CIS-CAT Lite Assessor v4.0.22",
      "path": "/cis-cat/lite/4.0.22"
    },
    {
      "name": "CIS-CAT Lite Assessor v4.0.23",
      "path": "/cis-cat/lite/4.0.23"
    },
    {
      "name": "CIS-CAT Lite Assessor v4.0.24",
      "path": "/cis-cat/lite/4.0.24"
    },
    {
      "name": "CIS-CAT Lite Assessor v4.1.0",
      "path": "/cis-cat/lite/4.1.0"
    },
    {
      "name": "CIS-CAT Lite Assessor v4.2.0",
      "path": "/cis-cat/lite/4.2.0"
    },
    {
      "name": "CIS-CAT Lite Assessor v4.3.0",
      "path": "/cis-cat/lite/4.3.0"
    },
    {
      "name": "CIS-CAT Lite Assessor v4.4.0",
      "path": "/cis-cat/lite/4.4.0"
    }
  ]
}
```
