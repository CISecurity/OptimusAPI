Download Benchmark
==================
This API endpoint allows for the retrieval and download of Build Kit content in a given serialization.

.. list-table::
	:header-rows: 1

	* - Request Type
	  - Visibility
	* - GET
	  - SecureSuite Members Only

Endpoint
--------

::

	/buildkit/{workbenchId}/{format}

Request Payload/Parameters
--------------------------
In order to provide download authorization, members must first authenticate their license key using the :code:`/license` endpoint.  The response from that endpoint is an authorization token.


Request Headers
^^^^^^^^^^^^^^^
.. list-table::
	:header-rows: 1

	* - Header Name
	  - Description
	* - X-SecureSuite-Token
	  - The token received from a successful license key verification, e.g., :code:`7b68c544113bc43458f747ebff4f2bb61358ffd4ba7f254e39c4a842cefed748`

URL Parameters
^^^^^^^^^^^^^^
.. list-table::
	:header-rows: 1

	* - URL Parameter
	  - Description
	* - workbenchId
	  - The unique identifier for a specific benchmark as stored in CIS WorkBench.
	* - format
	  - The format of the content being requested; one of: "JSON", "SCAP", "YAML", "XCCDFPLUSAE", or "DATASTREAM"

Response Payload
----------------


Media Type
^^^^^^^^^^

::

	/application/zip


Description/Fields
^^^^^^^^^^^^^^^^^^
The response payload will contain a zip bundle encapsulating the benchmark content in the requested format.

Response Example
^^^^^^^^^^^^^^^^
N/A



.. history
.. authors
.. license