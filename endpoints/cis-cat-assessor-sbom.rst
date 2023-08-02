Download the CIS-CAT Assessor and Lite SBOM
=========================================================
The “CIS-CAT Assessor SBOM” endpoint allows both members and non-members to obtain the SBOM (Software Bill of Materials) of the latest version of CIS-CAT.

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

	/cis-cat/sbom

Request Payload/Parameters
--------------------------

Request Headers
^^^^^^^^^^^^^^^

URL Parameters
^^^^^^^^^^^^^^

Response Payload
----------------


Media Type
^^^^^^^^^^

::

	/application/zip


Description/Fields
^^^^^^^^^^^^^^^^^^
The response payload will be the zip bundle representing the requested CIS-CAT Assessor SBOM file.

Response Example
^^^^^^^^^^^^^^^^
None

.. history
.. authors
.. license
