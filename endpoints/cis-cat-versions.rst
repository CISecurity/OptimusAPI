List Available CIS-CAT Versions
=========================================================
This API endpoint responds with the list of currently released and available CIS-CAT versions.  Two lists are provided in the response from this endpoint: A list of available SecureSuite member-only CIS-CAT Pro Assessor versions (indicated as the "full" version), and the list of publicly-available CIS-CAT Lite versions.

.. list-table::
	:header-rows: 1

	* - Request Type 
	  - Visibility
	* - GET
	  - Public

Endpoint
--------

::

	/cis-cat/versions

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


Media Type
^^^^^^^^^^
::

	application/json

Description/Fields
^^^^^^^^^^^^^^^^^^
The response payload is simply a JSON array of strings representing the versions of CIS-CAT available for download.

.. list-table::
	:header-rows: 1

	* - Container
	  - Description
	* - full
	  - A JSON array containing entries which name the member-only versions of CIS-CAT Pro Assessor which are available for download
	* - lite
	  - A JSON array containing entries which name the lite (publicly available) versions of CIS-CAT available for download

.. list-table::
	:header-rows: 1

	* - Field 
	  - Description
	* - name
	  - The name of the CIS-CAT release
	* - path
	  - The path, relative to the base URL (https://sbp-api.cisecurity.org) which can be used to download the specific version

Response Example
^^^^^^^^^^^^^^^^

:: json

	{
	  "full": [
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
	      "name": "CIS-CAT Lite Assessor v4.3.0",
	      "path": "/cis-cat/lite/4.3.0"
	    },
	    {
	      "name": "CIS-CAT Lite Assessor v4.4.0",
	      "path": "/cis-cat/lite/4.4.0"
	    }
	  ]
	}


.. history
.. authors
.. license