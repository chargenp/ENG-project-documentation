.. warning:: Advanced users only!

**Network Developer Guide**
============================

This guide is for those developers who wish to see the inner workings of the website and contribute to its design. 
Below is information about the login system and the SQL queries used on the website. Also there is a very loose style 
guide for the website and some links to additional helpful information.

**Languages Used**
------------------

Valhalla Billiards uses PHP and embedded HTML.


**Login System**
----------------
	
The current login system uses php session variables to determine if someone is logged into the site.
After a user inputs their login credintials a simple SQL query is used to check if the account exists.

	SQL Query\:

		.. literalinclude:: sqlquery.txt
			:linenos:
			:language: sql
			:lines: 1-21

Using session variables means that every webpage must start with session_start() if the current user account info 
is needed on the page. 

**SQL Queries**
---------------
	
Every query is made using MySQLi's built in functions. More information can be found 
`here <https://www.php.net/manual/en/book.mysqli.php>`_.
		
  
**Contribution**
----------------

If you wish to contribute to the design, go through our GitHub page which can be found 
`here <https://github.com/chargenp/valhalla-billiards-network>`_.


**Troubleshooting**
------------------------

If you are having trouble, or have any questions, go to our :ref:`troubleshooting` page for contact information so that we may assist you further.