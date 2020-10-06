# [BudgetTracker](https://lit-beach-20526.herokuapp.com/)
## [GitHub](https://github.com/dylandewey/BudgetTracker.git)
This app enables a user to create and track purchases (withdrawals) and deposits. It updates the balance in the account to refelct the newly added deposit or withdrawal and adds a line for each new entry.  
This app uses MongoDB for the database to store the information for the budget on the backend. A serviceworker file is used so the app can be used when offline.  When the app comes back online it updates and adds the new lines that were added when offline.  The service worker caches files so it can work offline.  At first I had the service worker caching the index.html file.  In that file I had one of my script tags closed to early.  Because this file was being cached, even when I made the correction to the bug it still wouldn't work properly.  I had to clear the cache, make the change, and take the index.html out of the 'files to cache' in the service worker file.  After I figured that out (with my tutor) everything worked as expected.  

####Demo

