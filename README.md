# powerBI-FreshService
A template to import data from FreshService into Power BI via API

This is by no means a professionally developed file, but it suits my purposes and may work for others. It is provided 'as is', and I am not in a position to support it I'm afraid. That being said, if people improve it, please share it back! Just be sure to save as a template as this stops your data & credentials going with it.

I have included an allowance to limit the number of tickets retrieved. In practice, this only limits the number of pages requested, users will need to ensure they don't refresh too many times per hour, or try to retrieve too many tickets. Eg to retrieve 5000 tickets will be 50 pages @ 3 API credits per page = 150 credits. Thus an entry level plan (Sprout) can easily pull up to 30,000 tickets per hour assuming they aren't using the API elsewhere.

Instructions for FreshService.pbit template file

1. Open the File and Enter url, DateFrom & MaxTickets to retrieve. Note if you try to retrieve more tickets than are available in your date range, you will get an error. Ensure your 'Max Tickets' is less than the number of tickets in your range. I suggest you start with the defaults for testing.
2. After clicking Load, you will likely get a 'Refresh' Error. You will need to input your credentials. → Click 'Close', then click 'Refresh'.
3. You will be prompted for credentials. Click 'Basic' then enter your login details for Freshservice.com (not SSO details if used)
4. You may need to play with filters etc to get tickets to show.
5. You can also adjust the Papramaters (URL, DateFrom, MaxTickets) in the query editor.
