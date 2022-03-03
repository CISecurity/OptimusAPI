List Available Build Kits
=========================
Publicly available, a request to this endpoint returns a JSON array of basic information for every published build kit that is currently tracked by this API.

.. list-table::
	:header-rows: 1

	* - Request Type
	  - Visibility
	* - GET
	  - Public

Endpoint
--------

::

	/buildkits

Request Payload/Parameters
--------------------------
None

Request Headers
^^^^^^^^^^^^^^^
None

URL Parameters
^^^^^^^^^^^^^^
None

Response Payload
----------------
The response payload is a JSON array of objects noting basic information about all build kits, such as an ID, Benchmark Title, and Build Kit Title.

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
	  - The unique identifier for a benchmark per CIS WorkBench.  This ID can be used in subsequent requests to retrieve metadata or download benchmark content.
	* - buildKitTitle
	  - The title of the published build kit, e.g "CIS_Microsoft_Windows_Server_2012_Benchmark_v1.0.0.zip".
	* - benchmarkTitle
	  - The title of the published benchmark, e.g. "CIS Microsoft Windows 10 Enterprise Release 2004 Benchmark"
	* - buildKit
	  - The filename of the published build kit, e.g "CIS_Microsoft_Windows_Server_2012_Benchmark_v1.0.0.zip".

Response Example
^^^^^^^^^^^^^^^^

::

  {
	[
      {
        "workbenchId": "51",
        "buildKitTitle": "CIS_Microsoft_Windows_Server_2012_Benchmark_v1.0.0.zip",
        "benchmarkTitle": "CIS Microsoft Windows Server 2012 Benchmark [imported]",
        "buildKit": "CIS_Microsoft_Windows_Server_2012_Benchmark_v1.0.0.zip"
      },
      {
        "workbenchId": "55",
        "buildKitTitle": "CIS_Microsoft_Windows_Server_2008_R2_Remediation_Kit.zip",
        "benchmarkTitle": "CIS Microsoft Windows Server 2008 R2 [imported]",
        "buildKit": "CIS_Microsoft_Windows_Server_2008_R2_Remediation_Kit.zip"
      }
    ]
  }


.. history
.. authors
.. license