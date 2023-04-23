# Likhitha sree Data-Engineer-Assignment
Requirements:
1) Download the xml from this link
2) From the xml, please parse through to the first download link whose file_type is DLTINS and download the zip
3) Extract the xml from the zip.
4) Convert the contents of the xml into a CSV with the following header:
   FinInstrmGnlAttrbts.Id
   FinInstrmGnlAttrbts.FullNm
   FinInstrmGnlAttrbts.ClssfctnTp
   FinInstrmGnlAttrbts.CmmdtyDerivInd
   FinInstrmGnlAttrbts.NtnlCcy
   Issr
5) Store the csv from step 4) in an AWS S3 bucket
6) The above function should be run as an AWS Lambda(optional)


SOLUTION:

Xml is Downloaded from given link.

From the downloaded xml link, first_type is DLTINS: http://firds.esma.europa.eu/firds/DLTINS_20210117_01of01.zip file is downloaded.

Extract files from zip file which is downloaded. 

Using python code contents in xml  are converted into csv with the required headers and downloaded the final required csv file.

Then in AWS a S3 bucket is created and the final csv file is uploaded in S3 bucket.
