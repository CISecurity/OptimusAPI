Help
====

Available Endpoints
-------------------

Review the left-hand navigation for technical documentation on each individual API Endpoint

Available Downloads
-------------------

Benchmarks
^^^^^^^^^^

Developed by a global community of cybersecurity professionals, CIS Benchmarks are a collection of best practices for securely configuring IT systems, software, networks, and cloud infrastructure

CIS offers programmatic access to Benchmark export files via the SecureSuite API

**What files are available?**

*PDF* (Benchmarks in a human readable format)

`See Download PDFs page <https://optimusapi.readthedocs.io/en/stable/endpoints/download-pdf/>`_

*SCAP* (Only available for Benchmarks that include automated assessment content)

#. SCAP XCCDF + OVAL (.zip) - SCAP bundle including XCCDF, OVAL, CPE, SCE and DataStreams
#. DataStream (.xml) - SCAP standard collection format

*Intermediate Formats* (Benchmark data in a machine readable format intended to be more easily converted than SCAP)

#. XCCDF+AE Intermediate Format (.xml) – XCCDF, including any available Artifact Expressions (AE)
#. YAML (.yaml)  -  XCCDF+AE in YAML format
#. JSON (.json)  -  XCCDF+AE in JSON format

`See Download Benchmarks Content page <https://optimusapi.readthedocs.io/en/stable/endpoints/download-benchmark/>`_

**What files are included in the SCAP bundle?**

**XCCDF.xml** - The XCCDF acronym stands for Extensible Configuration Checklist Description Format. As the name suggests, the language is used to describe security checklists. These files contain benchmark recommendations

**OVAL.xml** - The OVAL acronym stands for Open Vulnerability and Assessment Language. OVAL is declarative language for making logical assertions about the state of system. These files work in conjunction with the xccdf.xml to help define what is collected from the system using standard OVAL.

**CPE-OVAL.xml** and CPE-DICTIONARY.xml - The Common Platform Enumeration (CPE) serves to identify IT platforms and systems using unequivocally defined names. These files exist for only specific platform benchmarks and they help the assessment tool check if the target platform is right for the benchmark. If it isn't, the assessment may give a warning or produce no results.

**SCE** - The Script Check Engine: SCAP extension to allow script execution from SCAP policy. It allows you to make your scripts interoperable with your security policy. This directory exists only if a specific benchmark references attached scripts. The referenced scripts are included in your export.

**COLLECTION.xml** – This is a DataStream file and it is a format that packs these other SCAP components, above, into a single file. Think, XCCDF, OVAL, CPE and SCE all in one place.

`See SCAP website components page <https://www.open-scap.org/features/scap-components/>`_

CIS-CAT Pro Assessor
^^^^^^^^^^^^^^^^^^^^

CIS-CAT Pro Assessor is a Java-based tool that scans against a target system's configuration settings and reports the system's compliance to the corresponding CIS Benchmark.

CIS-CAT Pro Assessor typically scans in just a few minutes, saving users hours of tedious manual configuration review.

Both CIS-CAT Pro and CIS-CAT Lite are available programmatically via the API

`See Download CIS-CAT Pro Assessor page <https://optimusapi.readthedocs.io/en/stable/endpoints/cis-cat-pro/>`_

`See Download CIS-CAT Lite page <https://optimusapi.readthedocs.io/en/stable/endpoints/cis-cat-lite/>`_

Remediation Kits
^^^^^^^^^^^^^^^^

CIS offers Build Kits for certain technologies to assist with remediation and assist in the automation of hardening systems.

For a subset of Benchmarks, you can download CIS Build Kits programmatically from the API

`See Download Build Kits page <https://optimusapi.readthedocs.io/en/stable/endpoints/download-buildkit/>`_

Download Availability
---------------------

All resources available from the API are made available as soon as they are released

Contact Us
----------

Join the `CIS Members : SecureSuite-API Discussions Community on WorkBench
<https://workbench.cisecurity.org/communities/152>`_.

This community is a place to seek guidance, share experience or information
between users. If you need further assistance, follow the link to the
`Support Portal <https://www.cisecurity.org/support>`_.