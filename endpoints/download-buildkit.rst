Download Build Kits
==================
This API endpoint allows SecureSuite members to obtain any released remediation content, also known as CIS Build Kits. For more information on Build Kits, go here: `CIS Build Kits FAQ <https://www.cisecurity.org/cis-securesuite/cis-securesuite-build-kit-content/build-kits-faq>`_.

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

	/buildkits/{workbenchId}

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
	  - The unique identifier for a specific Build Kit as stored in CIS WorkBench.

Response Payload
----------------


Media Type
^^^^^^^^^^

::

	/application/zip


Description/Fields
^^^^^^^^^^^^^^^^^^
The response payload will contain a zip bundle encapsulating the Build Kit content.

Response Example
^^^^^^^^^^^^^^^^
None



.. history
.. authors
.. license