API Token Validation
=========================================================
This endpoint allows checking the validation of a token without accessing any data on the server

.. list-table::
	:header-rows: 1

	* - **Request Type**
	  - **Visibility**
	* - GET
	  - SecureSuite Members Only

Base URL
--------

::

	https://workbench.cisecurity.org/api/vendor/v1

Endpoint
--------

::

	/token/check

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
None

Response Payload
----------------
The response from the license verification endpoint will, upon successful verification, provide the receiver with an authorization token that can be used in subsequent member-only requests.

Media Type
^^^^^^^^^^
::

	application/json

Description/Fields
^^^^^^^^^^^^^^^^^^
.. list-table::

	* - **Field**
	  - **Description**
	* - Status
	  - Token Validation Check Successful

.. list-table::

	* - **Field**
	  - **Description**
	* - Error
	  - Invalid or expired security token.

Response Example
^^^^^^^^^^^^^^^^
::

	{
		"status": "Token Validation Check Successful."
	}

::
	{
		"error": "Invalid or expired security token."
	}

.. history
.. authors
.. license
