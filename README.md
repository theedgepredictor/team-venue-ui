# Team Venue UI

Team Venue UI is a web application that displays the locations of sports league teams on an interactive map using Streamlit and Folium.  The app dynamically fetches and displays data based on the selected sport, league, and season.

## Features

- Interactive map showing team venues
- Dropdowns to select sport, league, and season
- Dynamic data fetching from remote sources
- Utilizes Streamlit for the web interface and Folium for the map visualization

## Data Sources

- **Season Data**: [College Football Season Data 2024](https://raw.githubusercontent.com/theedgepredictor/team-data-pump/main/data/football/college-football/2024/teams.json)
- **General Team Info**: [College Football General Team Info](https://raw.githubusercontent.com/theedgepredictor/team-data-pump/main/data/football/college-football/teams.json)
- **Venues**: [College Football Venues](https://raw.githubusercontent.com/theedgepredictor/venue-data-pump/blob/main/data/football/college-football/venues.json)
- **Generic Geocoded Locations**: [Generic Geocoded Locations](https://raw.githubusercontent.com/theedgepredictor/venue-data-pump/blob/main/data/geocoding.json)

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/team-venue-ui.git
    cd team-venue-ui
    ```

2. Install the required libraries:
    ```bash
    pip install streamlit folium pandas requests
    ```

## Usage

1. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

2. Open your web browser and navigate to `http://localhost:8501` to access the application.

## How It Works

1. **Initial Load**: The app fetches generic geocoded locations on initial load.
2. **Select Sport and League**: Users can select the sport (e.g., Football) and the league (e.g., college football, NFL).
3. **Fetch Data**: Upon league selection, the app fetches the relevant venues and general team info.
4. **Select Season**: Users can select the season (e.g., 2024). The app then fetches the season-specific data.
5. **Display Map**: The map is updated with markers for each team based on the selected sport, league, and season.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any enhancements or bug fixes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.