# EcoWiser Data-Science-Assignment
# LinkedIn API Data Scraping

## Overview
This Python script utilizes the `linkedin_api` library to scrape LinkedIn profile information. The script enables users to log in to their LinkedIn accounts, conduct searches based on first and last names, retrieve profile data for the top 10 search results, and save the data into a CSV file.

## Dependencies
Before running the script, ensure that you have the required library installed:

```bash
pip install linkedin_api
How to Use
Login Functionality

The login() function prompts the user for their LinkedIn credentials (username and password).
Maximum login attempts are set to 5, and the user is notified if login fails.
Search by Name

The search_name() function allows users to input a name (either full name or just the first name).
If no name is provided, the script defaults to a blank search based on LinkedIn connections.
Profile Information Retrieval

The profile_information_of_top_10_profiles(fname, lname=None) function obtains the unique URN (Uniform Resource Name) IDs for the top 10 search results.
The script then fetches detailed profile information using the obtained URN IDs.
Data Saving

The save_data(profiles) function consolidates the scraped profile information into a pandas DataFrame.
Empty lists in the data are replaced with None for better handling.
The data is reordered for better readability, and the script saves it to a CSV file named 'LinkedIN Profile Results'.
Runtime Information

The total runtime of the script is calculated and displayed.
