Change Log
================================

Review the Change Log below for the latest on the SecureSuite Member API.

August 2023
--------
1. `Endpoint added to download CIS-CAT Assessor SBOM <https://optimusapi.readthedocs.io/en/stable/endpoints/cis-cat-assessor-sbom/>`_

July 2023
--------
1. `Endpoint to check if token is still valid <https://optimusapi.readthedocs.io/en/stable/endpoints/token-validation/>`_
2. `Endpoint to individual benchmark information <https://optimusapi.readthedocs.io/en/stable/endpoints/benchmark/>`_

January 2023
--------
1. Base URL updated to new API location 
2. `API token format and duration updated <https://optimusapi.readthedocs.io/en/stable/endpoints/license-verification/>`_

July 2022
--------
1. Prose Only Benchmarks can be added to the Benchmarks API endpoint for download as an intermediate format
    - Note Prose Only Benchmarks do not contain Artifacts or Automated Assessment Content (AAC).
2. Prose Only Benchmarks are tagged as “Manual” and Benchmarks that contain AAC are marked “Automated”
    - See `List Available Benchmarks Endpoint <https://optimusapi.readthedocs.io/en/stable/endpoints/list-benchmarks/>`_
    - Are you looking for a Prose Only Benchmark that isn't currently listed? `Let us know! <https://www.cisecurity.org/support>`_

May 2022
--------
1. `Help section added <https://optimusapi.readthedocs.io/en/stable/about/help/>`_


April 2022
--------
1. Intermediate Formats, JSON and YAML, now include embedded SCE scripts
    - From the `Download Benchmarks Content endpoint <https://optimusapi.readthedocs.io/en/stable/endpoints/download-benchmark/>`_ you can download YAML or JSON translation of a given Benchmark. They now contain any relevant SCE files at the end of the file. SCE files are also included in SCAP and DATASTREAM download options.


March 2022
--------
1. Endpoint for Build Kits added
    - Upon request to the endpoint, any specified Build Kit can be downloaded directly from the API. The Build Kits included are from the list currently available to download in WorkBench.
    - See 'List Available Build Kits' documentation here: `List Available Build Kits <https://optimusapi.readthedocs.io/en/stable/endpoints/list-buildkits/>`_.
    - See 'Download Build Kits' documentation here: `Download Build Kits <https://optimusapi.readthedocs.io/en/stable/endpoints/download-buildkit/>`_.
    - For more information on Build Kits, go here: `CIS Build Kits FAQ <https://www.cisecurity.org/cis-securesuite/cis-securesuite-build-kit-content/build-kits-faq>`_.
2. Endpoint for PDFs added
    - Upon request to the endpoint, any specified PDF can be downloaded directly from the API. The PDFs included are pulled from WorkBench and those we include correlate with available Benchmarks from the /benchmarks endpoint list.
    - See 'List PDFs' documentation here: `List Available PDFs <https://optimusapi.readthedocs.io/en/stable/endpoints/list-pdf/>`_.
    - See 'Download PDFs' documentation here `Download PDFs <https://optimusapi.readthedocs.io/en/stable/endpoints/download-pdf/>`_.


January 2022
--------
1. SCAP Datastream collection format now available to download from the /benchmarks endpoint
    - See 'Download Benchmark Content' documentation here: `Download Benchmark Content <https://optimusapi.readthedocs.io/en/stable/endpoints/download-benchmark/>`_.

