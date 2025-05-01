# Dig Deep Construction
Website Project - HTML, CSS

The website is a landing page for a construction company. The website's main purpose is to inform the readers about their services, history and accreditations. The wesbite also provides contact information and provides the user an opportunity to request for a phone call about a specific service. 

![image](https://github.com/user-attachments/assets/e2e50f81-eda1-4414-869e-5de4a6f14884)

## Features
### 1. **Navbar**
   - Located at the top of the website.
   - Contains links to: "About", "Services" and "Contact"
   - "Contact" is a dropdown where the user picks between "Request Call" or "Our Info". Each directing them to a different section.

### 2. **Header**
   - Displays the company name and tagline.
   - Includes a call-to-action button linking to the contact form.
     
![image](https://github.com/user-attachments/assets/7f457706-3155-440f-b3f5-cff9325d7741)

### 3. **About Us**
   - Provides information about the company's history, values, and certifications.
![image](https://github.com/user-attachments/assets/46021117-0638-4c42-a067-88d595c29bac)

### 4. **Services**
   - Highlights the company's key services with detailed descriptions.
![image](https://github.com/user-attachments/assets/716b823b-e770-4e62-b3b3-340bac14db41)

### 5. **Contact**
   - A form for users to submit their name, email, phone number, service selection, and comments.
   - Includes a modal confirmation upon successful submission.
![image](https://github.com/user-attachments/assets/57ad7f25-3930-42b1-a2e5-8b503c3fc76f)
![image](https://github.com/user-attachments/assets/e3f220a1-2c15-4a35-8f29-96cedceda6cf)

### 6. **Footer**
   - Displays contact details, operating hours, location, and social media links.
![image](https://github.com/user-attachments/assets/5175b096-c6bf-4dff-ae91-07eab16a35d6)

### Key Files
- **`index.html`**: The main HTML file containing the structure of the website.
- **`styles.css`**: Custom CSS file for additional styling.
- **`helmet-safety-solid.svg`**: Favicon for the website.
- **`header-image.sjpg`**: Image for header background.

## Testing
- The website was tested on Chrome, Firefox and Safari for resposiveness.
- The form and dropdowns work as intended on all browsers listed.
- The wesbite looks as it was intended on all device sizes on the browsers mentioned above.

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
![image](https://github.com/user-attachments/assets/84d0c70a-74d5-4d37-b87d-4ac60a0fce1d)

### Unsolved bugs
- No bugs were left unsolved. 

## Dependencies
- [Bootstrap 5](https://getbootstrap.com/)
- [Font Awesome](https://fontawesome.com/)
- [Google Fonts](https://fonts.google.com/)

## Deployment
- The site was deployed using GitHub pages. The steps to deploy are as follows:
   - In the Github repository, navigate to Settings tab.
   - From the source section drop down menu, select Master Branch.
   - Once Master Branch selected, a link will be generated to the page.
   - The live link can be found here: [Dig Deep Construction](https://alijaycarter.github.io/dig-deep-construction/)

## Credits
- **Bootstrap**: Code from bootstrap was used for features such as cards, modal, navabar and form.
- **Co-pilot**: used to generate text to fill content. 

## Custom Scripts
The project includes a JavaScript snippet to handle form submission:
```javascript
document.getElementById('myForm').addEventListener('submit', function (event) {
  event.preventDefault(); // Prevent actual form submission

  // Show Bootstrap modal
  var myModal = new bootstrap.Modal(document.getElementById('submitModal'));
  myModal.show();
});
