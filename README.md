Updated: 02.2025  
Script created by Salvador Camacho

This script was created with best practices, so it is more resilient, such as:
* Transaction naming
* No add cookies
* No third party
* One validation per transaction
* Think times at the end of each transaction to better simulate user behavior
* Main URL parametrized, Nimbus AOS by default: (http://nimbusserver.aos.com:8000), credentials parametrized

This script logs in and then logs out. There are 10 rows in the user data and 2 of them are bad log ins,
so the script is expected to fail 80% of the times, which works well to show error snapshot and detail during the test
	
Runtime Settings were set to log only on errors and generate snapshot on errors, think times 75% to 150%

This script has 3 transactions:  
AOS-Web-S03-01 Access AOS URL  
AOS-Web-S03-02 Sign In  
AOS-Web-S03-03 Sign Out