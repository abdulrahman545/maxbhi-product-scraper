# Maxbhi.com Scraper

This is a scraper designed to extract data from the online marketplace Maxbhi.com, specializing in electronics, spare parts, tools, solar products, and more. The scraper is built in two stages to gather information about various products and store them in a structured format.

## Stage 1: Scraping Product Links

In this stage, the scraper collects all the product links available on Maxbhi.com and stores them in a file named `product_links.csv`. This file will be used as input for the next stage of the scraping process.

To run Stage 1, follow these steps:

1. Activate the virtual environment by running the command:
```bash
source bin/activate
```

3. Install the required dependencies by running(if you are not using a virtual environment):
```bash
pip install -r req.txt
```

5. Run the command:
   
```bash
python products_url_scraper.py
```
This will initiate the scraping process and generate the `product_links.csv` file.

## Stage 2: Scraping Product Information

In this stage, the scraper utilizes the `product_links.csv` file generated in Stage 1 to extract detailed information about each product. The collected data includes:

- Product Title (string)
- Product Image URLs (list of string URLs)
- Product Description (string)
- Product Price (string)
- Product Stock (boolean indicating whether the product is in stock or out of stock)
- Product Code (string)
- Device Type (string)
- Device Category (string)

To run Stage 2, ensure that you have the `product_links.csv` file in the same directory. Make sure you have completed Stage 1 before running this stage. Follow these steps:


1. Run the command:
  ```bash
python product_info_scraper.py
```
This will execute the scraping process using the `product_links.csv` file and generate an `out.csv` file as the final output.

Please note that this project does not currently allow for input parameters or advanced search options. If you require further filtration or specific search results, please contact the owner at gautamnegi0202@protonmail.com.

## Contributions

Contributions to this project are welcome! If you would like to contribute, please follow the guidelines provided by the owner. Feel free to reach out to the owner at gautamnegi0202@protonmail.com to discuss potential contributions and improvements to the Maxbhi.com scraper.

## Additional Information

- This scraper is designed to scrape data from over 1,438,000 products available on Maxbhi.com.

## License

This project is licensed under the MIT License. Please see the [LICENSE](LICENSE) file for more information.

