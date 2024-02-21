# Animated Loader

This repository contains HTML and CSS code to create an animated loader with a wave effect. Follow the steps below to understand how to use this code.

## Preview
![preview](https://github.com/withaarzoo/loader/assets/59678435/bf7dbee2-e9b5-4d10-a192-7b53c5f33edf)

## Steps:

1. **Clone the Repository:**
   ```
   git clone https://github.com/withaarzoo/loader.git
   ```

2. **Navigate to the Directory:**
   ```
   cd loader
   ```

3. **HTML Structure:**
   - Open `index.html` file in your preferred text editor.
   - You will find the following HTML structure:

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <link rel="stylesheet" href="style.css">
       <title>Animated Loader</title>
   </head>
   <body>
       <div class="loading-wave">
           <div class="loading-bar"></div>
           <div class="loading-bar"></div>
           <div class="loading-bar"></div>
           <div class="loading-bar"></div>
       </div>
   </body>
   </html>
   ```

4. **CSS Styles:**
   - Open `style.css` file.
   - You'll find the CSS styles responsible for creating the loader animation.
   - The animation is applied to the `.loading-bar` class using keyframes.
   - Each `.loading-bar` is given a specific animation delay to create a wave effect.

   ```css
   * {
       margin: 0;
       padding: 0;
       box-sizing: border-box;
   }

   body {
       display: flex;
       align-items: center;
       justify-content: center;
       min-height: 100vh;
   }

   .loading-wave {
       width: 300px;
       height: 100px;
       display: flex;
       justify-content: center;
       align-items: flex-end;
   }

   .loading-bar {
       width: 20px;
       height: 10px;
       margin: 0 5px;
       background-color: #3498db;
       border-radius: 5px;
       animation: loading-wave-animation 1s ease-in-out infinite;
   }

   .loading-bar:nth-child(2) {
       animation-delay: 0.1s;
   }

   .loading-bar:nth-child(3) {
       animation-delay: 0.2s;
   }

   .loading-bar:nth-child(4) {
       animation-delay: 0.3s;
   }

   @keyframes loading-wave-animation {
       0% {
           height: 10px;
       }
       50% {
           height: 50px;
       }
       100% {
           height: 10px;
       }
   }
   ```

5. **View in Browser:**
   - Open `index.html` in your web browser to see the animated loader in action.

6. **Customization:**
   - You can customize the loader by adjusting the width, height, colors, animation duration, etc., in the CSS file.

7. **Integration:**
   - Integrate this loader into your projects by copying the HTML structure and CSS styles.

8. **Enjoy!**
   - Enjoy using this animated loader in your projects.

Feel free to reach out if you have any questions or need further assistance!
