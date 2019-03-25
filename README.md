# Reading a google sheet with authentication

This script uses the google sheets api to read the date into a dataframe.

This could be used when the data requirement is sensative.

## Dependencies

1. Libraries
    ```bash
    apiclient==1.0.4
    google-api-python-client==1.7.8
    google-auth==1.6.3
    google-auth-httplib2==0.0.3
    httplib2==0.12.1
    oauth2client==4.1.3
    pandas==0.24.2
    ```
    All requirements => in `requirements.txt`
    
 2. Google sheets cloud API
    
    - [Python-api](https://developers.google.com/sheets/api/quickstart/python) => Enable => download as 'client_secret.json' (*need to rename*)
    - First run will ask for login authentication this will create the credentials.json
    
## How to use:

1. clone
2. `pip install -r requirements.txt`
3. set the document id `SPREADSHEET_ID` and the sheet name `RANGE_NAME` 


## Future updates:
How to use as a library just passing `get_data(sheet_id, range_name (sheet))`