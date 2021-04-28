# Download CIS-CAT Full (by version)

## Endpoint

```

/cis-cat/full/{version}

```

## Request Type
GET

## Description
The “CIS-CAT Full” endpoint allows SecureSuite members to obtain any released “full” version of CIS-CAT.  Members are first required to provide their license key to the /license endpoint in order to obtain the necessary token for download authorization.

## Visibility
SecureSuite Members Only

## Request Payload/Parameters
### Headers
In order to provide download authorization, members must first authenticate their license key using the /license endpoint, described at API: SecureSuite Member License Verification .  The response from that endpoint is a token.

| Header Name           | Description |
| ----------------------|------------ |
| X-SecureSuite-Token | The token received from a successful license key verification, ie 7b68c544503bc43458f747ebff4f2bb61358ff74bb7f254e39c4a842cefed748 |

## URL Parameter(s)

| Parameter Name      | Description |
| ----------------------|------------ |
| version | The version number identifier for the CIS-CAT Assessor bundle to be downloaded, i.e. “4.1.0” 

Example URL:
/cis-cat/full/4.1.0 |

## Response Payload
### Media Type

```

application/zip

```

The response payload will be the zip bundle representing the requested CIS-CAT Pro Assessor release version.