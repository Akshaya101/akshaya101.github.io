---
title: "User Profile for Spotify"
date: 2023-01-03T20:40:08+05:30
description: 'An application built using Spotify API'
ShowBreadCrumbs: true
ShowToc: true
TocOpen: false
cover:
    image: "images/spotify.png"
    # can also paste direct link from external site
    # ex. https://i.ibb.co/K0HVPBd/paper-mod-profilemode.png
    alt: "<alt text>"
    caption: "<text>"
    relative: false # To use relative path for cover image, used in hugo Page-bundles
---

## User Profile using Spotify
This website uses Spotify API and gives information about user activity. It also helps user to create playlists of their top tracks and recently played tracks.

This application gives information about user's 
- Top Tracks
- Top Artists
- Recently Played Tracks

It also lets the user create playlists for Top Tracks and Recently Played Tracks that will be added to User's Spotify Account Directly.

## Clone this Project

### Spotify Developer Dashboard Setup
1. To test this application locally, you need to register your application on [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/).
2. Create an app on the Developer Dashboard, you will be given **Client ID** and **Client Secret**
3. Upon achieving these, make sure you store these details somewhere as they would be further used in the application.

### Setting up the project locally

1. Clone the Project
2. Create a `.env` file in the root directory of the Project
3. In the .env file,
    - Create 4 Keys
    - `CLIENT_ID`, `CLIENT_SECRET`, `REDIRECT_URI`, `FRONTEND_URI`
    - Add the Client ID and Client Secret details here that we obtained from the developer dashboard.
4. `npm install`
5. `npm start`

### Find out more information
[Github Repository for the Application](https://github.com/Akshaya101/User-Profile-for-Spotify)