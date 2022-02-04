Download CIS-CAT Lite
=========================================================
The “CIS-CAT Lite” endpoint allows both members and non-members to obtain any released “lite” version of CIS-CAT.

.. list-table::
	:header-rows: 1

	* - Request Type 
	  - Visibility
	* - GET
	  - Public

Endpoint
--------

::

	/cis-cat/lite/{version}

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
	* - version
	  - The version number identifier for the CIS-CAT Lite Assessor bundle to be downloaded, e.g. “4.1.0”

Response Payload
----------------


Media Type
^^^^^^^^^^

::

	/application/zip


Description/Fields
^^^^^^^^^^^^^^^^^^
The response payload will be the zip bundle representing the requested CIS-CAT Lite Assessor release version.

Response Example
^^^^^^^^^^^^^^^^
N/A

.. history
.. authors
.. license