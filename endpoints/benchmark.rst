List Available Benchmarks
=========================================================
Publicly available, a request to this endpoint returns a JSON array of basic information for a specific published benchmark that is currently tracked by this API.
Basic information includes Benchmark assessment status (``Manual`` or ``Automated``).

``Manual`` status indicates a prose only Benchmark that does not contain Artifacts. Only intermediate formats (JSON, YAML and XCCDF+AE) are available for ``Manual`` status Benchmarks.

``Automated`` status indicates a Benchmark that contains at least one Artifact. Intermediate formats (JSON, YAML and XCCDF+AE), SCAP and DATASTREAM are available for ``Automated`` status Benchmarks.

.. list-table::
	:header-rows: 1

	* - Request Type 
	  - Visibility
	* - GET
	  - Public

Base URL
--------

::

	https://workbench.cisecurity.org/api/vendor/v1

Endpoint
--------

::

	/benchmarks/{workbenchId}

Request Payload/Parameters
--------------------------

Request Headers
^^^^^^^^^^^^^^^
None

URL Parameters
^^^^^^^^^^^^^^
.. list-table::
	:header-rows: 1

	* - URL Parameter
	  - Description
	* - workbenchId
	  - The unique identifier for a specific Build Kit as stored in CIS WorkBench.

Response Payload
----------------
The response payload is a JSON array of objects noting basic information about this benchmark, such as an ID, Title, Version, and Publication Date.

Media Type
^^^^^^^^^^
::

	application/json

Description/Fields
^^^^^^^^^^^^^^^^^^
.. list-table::
	:header-rows: 1

	* - Response Element 
	  - Description
	* - workbenchId
	  - The unique identifier for a benchmark per CIS WorkBench.  This ID can be used in subsequent requests to download benchmark content.
	* - benchmarkTitle
	  - The title of the published benchmark, e.g. "CIS Microsoft Windows 10 Enterprise Release 2004 Benchmark".
	* - benchmarkVersion
	  - The release version of the published benchmark, e.g. “1.3.0”.
	* - benchmarkStatus
	  - The current benchmark status value and date it was applied.
	* - assessmentStatus
	  - The benchmark assessment status value. Indicates whether the benchmark is Manual or Automated.
	* - availableFormats
	  - A JSON array containing the available download formats, such as "SCAP", "YAML", "JSON", "XCCDFPLUSAE", and/or "DATASTREAM".
	* - profile
	  - The available profile(s) for any given benchmark.
	* - platformId
	  - The primary Common Platform Enumeration (CPE) for a given benchmark.
	* - assets
	  - All assets relevant for a given benchmark including the assetName and  assetCpe (asset specific Common Platform Enumeration (CPE)).
	* - benchmarkUrl
	  - The path to the benchmark in WorkBench.
	* - ciscat
	  - If the benchmark is supported for use with CIS-CAT Pro Assessor and the metadata is available, the applicable versions are listed here.

Response Example
^^^^^^^^^^^^^^^^

::

{
    "workbenchId": "1234",
    "benchmarkId": "xccdf_org.cisecurity.benchmarks_benchmark_1.0.0_CIS_Microsoft_Windows_Server_2012_Benchmark",
    "benchmarkTitle": "CIS Microsoft Windows Server 2012 Benchmark",
    "benchmarkVersion": "1.0.0",
    "benchmarkStatus": {
        "status": "accepted",
        "statusDate": "02/22/2013"
    },
    "assessmentStatus": "Manual",
    "availableFormats": [
        "XCCDF+AE",
        "JSON",
        "YAML"
    ],
    "profiles": [
        {
            "profileId": "xccdf_org.cisecurity.benchmarks_profile_Level_1_-_Domain_Controller",
            "profileTitle": "Level 1 - Domain Controller"
        },
        {
            "profileId": "xccdf_org.cisecurity.benchmarks_profile_Level_1_-_Member_Server",
            "profileTitle": "Level 1 - Member Server"
        }
    ],
    "platformId": "cpe:/o:microsoft:windows_server_2012",
    "assets": [
        {
            "assetName": "Microsoft Windows Server 2012",
            "assetCpe": "cpe:/o:microsoft:windows_server_2012",
            "primary": "true"
        }
    ],
    "benchmarksUrl": "https://workbench.cisecurity.org/benchmarks/1234",
    "ciscat": {
        "ciscatPro": {
            "proAssessmentStatus": "",
            "proVersions": [

            ]
        },
        "ciscatLite": {
            "liteAssessmentStatus": "",
            "liteVersions": [

            ]
        }
    }
}


.. history
.. authors
.. license
