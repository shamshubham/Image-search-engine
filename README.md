# 📸 Image Search Application

Welcome to the Image Search Application, a sleek and intuitive web tool that allows users to search for stunning images using the Unsplash API. With a simple interface, you can enter search keywords and explore a world of high-quality visuals. Easily load more images with the "Show More" button to discover additional content.

## 📑 Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Usage](#usage)
- [Code Overview](#code-overview)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)
- [Screenshots](#screenshots)

## 🌟 Introduction

The **Image Search Application** is a user-friendly web app that leverages the Unsplash API to fetch and display images based on user queries. Simply type in your desired keywords, and the app will present a gallery of relevant images. Whether you're searching for inspiration or specific visuals, this tool makes it easy to explore Unsplash's extensive collection.

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, etc.)
- Basic knowledge of HTML, CSS, and JavaScript
- An API access key from [Unsplash](https://unsplash.com/developers) (Sign up and create an application to get an access key)

### Installation

1. **Clone the Repository**:

   ```bash
   git clone <repository-url>
   cd image-search-application
   ```

2. **Replace API Key**:

   Insert your Unsplash API access key in the JavaScript file:

   ```javascript
   const accessKey = "YOUR_ACCESS_KEY_HERE";
   ```

3. **Open the Project**:

   Open the `index.html` file in your web browser to start using the application.

## 🔧 Usage

1. **Search for Images**:

   - Enter a keyword in the search box and press the "Search" button or hit Enter.
   - The application will display a grid of images related to the entered keyword.

2. **Load More Images**:

   - Click the "Show More" button at the bottom of the results to load additional images.

## 🧩 Code Overview

### 1. API Integration

The Unsplash API is integrated to fetch images. The `accessKey` variable stores the API key, and the `searchImages()` function generates the API request URL using the search keyword and page number.

### 2. Handling User Input

An event listener on the `searchForm` triggers the image search upon form submission. The `searchBox` value is utilized as the search keyword, and the page number is initialized to 1.

### 3. Displaying Images

Images retrieved from the API are displayed by creating `img` elements wrapped in `a` tags, linking to the original Unsplash image. These are appended to the `searchResult` container.

### 4. Pagination

The "Show More" button fetches more images by incrementing the `page` variable and re-invoking `searchImages()`.

## 💻 Technologies Used

- **HTML5**: Provides the structure of the web app.
- **CSS3**: Handles the styling and layout.
- **JavaScript**: Manages data fetching, user interactions, and dynamic updates.
- **Unsplash API**: Supplies the image data.

## 🤝 Contributing

Contributions are highly encouraged! To contribute:

1. **Fork the Repository**: Create your version of the project.
2. **Create a New Branch**: Develop your changes in a dedicated branch.
3. **Commit Changes**: Document your work with clear commit messages.
4. **Push to Your Fork**: Upload your changes to your forked repository.
5. **Submit a Pull Request**: Submit your changes for review and potential inclusion in the main project.

For substantial modifications, please discuss your ideas via an issue first.

## 📜 License

This project is licensed under the MIT License.

## 🙏 Acknowledgments

- A special thanks to [Unsplash](https://unsplash.com/) for providing an amazing API with access to high-quality images.
- Thanks to all the open-source contributors whose tools and libraries have made this project possible.

## 📸 Screenshots

- ![Screenshot 1](https://github.com/shamshubham/Image-search-engine/blob/master/screenShots/Capture.JPG)
- ![Screenshot 2](https://github.com/shamshubham/Image-search-engine/blob/master/screenShots/Capture1.JPG)
- ![Screenshot 3](https://github.com/shamshubham/Image-search-engine/blob/master/screenShots/Capture3.JPG)
