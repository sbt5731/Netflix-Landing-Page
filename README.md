# React Movie App

This is a React application that fetches and displays information about upcoming, popular, now playing, and top-rated movies using the TMDB API.

## Technologies Used

- React
- Axios
- React Icons
- SCSS
- TMDB API

## Functionality

The application consists of the following components:

- `Card`: Renders an image card for a movie.
- `Row`: Renders a row of movie cards with a specified title.
- `Home`: The main component of the application that fetches and displays movie data.

The `Home` component contains state variables to store data fetched from the TMDB API:

- `upcomingMovies`: Stores the upcoming movie data.
- `nowPlayingMovies`: Stores the now playing movie data.
- `popularMovies`: Stores the popular movie data.
- `topRatedMovies`: Stores the top rated movie data.

The component uses the `useEffect` hook to fetch the movie data from the TMDB API when the component is mounted. It makes separate API calls for each category of movies and updates the respective state variables.

The rendered output includes a banner section that displays information about the most popular movie. It shows the movie's title, overview, and background image. Buttons for playing the movie and adding it to the user's list are also provided.

Following the banner section, there are rows for each category of movies: upcoming, popular, now playing, and top rated. Each row contains a title and a list of movie cards, where each card displays the movie's cover image.

## Configuration

To run the application, you need to provide your TMDB API key. Open the `Home.js` file and replace the value of the `apiKey` constant with your TMDB API key.

## Usage

To run the application, you can use a development server such as [Create React App](https://create-react-app.dev/) or any other method you prefer.
