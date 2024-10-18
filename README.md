# Tatkal-Train-Ticket-Booking-using-UIPath
an RPA code that is invoke in UIPath for booking the train ticket in tatkal
This repository contains an RPA solution built with UiPath Studio to automate the process of booking Tatkal train tickets on the Indian Railways website (IRCTC). The automation script fills in the required booking details, navigates the IRCTC website, and completes the booking for a Tatkal ticket.

Table of Contents
Prerequisites
 Features
 Process Overview
 Installation
 Configuration
 Usage
 Contributing
 License
 Prerequisites
Before running this automation, ensure the following software is installed on your system:

UiPath Studio
UiPath Browser extension (for Chrome/Firefox)
A valid IRCTC account
Access to a Tatkal ticket booking window
Features
Automates the login process to the IRCTC website.
Handles form filling for passenger details, travel class, and other required information.
Selects trains based on availability, class, and timing.
Manages Captcha inputs (to a degree, manual intervention is required).
Finalizes booking using pre-saved payment methods.
Process Overview
Login to IRCTC: The bot opens the IRCTC website and logs in using credentials provided during the configuration.
Navigate to Tatkal Booking Section: The bot navigates to the Tatkal ticket booking window, selects the train route, and date.
Passenger Information: Passenger details, such as name, age, gender, and seat preferences, are entered automatically.
Captcha Handling: Since captchas require human intervention, the bot pauses and waits for manual captcha entry before proceeding.
Finalize Booking: The bot completes the booking by selecting a preferred payment method, which must be set up in the configuration.
Installation

Open the project in UiPath Studio.
Install the required dependencies from the Manage Packages section in UiPath Studio.
Configuration
IRCTC Credentials:

Go to the Config.xaml file in the project.
Add your IRCTC credentials (username and password) in the respective arguments.
Passenger Details:

In the PassengerDetails.xlsx file, enter the necessary information (name, age, gender, etc.) for each passenger.
Preferred Trains & Payment Method:

Modify the workflow to select your preferred train and payment option. You can edit the selectors for these actions in UiPath Studio.
Usage
Open UiPath Studio and run the automation from the main workflow file (Main.xaml).

Once executed, the bot will:

Launch a web browser and navigate to the IRCTC website.
Log in using your credentials.
Begin the booking process for the selected route and train.
Wait for manual input to solve the captcha.
Finalize the booking.
Important: You will need to manually enter the captcha at the required steps during the booking process.

Contributing
Feel free to submit a pull request if you want to improve the automation, add features, or fix any bugs.

License
This project is licensed under the MIT License - see the LICENSE file for details.
