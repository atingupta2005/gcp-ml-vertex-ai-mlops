
# /architectures/tracking/setup/youtube/readme.md

Setup the data reads from YouTube APIs

## Understand the API:
Overview:
- YouTube Developers Site: https://developers.google.com/youtube
    - Data API is for Search and Functionality: https://developers.google.com/youtube/v3
    - Analytics and Reporting API is for channel and content metrics: https://developers.google.com/youtube/analytics

Analytics & Reporting: https://developers.google.com/youtube/reporting
- Analytics API = Query
    - real-time, targeted queries that provide filtering and sorting parameters
    - requires data range for what to return - weekly,  monthly data sets
    - does the work of an application
- Reporting API = Bulk
    - bulk reports for a channel or owner
    - relies on the client caller to manage filtering and sorting
    
## Notebooks In This Folder:
    
