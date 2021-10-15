# web-scraping-challenge
In this assignment, you will build a web application that scrapes various websites for data related to the Mission to Mars and displays the information in a single HTML page. The following outlines what you need to do.

A Flask application created by web scraping the latest Mars news, facts, and images and storing in/pulling from a Mongo database.

# Contents

/Mission_to_Mars
/templates: contains template HTML file for Flask application
app.py: Flask application
mission_to_mars.ipynb: web scraping Mars news, facts, and images in Jupyter Notebook from various websites
scrape_mars.py: web scraping in Python function form for use in Flask application
Description

The latest Mars news, facts, and space images are continually updated. To keep up with that, a web scraping script was created using BeautifulSoup and Splinter in Python. The resulting contents are summarized in a Flask application webpage in this project.

The following websites were scraped and data obtained:

NASA Mars News Site: latest Mars News Title and associated Paragraph Text
JPL Featured Space Image: image url for the current Featured Mars Image
Mars Weather twitter account: latest Mars weather tweet
Mars Facts webpage: facts table about the Mars including Diameter, Mass, etc.
USGS Astrogeology site: high resolution images for each of Mar's hemispheres
This data was then stored in a MongoDB collection. This collection is accessed in a Flask app and HTML template (using Jinja) to create the resulting webpage:
