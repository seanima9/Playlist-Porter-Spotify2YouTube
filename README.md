# Spotify to YouTube Playlist Synchronizer 🚀

This project synchronizes tracks from a Spotify playlist to a YouTube playlist, automatically adding new tracks from Spotify to YouTube without duplicating existing ones. It's built using Python and utilizes the Spotify Web API and YouTube Data API v3 for playlist management.

## Getting Started

These instructions will guide you through setting up and running the project on your local machine.

## Prerequisites

Python 3.6 or higher
pip for installing dependencies
A Spotify Developer account and a Google Developer account for API access

## Installation

Clone the repository

Install required Python packages with
pip install -r requirements.txt

### Set up Spotify API access at https://developer.spotify.com/

Go to the Spotify Developer Dashboard and create an app to get your SPOTIFY_CLIENT_ID and SPOTIFY_CLIENT_SECRET.
Set up YouTube API access:

### Set up Google auth at https://console.cloud.google.com/getting-started?pli=1

Visit the Google Cloud Console, create a project, and enable the YouTube Data API v3.
Create OAuth 2.0 credentials to obtain the client_secret.json file. Download this file to your project directory.
Configure environment variables:


### Fill in your Spotify and Google credentials in a .env file in the same dir:

Will look like:

SPOTIFY_CLIENT_ID=your_spotify_client_id_here

SPOTIFY_CLIENT_SECRET=your_spotify_client_secret_here

YOUTUBE_CLIENT_SECRETS=path/to/your/downloaded/client_secret.json

## Usage

### Set Spotify Playlist ID and YouTube Playlist ID:

Add them to playlist_ids.txt, adding spotify id to line one and youtube music id to line 2

Run the Application:

Activate your venv, then run the program with 'python youtube_api.py'.
Make sure you are in the right dir when doing this
Follow the on-screen instructions to authenticate with YouTube on your first run.

Be aware of the API quota limits set by Google and Spotify.
Extensive use of the APIs will cause a quota timeout, you can rerun program again at 00:00 Tuesday, Pacific Time (PT) since the quota will have reset.

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues to suggest improvements or add new features.
