Simple Web App: Self-Intro Generator
This repository contains a simple, single-page web application designed to generate professional self-introduction or resume-like text based on user input. This client-side application was developed with the assistance of ChatGPT, leveraging its capabilities to quickly generate HTML, CSS, and JavaScript code.

Features:
---------
* Dynamic Form: Fields adapt based on user selections (e.g., "Experienced" option reveals more fields like "Years of Experience," "Company," and "Domain").
* IT/Non-IT Domain Selection: Populates relevant domain options based on the chosen industry.
* Application Support Level: Includes a specific field for "Application Support" domain users.
* Professional Intro Generation: Creates a concise self-introduction string based on collected data.
* Basic Navigation: "Home," "About," and "Contact" sections organize content, with client-side routing for a smooth user experience.
* Responsive Design: Uses meta viewport for basic responsiveness across various screen sizes.
Technologies Used-
------------------
* HTML5: Provides the foundational structure for the web page and its interactive form.
* CSS3: Styles the application, offering a modern and user-friendly interface with visual enhancements like gradients, shadows, and hover effects.
* JavaScript: Powers all interactive elements, including:
* Toggling form field visibility based on user input.
* Dynamically populating dropdown options.
* Generating the self-introduction text.
* Handling client-side navigation between different sections.
* Deployment Instructions (Debian/Ubuntu with Apache2)
  
This section outlines the steps to deploy this simple web application on a Debian or Ubuntu server using Apache2 as the web server.

Update Package Lists:
sudo apt update

Install Apache2:
sudo apt install apache2

Navigate to Apache's Web Root:
The default web root for Apache2 on Debian/Ubuntu is /var/www/html/.
cd /var/www/html

Clone the Repository:
Download the web application files from the GitHub repository.
sudo git clone https://github.com/Naveen-DevOps-IT/simplewebapp
(Note: You might need sudo if the current user doesn't have write permissions in /var/www/html)

Move Files to Web Root:
The git clone command creates a simplewebapp directory. Move all its contents directly into the current web root (/var/www/html/).
sudo mv simplewebapp/* .
(If you had an existing index.html or other files in /var/www/html, this command will overwrite them.)

Clean Up (Optional):
You can remove the now-empty simplewebapp directory.
sudo rm -r simplewebapp
After these steps, your web application should be accessible via your server's IP address or domain name in a web browser.
