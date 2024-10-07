# Genre Fetching from Spotify
This Python script, getgenre.py, retrieves music genres for songs listed in a Billboard CSV file using the Spotify API. Below is a brief overview of its functionality:
Key Features:
Spotify API Integration: Utilizes the Spotipy library to connect to the Spotify API and fetch genre information.
CSV Handling: Reads a CSV file containing song and artist data, specifically Billboard100rank2023up.csv.
Genre Retrieval: For each song, it searches the Spotify database to obtain the associated genres.
Caching Mechanism: Implements a caching system to avoid redundant API calls, storing results in a JSON file (cachedict.json).
Rate Limiting Management: Handles API rate limits by pausing execution when necessary and retrying requests.
Output: Updates the original CSV file by adding a new column for genres.
Usage:
1. Ensure you have valid Spotify API credentials.
2. Place the Billboard100rank2023up.csv file in the same directory.
3. Run the script to fetch and append genres to the CSV file.
Dependencies:
pandas
spotipy
tqdm
json
os
---
