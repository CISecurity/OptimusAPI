List Available PDFs
=========================
Publicly available, a request to this endpoint returns a JSON array of basic information for each available PDF file that is currently tracked by this API.

.. list-table::
	:header-rows: 1

	* - Request Type
	  - Visibility
	* - GET
	  - Public

Base URL
--------

::

	https://sbp-api.cisecurity.org

Endpoint
--------

::

	/pdf

Request Payload/Parameters
--------------------------

Request Headers
^^^^^^^^^^^^^^^
None

URL Parameters
^^^^^^^^^^^^^^
None

Response Payload
----------------
The response payload is a JSON array of objects noting basic information about all PDFs, such as an ID, Benchmark Title, and PDF Title.

Media Type
^^^^^^^^^^
::

	application/json

Description/Fields
^^^^^^^^^^^^^^^^^^
.. list-table::
	:header-rows: 1

	* - Response Element
	  - Description
	* - workbenchId
	  - The unique identifier for a PDF per CIS WorkBench.  This ID can be used in subsequent requests to download PDF benchmark content.
	* - pdfTitle
	  - The title of the published PDF, e.g "CIS Red Hat Enterprise Linux 8 Benchmark v2.0.0 - PDF".
	* - benchmarkTitle
	  - The title of the published benchmark, e.g. "CIS Red Hat Enterprise Linux 8 Benchmark v2.0.0".
	* - pdfFileName
	  - The filename of the published PDF, e.g "CIS_Red_Hat_Enterprise_Linux_8_Benchmark_v2.0.0.pdf".

Response Example
^^^^^^^^^^^^^^^^

::

  {
    "Total number of results": 269,
    "PDFs": [
        {
            "workbenchId": "9089",
            "pdfTitle": "CIS CentOS Linux 8 Benchmark v2.0.0 - PDF",
            "benchmarkTitle": "CIS CentOS Linux 8 Benchmark v2.0.0",
            "pdfFileName": "CIS_CentOS_Linux_8_Benchmark_v2.0.0.pdf"
        },
        {
            "workbenchId": "9090",
            "pdfTitle": "CIS Red Hat Enterprise Linux 8 Benchmark v2.0.0 - PDF",
            "benchmarkTitle": "CIS Red Hat Enterprise Linux 8 Benchmark v2.0.0",
            "pdfFileName": "CIS_Red_Hat_Enterprise_Linux_8_Benchmark_v2.0.0.pdf"
        }
    ]
  }


.. history
.. authors
.. license