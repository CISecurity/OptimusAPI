Download CIS-CAT Pro Assessor
=========================================================
The “CIS-CAT Pro Assessor” endpoint allows SecureSuite members to obtain any released “full functionality” version of CIS-CAT.

.. list-table::
	:header-rows: 1

	* - Request Type 
	  - Visibility
	* - GET
	  - SecureSuite Members Only

Base URL
--------

::

	https://sbp-api.cisecurity.org

Endpoint
--------

::

	/cis-cat/pro/{version}

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
The response payload will be the zip bundle representing the requested CIS-CAT Pro Assessor release version.

Response Example
^^^^^^^^^^^^^^^^
None


.. history
.. authors
.. license