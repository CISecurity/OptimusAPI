# List Available Benchmarks

## Description
Publicly available, a request to this endpoint returns a JSON array of basic information for every published benchmark that is currently tracked by this API.

## Visibility
Public

## Endpoint

```
/benchmarks
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

### Description/Fields
The response payload is a JSON array of objects noting basic information about all benchmarks, such as an ID, Title, Version, and Publication Date.

| Response Element      | Description |
| ----------------------|------------ |
| workbenchId | The unique identifier for a benchmark per CIS WorkBench.  This ID can be used in subsequent requests to retrieve metadata or download benchmark content. |
| benchmarkTitle | The title of the published benchmark |
| benchmarkVersion | The release version of the published benchmark, i.e. “1.3.0” |
| benchmarkStatus | The current benchmark status value and date it was applied: 
* statusDate: The date the benchmark status took effect, formatted as MM-DD-YYYY
* status: The status of this benchmark; one of
  * accepted, 
  * deprecated, 
  * draft, 
  * incomplete, or 
  * interim. |
| availableFormats | A JSON array containing the available download formats, such as JSON, SCAP, YAML, XCCDF+AE, (and down the road: Word, PDF, and/or Excel). |

### Example

``` 
{
  [
    {
      "workbenchId": "1234", 
      "benchmarkTitle": "CIS Microsoft Windows 10 Enterprise Release 2004 Benchmark", 
      "benchmarkVersion": "1.9.1", 
      "benchmarkStatus": {
        "statusDate": "10-20-2020", 
        "status": "accepted"
      }, 
      "availableFormats": [
        "SCAP", 
        "XCCDF+AE", 
        "YAML", 
        "JSON"
      ]
    }, 
    {
      "workbenchId": "2000", 
      "benchmarkTitle": "CIS Apache Tomcat 9 Benchmark", 
      "benchmarkVersion": "1.9.1", 
      "benchmarkStatus": {
        "statusDate": "12-14-2020", 
        "status": "accepted"
      },
      "availableFormats": [
        "SCAP"
      ]
    }
  ]
}
 ```
