# Vulnerabilities

Uses the NVD (National Vulnerability Database) API to get information about a list of software names CVSS and description of the Vulnerability of the Software.

The script uses an excel workbook to find the column named "Software" and then converts that into a list to itirate over and submit through the API. Once the information is received
it puts it into another list and at the end of the script it puts it into a excel sheet using the Pandas Dataframe.

NOTE:
There is a progress bar to help scale how long when the process will be done. There is a built in 0.6 second wait time within the for loop to prevent overloading the NVD API
