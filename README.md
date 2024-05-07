Name:
-----
IBM Tivoli Netcool Omnibus WebGUI Performance Health Check Evaluation Portal.


Description:
------------
This Web Portal identifies the Key Performance Indicators(KPIs) of existing IBM Tivoli Netcool Omnibus WebGUI deployment, validates the KPI values with the reference baseline values recommended by IBM and generates a Performance Health Check Report.


Usage:
------
To Generate the Performance Health Check Report for IBM Tivoli Netcool Omnibus WebGUI, Obtain the KPI's from the existing installation of WEBGUI by using the script: get_webgui_metrics.pl and upload the output file (generated in the json format) by using the upload option available on the web portal and click on the Submit button.

There is an alternate option to manually enter the values of KPI's obtained from the existing WebGUI Installation and then click on the submit button to generate the Performance Health Check Report.

Refer to the Section "Procedure to run the get_webgui_metrics.pl script" for more details.


Procedure to Run the get_webgui_metrics.pl Script:
--------------------------------------------------
Run the script "get_webgui_metrics.pl" for obtaining the Key Performance Indicators(KPIs) from the existing installation of IBM Tivoli Netcool Omnibus WebGUI.
1. Download the "get_webgui_metrics.pl" script from the location: <>
2. Create a new directory (Ex: mkdir /tmp/ncw_kpis)
3. Copy the "get_webgui_metrics.pl" script to the newly created directory /tmp/ncw_kpis.
4. Run the command given below:
   cd /tmp/ncw_kpis
   perl get_webgui_metrics.pl 
5. The output file webgui_kpi.out is generated in the same directory /tmp/ncw_kpis.
6. Get the webgui_kpi.out file from the server where it was generated and upload it on the WebGUI Health Check Portal to validate & generate the IBM Tivoli Netcool Omnibus WebGUI Performance Health Check Report.
7. Once the Report is generated, It can be downloaded in the pdf format to the local pc.


Limitations:
------------
1. The Script get_webgui_metrics.pl retrieves the Performance KPI's only from the Linux based installation of IBM Tivoli Netcool Omnibus WebGUI.
2. Perl is required to run the script get_webgui_metrics.pl. Perl should be pre-installed on the server where the script get_webgui_metrics.pl is executed.


Scripts Download Location:
--------------------------
https://github.com/GDC-ITAuto/Netcool-WebGUI-Upload

REVISION HISTORY:
-----------------
REVISION 1 :
Date: 15-April-2024, Initial release.


CONTACT:
--------
Author: Karthikeyan P, karpandr@in.ibm.com

