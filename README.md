# Hunter Shaye Web Gallery

This project consists of a webpage with a dynamic header, breadcrumbs, and a section featuring content related to Hunter Shaye. It includes integration with the Magnific Popup library for a sleek image gallery.

## Table of Contents

- [Project Structure](#project-structure)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Additional Information](#additional-information)

## Project Structure

 
|-- root
    |-- index.html
    |-- README.md
    |-- css/
    |   |-- styles.css
    |-- js/
        |-- script.js
 

## Dependencies

- [Magnific Popup](https://github.com/dimsemenov/Magnific-Popup): A responsive lightbox & dialog script with focus on performance.

## Usage

1. **HTML Structure:**
   - Include the following structure in your HTML file:
 
   <div class="page-width page-content"> 
     {%- render 'breadcrumbs' -%} 
     <header class="section-header">
       <h1 class="section-header__title">{{ page.title }}</h1>
     </header> 
     {% section 'hunter_shaye_section' %} 
   </div>
 

2. **Stylesheets:**
   - Include the Magnific Popup stylesheet in your HTML file:
 
   <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/magnific-popup.js/1.0.0/magnific-popup.min.css">
 

3. **JavaScript:**
   - Include jQuery and the Magnific Popup scripts in your HTML file:
 
   <script src="//ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
   <script src="https://cdnjs.cloudflare.com/ajax/libs/magnific-popup.js/1.0.0/jquery.magnific-popup.min.js"></script>
   <script src="https://cdnjs.cloudflare.com/ajax/libs/magnific-popup.js/1.0.0/jquery.magnific-popup.js"></script>
 

   - Add the following script for initializing Magnific Popup:
 
   <script type="text/javascript"> 
     $(document).ready(function ($) {
       $('.video').magnificPopup({
         type: 'image',
         gallery: {
           enabled: true
         }
       }); 
     }); 
   </script>
  

## Additional Information

- Make sure to customize the HTML, CSS, and JavaScript according to your project's requirements.
- Explore the Magnific Popup documentation for more configuration options: [Magnific Popup Documentation](https://dimsemenov.com/plugins/magnific-popup/documentation.html)
 

Feel free to customize this template based on the specifics of your project and add more details as needed.
