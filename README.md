# DB-Github VERSION: 2.0
GitHub Text Fetcher Extension for Kodular
Easily fetch raw text data directly from GitHub for dynamic content in your Kodular apps.

# About This Extension
This Kodular extension (GitHub Text Fetcher) provides a simple and efficient way for your applications to retrieve raw text content from any public GitHub file. This allows you to update in-app information (like announcements, configurations, news, etc.) without needing to publish a new app version.

# Features
1.Asynchronous Data Fetching: Retrieves text data in the background without freezing your app's UI.
2.Direct GitHub Raw Link Support: Works directly with the raw file URLs from GitHub.
3.Event-Driven Responses: Triggers specific events for both successful data retrieval and any errors that occur.
4.Lightweight & Easy to Use: Minimal blocks required to integrate dynamic content.

# Installation 
 Download the DB_Github.aix file from the root of this repository.
 Open Kodular Creator.
 In the Palette section, navigate to "Extension" and click "Import Extension."
 Select and import the downloaded GitHubTextFetcher.aix file.
 Drag the GitHubTextFetcher component from the "Extension" category onto your screen in the Designer.

# Blocks
The DB_Github extension provides the following blocks for seamless integration with your Kodular projects:

1. ![image](https://github.com/user-attachments/assets/01e4cd45-8474-4d0d-becb-7787afd200a5)

with this block you can call spesific text data but you must add its raw URL
example: (https://raw.githubusercontent.com/your-username/your-repository/main/your-file.txt)

2. ![image](https://github.com/user-attachments/assets/6771189a-6105-475b-941a-f63313dc7e9d)

This event is triggered when the text data has been successfully fetched from the GitHub raw URL specified in the GetGithubData call. This is where you will receive the content of your GitHub file.

3. ![image](https://github.com/user-attachments/assets/b7699151-17a7-47b2-8964-6fe7d1f4e6da)

This event is triggered if an error occurs during the data fetching process (e.g., network issues, invalid URL, file not found, server errors, or any other issue that prevents a successful request).

4. ![image](https://github.com/user-attachments/assets/91908341-c088-428d-ba7a-f3a6589256ba)

This event allows you to download a file from a specified URL (e.g., a raw GitHub file) and save it to a designated location on the user's device. This is particularly useful for downloading assets, configurations, or other files directly from your GitHub repository.

5. ![image](https://github.com/user-attachments/assets/57f17325-9ce2-4f0f-b13f-18b35cc0f9ac)

This method is designed to fetch JSON formatted data from a specified URL, typically a raw JSON file hosted on GitHub.

6. ![image](https://github.com/user-attachments/assets/457c3d86-81fd-4f84-bcd1-8ef2b5aedcb5)

This event is triggered when a file initiated by the Download File method has been successfully downloaded and saved to the specified folderPath on the device.

7. ![image](https://github.com/user-attachments/assets/7a26337a-b67b-4c70-b204-e56c6642a3be)

This event is triggered when JSON data, initiated by the FetchJsonData method, has been successfully fetched from the specified GitHub URL. This block provides the raw JSON content as a string, which you can then parse using Kodular's built-in JSON utilities.









