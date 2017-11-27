FEND Website Optimization Project
==============================================================================

Installation and Use
------------------------------------------------------------------------------
- Download the Website's ZIP file [here](https://github.com/srdmdev8/frontend-nanodegree-mobile-portfolio)
  - Select **Clone or download**
  - Then select **Download ZIP**
- Save the ZIP file in desired location on your computer
- Unzip/extract all files
- Open the **index.html** file
  - Double-click the file to open in your computer's default browser or
  - Right-click the file and choose **Open** or **Open with..**
    - *Open with.. will allow you to choose the application you would like to open the file with*

Optimizations Made
------------------------------------------------------------------------------
#### index.html:
- Updated all images to reference actual saved images within the project
- Moved **style.css** to the footer section
- Removed the Google Font link and added it to **style.css**
- Added `media="print"` to **print.css**

#### main.js
- Simplified the calculations for the `changePizzaSizes` function:
  - Removed the `determineDx` function
  - Combined the `changePizzaSizes` and `sizeSwitcher` functions:
   - Added variable **pizzaWidth** and made it equal to the 3 different sizes in the switch case
   - For my **randomPizzas** varibale, I updated the `querySelector` to `getElementsByClassName`
   - Calculated pizza sizes in the For loop using the percentage of my new **pizzaWidth** variable
- Updated the `updatePositions` function:
  - For the **items** variable, I updated the `querySelector` to `getElementsByClassName`
  - Cached the *scrollTop* item in my **top** variable outside of the For loop
- In the function for the `addEventListener` that initially loads the sliding pizzas, I updated the count of 200 to 20 within the For loop. This way the page only loads 20 pizzas instead of 200 since you can only see very few pizzas at any given time

#### images
- Added images to the main images folder that were being reference from a URL
in index.html so that I could reference the images directly from the project
- Resized the pizzeria JPEG and saved it as a PNG
