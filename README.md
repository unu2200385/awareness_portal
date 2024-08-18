The primary objective of this system is to enhance awareness of phishing by offering a user-friendly tutorial and personalized assessment. This assessment does not involve any real setup, such as a domain, infrastructure, or actual email address. It evaluates individuals' responses in various scenarios and provides insights into their current level of awareness.

## What?

- One of the primary goals of enterprises doing red team assessments is to identify vulnerabilities in the IT ecosystem, encompassing both individuals and networks. The organization makes every attempt to enhance their perimeter security and address any holes discovered, but individuals continue to be the most vulnerable aspect. Phishing is crucial for assessing an employee's level of security knowledge. 

- This system allows users to gain understanding of the concept without actually carrying out a real phishing assault. This is achieved by utilizing interactive and user-friendly training sessions.

- The tool provides a personalized platform for designing tests according to your specific needs. It generates tailor-made questions for each organization and individual, simulating real-time phishing attacks that are targeted, challenging, and scenario-based. It covers both SMishing questions and does not require any actual setup. After the test is created, all members of the intended audience can participate in the evaluation and submit their answers. We shall conduct an analysis at the conclusion of the campaign to ascertain the present state of awareness.

- A single click is all that is required. This will compel us to reconsider before doing that single action.

## Why?

Performing a red team evaluation is a challenging process of establishing a comprehensive phishing campaign. Select a domain, purchase it, establish a phishing website, create an email, and select a target audience. Monitor the clicks to determine the individuals who clicked on the email and their level of awareness.

- The establishment of this will require a significant amount of effort and specialized knowledge. 

- This tool will efficiently perform all of these tasks with just a few legitimate clicks, providing you with assistance.

- Individuals are highly unpredictable, and this tool will assist you in understanding their behavior and the patterns of their clicks.

## Features and How to use

This system have 2 main modules:
1. Admin Module : Which has access to setup test and view analysis, can be accessed at http://localhost/AdminPanel/login.php, default login credentials are admin/admin
- Set up test (Admin Module)
 	- The tool will prompt you to provide essential information at this stage. Some examples include:
 	- Domain Name: Please input your valid domain name, and the tool will generate a series of similar domains that potential attackers can use to target you.You have the option to select one of them, which will be utilized for your phishing simulation evaluation. 
 	- URL: Enter the URL of the websites you frequently visit, and system will generate a phishing website that closely resembles it. This website will be displayed under a domain that looks identical to the original, producing a real-life scenario known as 'Typosquatting' for assessment purposes.
 	- Test Code: You can generate a unique test code for each department and configure different tests for them, resulting in each person being exposed to distinct phishing sites. This approach makes the evaluation more challenging. Even when using the same exam set of questions, the responses will vary across each employee.
 	- Preview: You can examine the appearance and aesthetic of the phishing webpage that we have designed to closely resemble your original site.
 	- Email Id: Please provide an official email address that is commonly used for mass communication. We will generate other combinations of email addresses and utilize them for assessment purposes.
- Analysis (Admin Module)
	- This will have a graph of analysis of different scenarios based on the pattern in which employees has answered the questions.
	- This will help to know the current awareness posture of organization.
- Invite (Admin Module)	
	- Admin can upload CSV file and invite the members to take test.

2. Client Module : Which only has access to tutorial and assessment, can be accessed at http://localhost/phishClient/
 - Tutorial (Client Module)
	- This will have a tutorial book which introduces phishing and the general techniques used which will create awareness and educate.
- Assessment (Client Module)
	- This will consist of a range of inquiries that may involve phishing emails, phishing websites, situations, or SMiShing. Users will need to decide whether to click on, ignore, or report these items.
	- Each user will receive unique questions even if they have the same test code.
	- Questions shall consist of an equitable combination of positive and negative inquiries.
	- In order to successfully complete the test, it is necessary for all answers to be correct. It only takes one wrong action to be a victim of a Phishing attack

### Installation Guidelines

1. Download XAMPP from - https://www.apachefriends.org/download.html and follow installation flow on the screen. It will install webserver and MySQL for you.
2. Once you have completed Step 1, on XAMPP control panel start 'Apache' and 'MySQL' service.
4. Open http://localhost/phpmyadmin/ on the browser.
5. Click on 'Databases' create database with name 'phishadmin'
6. Click on 'Import' and import the database file from /sql/folder phishadmin.sql
7. Copy the source code of the system, paste it in C:\xampp\htdocs\ and you are done with setup. 
