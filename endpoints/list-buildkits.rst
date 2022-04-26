List Available Build Kits
=========================
Publicly available, a request to this endpoint returns a JSON array of basic information for every published Build Kit that is currently tracked by this API.

.. list-table::
	:header-rows: 1

	* - Request Type
	  - Visibility
	* - GET
	  - Public

Base URL
--------

::

	https://sbp-api.cisecurity.org

Endpoint
--------

::

	/buildkits

Request Payload/Parameters
--------------------------

Request Headers
^^^^^^^^^^^^^^^
None

URL Parameters
^^^^^^^^^^^^^^
None

Response Payload
----------------
The response payload is a JSON array of objects noting basic information about all Build Kits, such as an ID, Benchmark Title, and Build Kit Title.

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
	  - The unique identifier for a Build Kit per CIS WorkBench.  This ID can be used in subsequent requests to download Build Kit content.
	* - buildKitTitle
	  - The title of the published Build Kit, e.g "CIS Microsoft Windows 10 Enterprise Release 1809 Benchmark v1.6.0 - Build Kit".
	* - benchmarkTitle
	  - The title of the published benchmark, e.g. "CIS Microsoft Windows 10 Enterprise Release 1809 Benchmark v1.6.0".
	* - buildKit
	  - The filename of the published Build Kit, e.g "Windows10v1.6.0.zip".

Response Example
^^^^^^^^^^^^^^^^

::

  {
    "Total number of results": 116,
    "Build Kits": [
      {
        "workbenchId": "4177",
        "buildKitTitle": "CIS Microsoft Windows 10 Enterprise Release 1809 Benchmark v1.6.0 - Build Kit",
        "benchmarkTitle": "CIS Microsoft Windows 10 Enterprise Release 1809 Benchmark",
        "buildKit": "Windows10v1.6.0.zip"
      },
      {
        "workbenchId": "4179",
        "buildKitTitle": "CIS Microsoft Windows Server 2019 Benchmark v1.0.0 - Build Kit",
        "benchmarkTitle": "CIS Microsoft Windows Server 2019 Benchmark",
        "buildKit": "Server2019v1.0.0.zip"
      }
    ]
  }


.. history
.. authors
.. license