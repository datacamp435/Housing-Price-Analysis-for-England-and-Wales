# Problem Description and Details
## Udacity Data Scientist Nanodegree Program: Project 1
### Housing price analysis

In this project, I analyze the housing data from New England and Wales.

HM Land Registry publish the “Price Paid Data”, detailed data on the sale prices of properties in England and Wales. Datasets are published monthly with transaction-level information, including price, date, location, property type, property age, tenure duration, and transaction type. 
Datasets are available in bulk in multiple file formats and filtered via the Linked Data API. Please use whatever source is most appropriate to your analysis, acknowledging it appropriately in your report.

The UK Government's Statistical Datasets are found here:
http://prod.publicdata.landregistry.gov.uk.s3-website-eu-west-1.amazonaws.com/pp-complete.csv
(Contains HM Land Registry data © Crown copyright and database right 2021. This data is licensed under the Open Government Licence v3.0)

It comprehensively covers data from the housing market in England and Wales from 1995 to 2022 and can be used even for commercial analysis.

Dataset Description:

Data item	Explanation (where appropriate)
Transaction unique identifier	A reference number which is generated automatically recording each published sale. The number is unique and will change each time a sale is recorded.
Price	Sale price stated on the transfer deed.
Date of Transfer	Date when the sale was completed, as stated on the transfer deed.
Postcode	This is the postcode used at the time of the original transaction. Note that postcodes can be reallocated and these changes are not reflected in the Price Paid Dataset.
Property Type	D = Detached, S = Semi-Detached, T = Terraced, F = Flats/Maisonettes, O = Other
Note that:
- we only record the above categories to describe property type, we do not separately identify bungalows
- end-of-terrace properties are included in the Terraced category above
- ‘Other’ is only valid where the transaction relates to a property type that is not covered by existing values, for example where a property comprises more than one large parcel of land
Old/New	Indicates the age of the property and applies to all price paid transactions, residential and non-residential.
Y = a newly built property, N = an established residential building
Duration	Relates to the tenure: F = Freehold, L= Leasehold etc.
Note that HM Land Registry does not record leases of 7 years or less in the Price Paid Dataset.
PAON	Primary Addressable Object Name. Typically the house number or name.
SAON	Secondary Addressable Object Name. Where a property has been divided into separate units (for example, flats), the PAON (above) will identify the building and a SAON will be specified that identifies the separate unit/flat.
Street	 
Locality	 
Town/City	 
District	 
County	 
PPD Category Type	Indicates the type of Price Paid transaction.
A = Standard Price Paid entry, includes single residential property sold for value.
B = Additional Price Paid entry including transfers under a power of sale/repossessions, buy-to-lets (where they can be identified by a Mortgage), transfers to non-private individuals and sales where the property type is classed as ‘Other’.

Note that category B does not separately identify the transaction types stated.
HM Land Registry has been collecting information on Category A transactions from January 1995. Category B transactions were identified from October 2013.
Record Status - monthly file only	Indicates additions, changes and deletions to the records.(see guide below).
A = Addition
C = Change
D = Delete

Note that where a transaction changes category type due to misallocation (as above) it will be deleted from the original category type and added to the correct category with a new transaction unique identifier.

In the Jupyter, the data is cleaned and analyzed to answer the following questions:
- What is the most sold property type in England and Wales?
- Which are the most expensive cities?
- Which property type sold most in the top city?
- What were the effects of crises over the years (the Financial Crash of 2008, Brexit, Covid-19, etc.) on the housing market?
- What are the monthly effects of the sales trends over the years?
- What are the effects when we drill down to the counties? How are the total sales? What is the mean?

A Medium blog post with the most important insights can be found here:
https://medium.com/@data.camp435/how-to-analyze-the-housing-market-in-england-and-wales-fbf5fa214db4
