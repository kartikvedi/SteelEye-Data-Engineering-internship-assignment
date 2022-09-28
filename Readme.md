# Python Engineer Assessment

<hr>

### <b>Brief:</b>

- The requirement needs to be developed in Python 3
- Code should follow pep8 standards and should include pydoc, logging & unit tests
- Please provide github link for review.

<hr>

### <b>Requirement:</b>

1. Download the xml from this [link][link]
2. From the xml, please parse through to the first download link whose file_type is <i>DLTINS</i> and download the zip
3. Extract the xml from the zip.
4. Convert the contents of the xml into a CSV with the following header:
	- FinInstrmGnlAttrbts.Id
	- FinInstrmGnlAttrbts.FullNm
	- FinInstrmGnlAttrbts.ClssfctnTp
	- FinInstrmGnlAttrbts.CmmdtyDerivInd
	- FinInstrmGnlAttrbts.NtnlCcy
	- Issr
5. Store the csv from step 4) in an AWS S3 bucket
6. The above function should be run as an AWS Lambda (Optional)

<hr>

## <p align="center">Step-by-Step Outputs</p>

* <b> Step-1: Download the XML file from the link </b>

<img src="https://user-images.githubusercontent.com/70031291/192754334-43a3cac8-ab33-4190-a01f-3bfb1c53c4fe.png">

* <b> Step-2: parse through xml to the first download link whose file_type is <i>DLTINS</i> and download the zip </b>

<img src="https://user-images.githubusercontent.com/70031291/192755978-0be3d645-2202-4dab-84b3-375337af1caa.png">

* <b> Step-3: Extract the xml from the zip. </b>

<img src="https://user-images.githubusercontent.com/70031291/192756791-57767f09-6896-4521-b656-7a26948e8f4a.png">

* <b> Step-4: Convert the contents of the xml into a CSV with the following header: </b>

<img src="https://user-images.githubusercontent.com/70031291/192757389-2e1af5c7-c1cd-41aa-ace8-8140f82fc52c.png">

csv file created

<img src="https://user-images.githubusercontent.com/70031291/192757677-859375ee-b06f-4dc1-bde7-c66986719602.png">

* <b> Step-5: Store the csv from step 4) in an AWS S3 bucket </b>

<img src="https://user-images.githubusercontent.com/70031291/192757977-1a2ce9ff-2584-45ed-b92d-f045db26e78c.png">






[link]: https://registers.esma.europa.eu/solr/esma_registers_firds_files/select?q=*&fq=publication_date:%5B2021-01-17T00:00:00Z+TO+2021-01-19T23:59:59Z%5D&wt=xml&indent=true&start=0&rows=100
