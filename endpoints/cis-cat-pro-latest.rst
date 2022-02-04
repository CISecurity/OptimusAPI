Download Latest CIS-CAT Pro Assessor
=========================================================
The “CIS-CAT Pro Assessor” endpoint allows SecureSuite members to obtain the latest “full functionality” version of CIS-CAT.

.. list-table::
	:header-rows: 1

	* - Request Type 
	  - Visibility
	* - GET
	  - SecureSuite Members Only

Endpoint
--------

::

	/cis-cat/pro/latest

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
N/A

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
N/A


.. history
.. authors
.. license