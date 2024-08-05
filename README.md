# Image Search Application

This project is a web application that allows users to search for images using the Unsplash API. It provides an interface to enter search keywords and displays relevant images based on the search criteria. Users can also load more images related to their search with the "Show More" button.

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Usage](#usage)
- [Code Overview](#code-overview)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Introduction

The Image Search Application is a simple web app that utilizes the Unsplash API to fetch and display images based on user search inputs. It features a search box where users can input keywords, and the application fetches relevant images from Unsplash. Users can view more images related to the same search by clicking the "Show More" button.

## Getting Started

### Prerequisites

- A modern web browser (e.g., Chrome, Firefox, Safari)
- Basic knowledge of HTML, CSS, and JavaScript
- An API access key from [Unsplash](https://unsplash.com/developers) (You need to sign up and create an application to obtain an access key)

### Installation

1. **Clone the Repository**:

   ```bash
   git clone <repository-url>
   cd image-search-application
   ```

2. **Replace API Key**:

   Replace the `accessKey` variable in the JavaScript file with your own Unsplash API access key:

   ```javascript
   const accessKey = "YOUR_ACCESS_KEY_HERE";
   ```

3. **Open the Project**:

   Open the `index.html` file in your web browser to use the application.

## Usage

1. **Search for Images**:

   - Enter a keyword in the search box and press the "Search" button or hit Enter.
   - The application will display a grid of images relevant to the entered keyword.

2. **Load More Images**:

   - Click the "Show More" button at the bottom of the search results to load more images.

## Code Overview

### 1. API Integration

The application uses the Unsplash API to fetch images. The API key is stored in the `accessKey` variable. The `searchImages()` function constructs the API URL using the search keyword and page number and fetches the images.

### 2. Handling User Input

The `searchForm` event listener triggers the image search when the user submits the form. The `searchBox` value is used as the search keyword, and the page number is reset to 1.

### 3. Displaying Images

Fetched images are displayed by creating `img` elements and wrapping them in `a` elements, linking to the original image on Unsplash. These elements are then appended to the `searchResult` container.

### 4. Pagination

The "Show More" button allows users to load additional images by incrementing the `page` variable and calling `searchImages()` again.

## Technologies Used

- **HTML**: Structure of the application interface.
- **CSS**: Styling and layout of the application.
- **JavaScript**: Logic for fetching and displaying images, handling user interactions.
- **Unsplash API**: Source of images.

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please fork the repository and create a pull request. For significant changes, please open an issue to discuss your ideas.

## License

This project is licensed under the MIT License.

## Acknowledgments

- Thanks to [Unsplash](https://unsplash.com/) for providing access to high-quality images through their API.
- Special thanks to the developers who created tools and libraries that made this project possible.
