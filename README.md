🕵️‍♂️ Task 4 – Web Scraping with Jsoup

This project demonstrates how to fetch data from a website, parse its HTML, extract useful information, and save it into a CSV file for later use.

🔹 Steps Involved
🌐 1. Fetch Website

The program uses the Jsoup library to send a request to a website.

Jsoup downloads the HTML code of the target page.

Example: If the website contains product listings, Jsoup pulls all that raw HTML.

🧩 2. Parse HTML

The raw HTML is not easy to work with.

Jsoup parses the HTML and converts it into a structured Document object.

This allows us to navigate through tags (<div>, <span>, <a>, etc.) easily.

🔎 3. Extract Data

Using CSS selectors or tag names, we grab only the required information.

Example:

📦 Product Name → inside <h2> tags

💰 Price → inside <span class="price">

⭐ Rating → inside <div class="rating">

This step turns messy HTML into clean Java variables.

📄 4. Save to CSV

After extracting the required fields, the program writes them into a CSV file.

CSV (Comma-Separated Values) is a simple file format supported by Excel, Google Sheets, etc.

Each row in the CSV represents one item/product.

Example:

Name, Price, Rating
Product A, ₹999, 4.5
Product B, ₹599, 4.0

⚒️ Tools & Libraries

Java – Core programming language

Jsoup – HTML parsing & web scraping library

FileWriter – For writing extracted data into a CSV file

🚀 How to Run

Download and add jsoup-x.x.x.jar to your project (lib/ folder).

Compile and run the Java program:

javac -cp ".;lib/jsoup-1.17.2.jar" Task04.java
java -cp ".;lib/jsoup-1.17.2.jar" Task04


Check the generated output.csv file for your scraped data.