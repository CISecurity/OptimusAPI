Download PDF
==================
This API endpoint allows for the retrieval and download of benchmark content in the PDF format.

.. list-table::
	:header-rows: 1

	* - Request Type
	  - Visibility
	* - GET
	  - Public

Endpoint
--------

::

	/pdf/{workbenchId}

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
	* - workbenchId
	  - The unique identifier for a specific PDF as stored in CIS WorkBench.

Response Payload
----------------


Media Type
^^^^^^^^^^

::

	.pdf


Description/Fields
^^^^^^^^^^^^^^^^^^
The response payload will contain a PDF (.pdf) download.

Response Example
^^^^^^^^^^^^^^^^
None



.. history
.. authors
.. license