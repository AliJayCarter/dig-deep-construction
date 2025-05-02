# Dig Deep Construction
Dig Deep Construction is a time efficent landing page whereby the user can quickly access the information needed about the company. The user can then request a call from the company with their desired needs as efficently as possible, allowing the business to have a specialist in their required service contact the user. 

![image](https://github.com/user-attachments/assets/e2e50f81-eda1-4414-869e-5de4a6f14884)

## Features
### 1. **Navbar**
   - Located at the top of the website at all times and follows down the page as the user scrolls down. 
   - Contains links to: "About", "Services" and "Contact"
   - "Contact" is a dropdown where the user picks between "Request Call" or "Our Info". Each directing them to a different section.
   - "Contact" link has been removed for the success page once the user has submitted their request for a call.

#### Large laptop view
![image](https://github.com/user-attachments/assets/7802fd04-dc3e-459a-99bf-ebd61006f19f)

#### Mobile
![image](https://github.com/user-attachments/assets/75532e19-f147-47b7-98d6-f31db3ddc349)
![image](https://github.com/user-attachments/assets/a5779e95-a608-4679-858f-25808ef0e993)


### 2. **Header**
   - Displays the company name and tagline.
   - Includes a call-to-action button linking to the contact form.
   - **See images above**

### 3. **About Us**
   - Provides information about the company's history, values, and certifications.
#### Large Laptop
![image](https://github.com/user-attachments/assets/95651c1b-3f90-4314-91e7-e51ff1ff6aa2)
#### Mobile
![image](https://github.com/user-attachments/assets/484fe761-663d-4ad1-ab26-6eed76d89f71)

### 4. **Services**
   - Highlights the company's key services with detailed descriptions.
#### Large laptop
![image](https://github.com/user-attachments/assets/b43e8569-0dbb-4fb0-b51b-8a9919706974)
#### Mobile
![image](https://github.com/user-attachments/assets/9e34c6f1-d951-4835-a8e5-02967a6e95b2)

### 5. **Contact**
   - A form for users to submit their name, email, phone number, service selection, and comments. Form validation included to ensure that the user completes the form. 
   - Opens a new html file "success.html" where a message is shown about thir succesful submission. They can then naviaget themselves back to the home back from the modified navbar.
   - Submit button changes color when mouse is hovered over the button. 
#### Large Laptop
![image](https://github.com/user-attachments/assets/98efadff-e937-4cd1-b028-50f4016d25bd)
#### Mobile
![image](https://github.com/user-attachments/assets/91b98f06-0eb0-44c2-8ac4-9c809a0d4863)

### 6. **Success**
   - New html file where a message is shown to the user that their submission has been recieved and that they will be contacted shortly.
   - User can direct themselves back to the home page by clicking on the "helmet" icon or directing themselves back to the "index.html" file to review the services again.
#### Large laptop
![image](https://github.com/user-attachments/assets/2b589dc4-4b91-4612-88f0-d8fb3906030f)
#### Mobile
![image](https://github.com/user-attachments/assets/a5cc006a-ad9e-498f-8ad5-7e9076572536)

### 6. **Footer**
   - Displays contact details, operating hours, location, and social media links.
   - Footer is the same for the "home(index.html)" page and the "success" page. 
#### large Laptop
![image](https://github.com/user-attachments/assets/1370f954-1ef7-40d0-b327-aaa1471a3ec0)
#### Mobile
![image](https://github.com/user-attachments/assets/f7dab9c4-da4c-4bd4-9f47-279072c0c45c)

## Wireframe
![image](https://share.balsamiq.com/c/1etaBDNsjZGiC76nG88zmo.jpg)


## Key Files
- **`index.html`**: The main HTML file containing the structure of the website.
- **`success.html`**: The main HTML file containing a success message once the user completes a "request for contact" form. 
- **`styles.css`**: Custom CSS file for additional styling.
- **`helmet-safety-solid.svg`**: Favicon for the website.
- **`header-image.sjpg`**: Image for header background.

## Manual Testing
### 1. General Testing
- Website checked if it loaded correctly and it worked as intended.
- Various browers were used to check cross-platform functionality.
- Resposiveness was checked on the various browsers.
- Checked the favicon and wesbite title was displayed. 

### 2. Navbar: 
- The navbar was tested to ensure it was visible and toggled to a drowdown icon on mobile screens and expanded on laptop screens.
- Each link(about, services and contact) was clicked to check to see if it naviagted to the correct section.
- Contact link was checked for dropdown functionality and if Request call and Our info was displayed below. 
- Checked if it was sticky by scrolling down the page. 

### 3. Header: 
- The section was checked if the image, text and button displayed correctly.
- The "request call" button was checked to ensure it navigated correctly. 

### 4. About Section: 
- Checked to ensure the cards displayed correctly on various screen sizes.
- Informaition on the cards was checked to ensure it was correct.
- Titles of the cards were checked.
  
### 5. Services Section
- Checked to ensure the cards displayed correctly on various screen sizes.
- Informaition on the cards was checked to ensure it was correct.
- Titles of the cards were checked.
  
### 6. Contact Form Section
- Checked the form displayed correctly depending on the screen size.
- Verified the titles were correct for each field.
- Ensured the titles were requried and of the correct type.
- Pressed the "submit information" button with valid data to ensure redirect to "success.html" file.

### 7. Footer
- Checked for correct display for different screen sizes.
- Checked the information and titles were correct.
- Tested the Google maps embedded code to ensure it displayed the correct location.
- Clicked on the social media links to ensure it opened in a new tab. 

### 8. Success Page
- Ensured the page was displayed when completing form with valid data.
- Ensured the page was responsive according to various screen sizes.
- Checked the success message was correct.
- Verified the "helmet" icon redirects to the "home" page.
- Checked the nav bar to ensure the "contact" link was not displayed.
- Checked the footer to ensure it displayed the same way as the "index" file.
- Checked social media links to ensure they open in a new tab. 

## Bugs
### Fixed Bugs
- Heights of cards from Bootstrap library varied in height for the "About" and "Services" section on various devices. Media queries for screen widths were added to ensure the heights alligned.
   - max-width: 425px: min-height for both sections changed to 200px.
   - min-width: 768px min height "About" set to 342px and 430px for "Services sections.
   - min-width: 1024px min height "About" set to 230px and 250px for "Services sections.
- Contact form: Added value="" to ensure user cannot submit without picking a dropdown option for the "Services".

### Validator Testing
- HTML: No erros were returned from the official W3C validator.
- CSS: No erros were returned from the official Jigsaw validator.
- Accessibilty: I confirmed the fonts and colors are suitable by running the code through Lighthouse in devtools.
![image](https://github.com/user-attachments/assets/e6a2f759-0a50-4b36-ae9f-7041a3563ad1)

### Unfixed bugs
- No bugs were left unfixed. 

## Dependencies
- [Bootstrap 5](https://getbootstrap.com/)
- [Font Awesome](https://fontawesome.com/)
- [Google Fonts](https://fonts.google.com/)

## Deployment
### Github
- The site was deployed using GitHub pages. The steps to deploy are as follows:
   - In the Github repository, navigate to Settings tab.
   - From the source section drop down menu, select Master Branch.
   - Once Master Branch selected, a link will be generated to the page.
   - The live link can be found here: [Dig Deep Construction](https://alijaycarter.github.io/dig-deep-construction/)
 
### Local
- Install Git and VS Code.
   - Clone the repository using git clone.
   - Navigate into the project folder.
   - Open the project in VS Code.
   - Run the project.

## Credits
- **Bootstrap**: Code from bootstrap was used for features such as cards, modal, navabar and form.
- **Pexels**: Used to obtain the header image.
- **w3schools**: Used for coding help for different aspects of the project.
