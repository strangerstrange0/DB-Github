# DB-Github
GitHub Text Fetcher Extension for Kodular
VERSION: 1.0
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




