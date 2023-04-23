
# Globant Challenge

This is the challange for Globant Data Engineer Position.


## Documentation

This challenge was resolved using the following technologies:

* Azure Blob Storage

All files were uploaded in the following container in ADLS2

![App Screenshot](https://github.com/jaimepc/globant-challenge/blob/main/screenshots/adls.png)

* Azure Synapse (SQL Serverless db)

Then all the data was processed using a medallion architecture where all bronze tables are the new data that we fetch daily/weekly etc.

Then it is transformed into silver tables after we do data cleaning and validations. This process can be achieved in ADF but in this challenge that step was skipped.

Finally the data is curated and pushed into the final gold tables that represent the data we need for our reports.

![App Screenshot](https://github.com/jaimepc/globant-challenge/blob/main/screenshots/synapse.png)

* Power BI

In order to present the final reports, the SQL Serverless database was connected to power bi, exported into power bi web site and then published in a custom HTML page located called index.html located at root of this repository

![App Screenshot](https://github.com/jaimepc/globant-challenge/blob/main/screenshots/powerbi.png)

![App Screenshot](https://github.com/jaimepc/globant-challenge/blob/main/screenshots/finalresults.png)

* Github

All code was commited and pushed into this repo, also the pbxi file and some versions were release to highlight the milestones of the project.

## Authors

- [@Jaime Padron](jaimepc199@gmail.com)

