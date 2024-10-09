# Movie Recommender System

This is a movie recommendation system built using Streamlit, pickle, and The Movie Database (TMDb) API. The application allows users to select a movie from a dropdown menu and get recommendations for similar movies along with their posters.

## Features

- **Movie Recommendations**: Recommends five similar movies based on the selected movie.
- **Movie Posters**: Displays the posters of the recommended movies by fetching data from the TMDb API.
- **Interactive User Interface**: Built using Streamlit, the UI is interactive and easy to use with dropdown selections and responsive design.

## How It Works

1. **Movie Selection**: Users can select a movie from the dropdown, which is populated with data from a preloaded list of movies.
2. **Recommendation**: The application calculates similarity scores between the selected movie and other movies using a pre-trained model.
3. **Poster Fetching**: The application fetches the poster of the recommended movies using TMDb API.


### Prerequisites

- Python 3.x
- Required Python libraries:
  - `streamlit`
  - `requests`
  - `pickle`
  - `pandas`
  - `numpy`

### Setup and Running the App

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/movie-recommender-system.git
    cd movie-recommender-system
    ```

2. Install the required libraries:

    ```bash
    pip install -r requirements.txt
    ```

3. Run the Streamlit app:

    ```bash
    streamlit run app.py
    ```

4. Open your browser and go to `http://localhost:8501` to view the application.

### TMDb API Key

To run the app, you will need a TMDb API key. You can get one by signing up at [The Movie Database](https://www.themoviedb.org/).

Replace the API key in `app.py` at the following line:

```python
url = "https://api.themoviedb.org/3/movie/{}?api_key=YOUR_API_KEY&language=en-US".format(movie_id)
