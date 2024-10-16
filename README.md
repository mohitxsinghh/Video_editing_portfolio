# Video Editing Portfolio Website

This project showcases a video editing portfolio, allowing users to explore various categories of video content such as short-form videos, gaming videos, football edits, and more. Users can click on a category and view the corresponding video in the featured video section.

## Features

- **Interactive Video Categories**: Users can select from a list of categories like short-form videos, gaming videos, eCommerce ads, etc. Each category showcases a specific video related to that content.
- **Featured Video Display**: The website displays a default featured video upon loading. Users can click on a category to change the video displayed in the featured section.
- **Dynamic Video Switching**: Using JavaScript, the video in the featured section changes dynamically based on the user's selection, without reloading the page.
- **Responsive Design**: The website is optimized for desktop and mobile viewing.

## Technologies Used

- **HTML5**: For structuring the webpage.
- **CSS3**: For styling and making the layout responsive.
- **JavaScript**: For dynamically changing the video in the featured section when a category is selected.
- **YouTube Embed API**: Videos are embedded from YouTube using the embed URL format.

## How to Use

1. **Default Featured Video**: 
   - When the website first loads, a default featured video will be displayed in the player. This is defined in the `src` attribute of the `<iframe>`.
   
2. **Changing the Featured Video**:
   - Users can click on any of the video category buttons (e.g., "Short-form Videos," "Gaming Videos") to update the video displayed in the featured section.
   - This is handled by the `changeVideo()` function in JavaScript, which updates the video URL dynamically.

## Customizing the Website

### 1. Adding Your Own Videos
   - Replace the video URLs in the `src` attributes of the iframe and the `onclick` event in the HTML with the embed URLs of your own videos.
   - For YouTube videos, use the format:
     ```
     https://www.youtube.com/embed/VIDEO_ID
     ```
     Where `VIDEO_ID` is the unique identifier for your YouTube video.

### 2. Adding More Categories
   - To add more video categories, you can simply copy the structure of one of the existing `.column` divs in the HTML and update it with the new category name and corresponding video URL.

   Example:
   ```html
   <div class="column" onclick="changeVideo('https://www.youtube.com/embed/yourVideoID')">
       <h3>New Category</h3>
   </div>
