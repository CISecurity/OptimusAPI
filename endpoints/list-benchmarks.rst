List Available Benchmarks
=========================================================
Publicly available, a request to this endpoint returns a JSON array of basic information for every published benchmark that is currently tracked by this API.

.. list-table::
	:header-rows: 1

	* - Request Type 
	  - Visibility
	* - GET
	  - Public

Endpoint
--------

.. code-block::

	/benchmarks

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
The response payload is a JSON array of objects noting basic information about all benchmarks, such as an ID, Title, Version, and Publication Date.

Media Type
^^^^^^^^^^
.. code-block::

	application/json

Description/Fields
^^^^^^^^^^^^^^^^^^
.. list-table::
	:header-rows: 1

	* - Response Element 
	  - Description
	* - workbenchId
	  - The unique identifier for a benchmark per CIS WorkBench.  This ID can be used in subsequent requests to retrieve metadata or download benchmark content.
	* - benchmarkTitle
	  - The title of the published benchmark, e.g. "CIS Microsoft Windows 10 Enterprise Release 2004 Benchmark"
	* - benchmarkVersion
	  - The release version of the published benchmark, e.g. “1.3.0”
	* - benchmarkStatus
	  - The current benchmark status value and date it was applied
	* - availableFormats
	  - A JSON array containing the available download formats, such as "JSON","SCAP", "YAML", "XCCDF+AE", and/or "DATASTREAM"

Response Example
^^^^^^^^^^^^^^^^

::

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


.. history
.. authors
.. license