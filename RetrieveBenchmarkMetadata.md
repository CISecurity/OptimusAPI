# TBD: Retrieve Benchmark Metadata

## Endpoint

```

/benchmarks/{workbenchId}

```

## Request Type
GET

## Description
Requesting information from this API endpoint will retrieve the set of metadata for the requested benchmark, as noted by its workbenchId, determined from the output of the /benchmarks endpoint.

## Visibility
Public

## Request Payload/Parameters
URL Parameters

Parameter Name

Description

workbenchId

The unique identifier for a specific benchmark as stored in CIS WorkBench.

Response Payload
Media Type
application/json

Description/Fields
TBD

Response Element

Description

workbenchId

Unique identifier for a benchmark as stored in CIS WorkBench. This ID can be used in subsequent requests to retrieve metadata or download benchmark content.

benchmarkId

The XCCDF identifier for the benchmark.

benchmarkTitle

The title of the published benchmark

benchmarkVersion

The release version of the published benchmark, i.e. “1.3.0”

benchmarkStatus

The current benchmark status value and date it was applied:

statusDate: The date the benchmark status took effect, formatted as MM-DD-YYYY

status: The status of this benchmark; one of accepted, deprecated, draft, incomplete, or interim.

availableFormats

A JSON array containing the available download formats, such as JSON, SCAP, YAML, XCCDF+AE, Word, PDF, and/or Excel.

profiles

A JSON array containing information about the profiles named in the benchmark. 

profileId: The XCCDF identifier for the profile

profileTitle: The title of the Profile

platformId

A common platform enumeration (CPE) name.

assets

A JSON array containing a list of applicable assets, expressed as CPE names, to which the benchmark is applicable.  A single entry in the array may be configured as the “primary” asset.

assetName: A human-readable name for the asset

assetCpe: The common platform enumeration (CPE) name for the asset

primary: (boolean) An indicator of whether this asset is considered the primary asset identifier.

benchmarkUrl

The location in CIS WorkBench, to find this benchmark.

ciscat

Indicates whether supported content exists in CIS-CAT versions:

v3: (boolean) Indicates content supported in latest CIS-CAT Pro Assessor v3

v4: (boolean) Indicates content supported in latest CIS-CAT Pro Assessor v4

lite: (boolean) Indicates content is included in the latest CIS-CAT Lite.

Example

{
  "workbenchId": "1422", 
  "benchmarkId": "xccdf_org.cisecurity.benchmarks_benchmark_1.9.1_CIS_Microsoft_Windows_10_Enterprise_Release_2004_Benchmark", 
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
  ], 
  "profiles": [
    {
      "profileId": "xccdf_org.cisecurity.benchmarks_profile_Level_1_L1_-_CorporateEnterprise_Environment_general_use", 
      "profileTitle": "Level 1 (L1) - Corporate/Enterprise Environment (general use)"
    }, 
    {
      "profileId": "xccdf_org.cisecurity.benchmarks_profile_Level_1_L1__BitLocker_BL", 
      "profileTitle": "Level 1 (L1) + BitLocker (BL)"
    }
  ], 
  "platformId": "cpe:/o:microsoft:windows_10", 
  "assets": [
    {
      "assetName": "Microsoft Windows 10", 
      "assetCpe": "cpe:/o:microsoft:windows_10", 
      "primary": "true"
    }
  ], 
  "benchmarkUrl": "https://workbench.cisecurity.org/benchmarks/1422", 
  "ciscat": {
    "v3": "false", 
    "v4": "true", 
    "lite": "true"
  }
}
 