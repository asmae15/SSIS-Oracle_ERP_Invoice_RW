# README #

This README would normally document whatever steps are necessary to get your application up and running.

### What is this repository for? ###

* The Oracle ERP Invoice RW package extracts invoice data from RentalWorks (RW) and saves the data to an Excel file.  It is scheduled to run daily from TQ9-SQL and 
save the file to the H:\PROJECTS & TEAMS\RW Transition Files\Oracle ERP- Data\SIM Integration Docs\Invoice\Production\RW Production Invoices\Raw Files folder.

* There are two SSIS packages in the project.  The RW_Invoice_ETL extracts the invoices for the Lighting and Grip divisions and the RW_Invoice_Studio_ETL extracts 
the invoices for the Studios division.   

* Version
* [Learn Markdown](https://bitbucket.org/tutorials/markdowndemo)

### How do I get set up? ###


* Configuration
    * The isDev variable controls whether the package is being run for Development or Production.
    * For Development the RootfilePath variable needs to be updated to the new base folder location.  The package is expecting that the Excel template exists in a 
DNT-Template sub-folder from the base folder location and that there is a Raw Files sub-folder to save the generated files into. 
    * The DDvalue and DDEndValue variables set the date range that the extract is for. The DDEndValue is hard-coded to -1 (yesterday). 

* Dependencies
* Database configuration
* How to run tests
* Deployment instructions
 

### Contribution guidelines ###

* Writing tests
* Code review
* Other guidelines

### Who do I talk to? ###

* Repo owner or admin
* Other community or team contact