Obtain SecureSuite API License Key
==================================

To unlock full features and content access for SecureSuite Member API, it is
required to download and apply your organization’s SecureSuite license from `CIS WorkBench <https://workbench.cisecurity.org>`_.

Obtain License Files
--------------------
#. Login to CIS WorkBench
#. In the top right, click on your login name
#. Click on your Organization Name
#. Select the “Licenses” tab beneath your organization name on the left side of the screen
#. Click on Download
	#. **NOTE**: Ensure that java script is unblocked on your browser if you do not see that the file has downloaded.
#. Navigate to the downloaded files and extract the contents

Obtain a Bearer Token for Use With the API
------------------------------------------
#. Once you've retrieved your organization's license files, described above, locate the license.xml file. This is your license key
#. Take the full contents of this file and place it into the body of a POST request to the /license API endpoint
#. Save the token returned and use this to authenticate when downloading resources from the API
`Go here for more details on the /license API endpoint <https://optimusapi.readthedocs.io/en/stable/endpoints/license-verification/>`_

License Renewal
---------------
The license file will expire when your SecureSuite Membership expires. Once your SecureSuite Membership renewal has been processed, your
new license file bundle will be available in WorkBench. Download an updated license by following the initial license installation instructions,
replacing the existing license files.