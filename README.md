The application is built using CustomTkinter and provides a modern dark-themed interface for browsing seasonal anime information.

Key Features

• Scrapes seasonal anime from MyAnimeList by Year and Season  
• Filters results to only include "TV New" anime entries  
• Grid and List viewing modes for browsing anime  
• Dynamic search across title, genres, studio, and synopsis  
• Genre filtering dropdown  
• Sorting options:
  - Title
  - Score
  - Release Date
  - Members

• Displays rich metadata for each anime:
  - Title and subtitle
  - Release date
  - Score
  - Members
  - Studio
  - Source
  - Episode info
  - Genres, themes, and demographics
  - Synopsis preview
  - MAL page link
  - Cover image

• Lazy-loaded cover images for improved performance  
• Hover UI effects for cards and list rows  
• Seasonal color accents (Winter, Spring, Summer, Fall)  
• Progress bar with live parsing status  
• CSV export functionality for scraped results  

Technical Highlights

- Uses requests + BeautifulSoup for scraping MAL seasonal pages
- Targets the MAL TV New section (`js-seasonal-anime-list-key-1`)
- Implements threaded scraping to prevent UI freezing
- Lazy image loading with caching to improve responsiveness
- Dynamic grid layout based on window width
- Search + filter pipeline applied client-side

Export

Users can export filtered results into a CSV file containing:
title, subtitle, release date, genres, themes, demographics, score, members, studio, source, synopsis, episode info, MAL link, image URL, and type.

Purpose

This tool helps users quickly explore seasonal anime releases and analyze MAL data in a clean desktop interface.

Future Improvements (planned)

- MAL API integration (if available)
- Pagination for very large seasonal lists
- Additional anime types (Movies, ONA, OVA)
- Local caching database
- Favorites / watchlist support
