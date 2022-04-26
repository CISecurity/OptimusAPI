SecureSuite Member License Verification
=========================================================
The body of this POST request includes the SecureSuite member's license key, and the backend function performs verification of the key, returning back to the caller a token (generated based on the license key) for future use. The token will be stored for future authorization purposes and to track a time limit for its usage.

.. list-table::
	:header-rows: 1

	* - **Request Type**
	  - **Visibility**
	* - POST
	  - Public

Base URL
--------

::

	https://sbp-api.cisecurity.org

Endpoint
--------

::

	/license

Request Payload/Parameters
--------------------------

The request body will contain the SecureSuite member license key, in either XML or JSON form.

::

	<securesuite_member_license>
	    <uuid>d2e343b8-ca58-432b-af1d-336ba365ef07</uuid>
	    <license_key>
	        --- START CIS LICENSE KEY ---
	        ABCD123iOiJqd3QiLCJhbGciOiJSUzI1NiJ9.eyJzdWIiOiJDSVMgTElDRU5TRSBLRVkiLCJqdGkiOiJ
	        lZmUzNDNiOC1jYTU4LTQzMmItYWYxZC0zMzZiYTM2NWVmMDciLCJpYXQiOjE1ODEzMTA4MDAsImV4cCI
	        6MTY3NjAwNTIwMCwibmFtZSI6IkNJUyIsImRvbWFpbiI6ImNpc2VjdXJpdHkub3JnIn0.EW1DFihmKx0
	        i8fV_jRrTVhV1nS1YWXfbso_2w8-sL-P6lx4vPIPK220wj7WvX385tIA4fKWxehEi70zVSjUEsTuUO35
	        iCTF8CZsbO7_VpfAvSfF5XjUe30nR7ijp8XXXepeqrmNNuR5HcIn9grW0jVS7osbfINLUsDpnrbKre89
	        nBz2NTDuqFTH2xqrBaBTwBronnTbqorZmExEQgMWUEt7Y8DdprsEw5Ugk0oQ1UT8uaMy-iGJellUS-WB
	        EcOHIg0qO55K8nwU2MFsQtc7Fog_dXqQixA7Slu-4Osa20imlB_3QdK1T221Job_mHXHWaZmxIXyOfcr
	        1HoRMg337pn9tsuQUUNBsfXF75xHBHDOZucaNfCiMSTbyAghOLnknb2nl3P6sukf28l4DJargqo9wMEM
	        hGzOn7_84yrxx_cWoAc5pw24pUzpN20kDr0on2VcIQk3Gb6xke3em9bQpg6TrXLYFp4iJ3tsd6pAardK
	        1y7WAO64JaWhc6eANve36RNqgV8ypDcGJogi88vL61H6E8S258zD5ETPpGO5ApQfHewdxJVGTR_Ql4zj
	        xJlbDTwa7ENWdBe1UKZb-xU75Du_p7PIp6A6upupzuZ73qikLqOnCfn0AWYcFliznMrk6c5q79xWkIaN
	        V4dicTib9ThaQccXl7HxgJiDVs8Ylz7X-kGttAbjsCZBD0PKbQezLZCKxDu5nYnTxRZ9Hv6CE4bySGT6
	        z9HywT58uuLWu4dBc9RDA51zjjgePMDXmQmNFc0yt37ggYfi1cTeg5T6eWGWyqoZh7icfsWO6YFX9v00
	        Wp7Zk-WpliaUTlcNDYUJmf7NXae7yjyspxluBdUBWp3rsiYUfHdzN_jGeiBSP0392xWWIARlluCUxWzh
	        vbvUov-7VjzRgMpife-GNtpe37F9zyu_VMKsB2ljT7eEb8tShwjNgHlyICUaCUqEsjDFPRNQS_nryft2
	        fjox2STZ_Rp20Ju00Wcs0Y_0FMIu4M1Qit37mN8M262wAwXpG0vKkvu0Ws8i_ut-_qcaKw1rkj4I4CFd
	        TihJEnBgq_Ge3IZM5VDcJ53FbgGK9sBGBFX-lV7peNAq7iRWJsJspWrMT6nSQJIiDOdk3-KedwYpve9-
	        MeNFjD4KTM9cFu1GwS7TTBm7fph1Q0k2m2izxBouuG91-11kGT_Q1k-9CB7QzlE8uYmn-yr_jULewmAR
	        -SwPz_mSkkO3DWBFmK7cnIHd_dG0S0eljISLJ5jqSPb3V_Ni8vETDbx2GGKqMrCENtzH7Ck4IT8-Rsgd
	        dABX4UNvGT_zEAoTt9p1OReyOW6MTeqZqQJ6Lv0wgvtzImdHihUCdt9m-wltAw-1DUEFy4BKzdT5ZQMj
	        7h-upGQ4We0szOxIvAHncmV3YBAA-H2g6gy0hFceuCxVyHDuiwkS-IQG9cyx2gFFHaAqvljZ-BHlUoEy
	        2YKWSAfOhu_8ey-oh7J-m4mnfBcem4-X_cYqBGpmtZILZmYmdf1y22Q9gInJ2evvBXOGcIicqvof4KOZ
	        TIlqmhyM9tYNrrNGQv1lOAGWoCKhBga5wvAYU3fabowf-AoUspNXOZZNc6diGP4hYMxLsi5IpXcNiiVR
	        gTIRc3MhaPAgnIXyGyjm4Pc7HV-Fa6H5yTudLvZEhF_AUngQmUPH4UV-PprKkALE7zYRuILHfiAy1JIe
	        wC1e6hjnoQYAMi9vm6y8wevDy47DlGI7zA3k2Xj5pm2xeowLMvaFyN9B3aOE49pS9prsJBX5ISl_siMT
	        vEUSvRI84Btc3q2h5INKDSypqYlj_wSRDyHToqs_vxItd3BD0PG-85ZBYicJBTRmG3yZX7_tgTPkdOYv
	        AqCHRxl_I77hOpmi24MmLmUIANh71D699WmFCvbiHiGe3126BSRmjEMhMOJ4cv3bde8q4__tfWd1f01n
	        BczbZ7gMYXw06jJ59Tjp2w0nQbks7IhQlm6NSX4n-59Gnj40j6KM_jn8M6pLpXgQ1TBRWnoemL-b-N4P
	        wqHcDLF_CxFr99vIsebx7We9KkMLd_AJrmi4N0Yz8mvgbFHiYz-RDHi_B_DAvwW_mE6v9LgHCxVrVJZ9
	        bR60V3IhhqOeHjxrUhKVm-EgDlU4B4pRyhxTKgucJ4ef2FOLBVFiX--YNjqpt4e18e_G4YFgMFTS6vAb
	        WwSlNbE2s4d45aRPhAtKecwuK0mpOs1IEEDVulkPYNbNMx8BkZpDEyc6buX4JS7ikbt7r4apOnbARO06
	        Xlnp08VuXkVGIsRoawRzoJBfHND-cCfqVHlu-ikEZvpBCwQCqYLQ6JrHXpQUjRXup-t_0YNuy8IWjdVi
	        -zCmMYWSpgBBNfyta71kVxa82m7crHShIrkqGjmFYV8KWAbPYouEmiwefw4H36Mc992_sma2OU_tPVCh
	        Yns5xo1_3gI0Q3yKV8S_nGgAbcnsuZnyYpqn04RG8YLpc_SmCZgkA1LEydvEB25wGoeH2tDF--FbH4j3
	        xtWZTyx3xZMllya5v___42BILVYzBSKYebjhPavM4wDEitvUGUHyeB6uVIShdpahJ4uN1L-acxHhMTkD
	        _p7_5C9dmwaS-bMOlssu4AilKPbt9FekCFNIV5IRs-pV35HddrT9M0MzS55sVOpKv32lx6OolHqKgAiS
	        wJokdeJlZVS6qMoQ8Bu8ab47DCNvwvHlJQLaaLlZmL1Wb0DaAYSOZQ7llSWC250QicUW9DgS2gjPvsJ4
	        --- END CIS LICENSE KEY ---
	    </license_key>
	</securesuite_member_license>

Request Headers
^^^^^^^^^^^^^^^
None

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
	* - token
	  - The token that can be utilized in future, authenticated interactions with the API.

Response Example
^^^^^^^^^^^^^^^^
::

	{
		"token": "7b68c544503bc43458f747ebff4f2bb61358ff7f787f254e39c4a842cefed748"
	}


.. history
.. authors
.. license