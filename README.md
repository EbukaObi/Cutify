# CUTIFY

## Introduction
CUTIFY is a web-based tool that allows users to shorten long URLs into shorter and more manageable links. It provides a simple, user-friendly interface to generate short URLs, track clicks, and manage the URLs and also user data.

The application is built using the Flask framework, a lightweight and extensible web framework for Python. It utilizes a SQLite database for storing URL mappings and tracking url clicks. The frontend is designed using HTML, CSS, and JavaScript, with support for generating QR codes for shortened URLs. And also other necessary libraries like matplotlib for generating charts for analytics, flask-cache for caching and also flask-limiter for rate limiting etc.

## Features
CUTIFY offers the following features:

1. **Shorten long URLs:** Users can input a long URL and generate a shorter, more compact and unique version. The application generates a unique shortcode for each URL, which is used to access the original URL when the shortened link is visited.
2. **Customizable URLs:** Users have the option to customize the shortcode of their shortened URL by providing a custom alias.
3. **Click Tracking and Analytics:** The application tracks the number of clicks received for each shortened URL. Users can view analytics data such as total clicks, clicks per day, and the most clicked day for each shortened URL with graphical representation.
4. **QR Code Generation:** The application generates QR codes for each shortened URL, making it convenient for users to download and share URLs across devices.
5. **History:** For users who would like to browse through URLs they previously shortened, the application also includes a history feature. URLs that were shortened by a user are stored and made accessible to users any time.  
6. **Password-Protected URLs:** One unique feature about this application is the option to secure shortened URLs 
   with passwords. For users that want to shorten and secure URLs contain sensitive data, you can choose to protect 
   your shortened URLs with a password 
   for added security. 

## Installation
To set up the URL Shortener application, follow these steps:

1. Clone the repository:
   ```
   git clone https://github.com/EbukaObi/Cutify
   ```
2. Change into the project directory:
   ```
   cd Cutify
   ```
3. Create a virtual environment:
   ```
   python3 -m venv venv
   ```
4. Activate the virtual environment:
   - On Windows:
     ```
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```
     source venv/bin/activate
     ```
5. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```
6. Set environment variable:
   - On Windows:
     ```
     set FLASK_APP=app.py
     ```
   - On MacOS/Linux:
     ```
     export FLASK_APP=run.py
     ```
7. Create database:
   ```
   flask shell
  
   db.create_all()
   
   quit()
   ```

9. To run and use the application locally, follow the steps above and execute this command:

```
python app.py
```


