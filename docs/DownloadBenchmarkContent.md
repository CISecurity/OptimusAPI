# Download Benchmark Content

## Description
This API endpoint allows for the retrieval and download of benchmark content.  When an active, valid member utilizes a Bearer Token for authorization to this endpoint, any content formats are allowed to be obtained.  If the member fails to provide a valid token, an error will be returned.  A token will need to be provided/generated for testing purposes.

* 301 Response code for successful retrievals 
* 404 Response code for Content not found 
* 400 Response code for an invalid workbenchId or format
* 500 Response code for internal server error.

## Visibility
SecureSuite Members Only

## Endpoint

```
/{workbenchId}/{format}
```

## Request Type
GET

## Request Payload/Parameters
### Request Header(s)

In order to provide download authorization, members must first authenticate their license key using the /license endpoint, described at API: SecureSuite Member License Verification .  The response from that endpoint is a token.

| Header Name           | Description |
| ----------------------|------------ |
| X-SecureSuite-Token | This header value is required for member-only requests and contains the valid SecureSuite token received as the response when invoking the /license endpoint. |

### URL Parameters

| URL Parameter         | Description |
| ----------------------|------------ |
| workbenchId | The unique identifier for a specific benchmark as stored in CIS WorkBench. |
| format | The format of the content being requested; One of:
* scap: A zip bundle containing XCCDF, OVAL, CPE-Dictionary, and CPE-OVAL
* json
* yaml
* xccdf+ae
(Future Enhancement):
* pdf
* word
* excel |

## Response Payload
### Media Type

```
application/zip
```

## Description/Fields
The response payload will contain a zip bundle downloading the requested format, or all formats. 

 