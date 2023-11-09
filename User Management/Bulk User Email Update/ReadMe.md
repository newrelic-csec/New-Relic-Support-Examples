# New Relic Bulk User Email Update

<a href="https://opensource.newrelic.com/oss-category/#example-code"><picture><source media="(prefers-color-scheme: dark)" srcset="https://github.com/newrelic/opensource-website/raw/main/src/images/categories/dark/Example_Code.png"><source media="(prefers-color-scheme: light)" srcset="https://github.com/newrelic/opensource-website/raw/main/src/images/categories/Example_Code.png"><img alt="New Relic Open Source example project banner." src="https://github.com/newrelic/opensource-website/raw/main/src/images/categories/Example_Code.png"></picture></a>


This Python script allows you to update the email addresses of one or multiple users in your New Relic account using the New Relic's Nerdgraph API. Please see further documentation on this API here: https://docs.newrelic.com/docs/apis/nerdgraph/examples/nerdgraph-manage-users/

## How to Use

1. Before using this script, you must have a New Relic account and generate an API key for your account. To generate an API key, please follow the instructions in the [New Relic documentation](https://docs.newrelic.com/docs/apis/get-started/intro-apis/types-new-relic-api-keys#admin).

2. Save the user ID and new email address for each user you wish to update in a CSV file. The CSV file should have two columns: 'ID' and 'Email'.

3. Run the script by executing the following command in your terminal or command prompt:

    ```
    python bulk-update.py
    ```

4. You will be prompted to enter your New Relic API key and the path to the CSV file.

5. The script will loop through each row in the CSV file and update the email addresses of each user.

6. If there are errors in the response from the New Relic Nerdgraph API, the script will print out the error messages. If the update is successful, the script will print out a success message for each user ID that has been updated.

## Requirements

- Python 3.x
- `requests` module: You can install this module by running `pip install requests` in your terminal or command prompt.
