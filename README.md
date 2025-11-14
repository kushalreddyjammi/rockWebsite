# RockMarket - Simple HTML Website

A simple, clean HTML website for browsing and displaying rocks. Data is fetched from a JSON file.

## Features

- Pure HTML, CSS, and JavaScript (no frameworks)
- Fetches product data from `products.json`
- Search and filter functionality
- Responsive design
- Modern, clean UI

## Files

- `index.html` - Main HTML page
- `styles.css` - All styling
- `products.json` - Product data in JSON format

## How to Use

1. Open `index.html` in a web browser
2. The page will automatically load products from `products.json`
3. Use the search and filter options to find specific rocks

## Note

If you're opening the file directly (file://), you may need to run a local server due to CORS restrictions when fetching JSON. You can use:

```bash
# Python 3
python -m http.server 8000

# Node.js (with http-server)
npx http-server

# Then open http://localhost:8000
```

## Product Data Structure

The `products.json` file contains an array of products with the following structure:

```json
{
  "products": [
    {
      "id": 1,
      "name": "Product Name",
      "description": "Product description",
      "category": "Category",
      "price": 45.99,
      "currency": "USD",
      "image_url": "URL or path to image",
      "stock_quantity": 15,
      "weight_kg": 0.5,
      "dimensions": "10cm x 8cm",
      "origin_country": "Country",
      "company_name": "Seller Name"
    }
  ]
}
```

