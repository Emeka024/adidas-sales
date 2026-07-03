# Adidas Sales Data Analysis

## Project Overview
This project explores the **Adidas Sales Dataset** to uncover trends, patterns, and insights related to Adidas product sales across different regions in the United States. The analysis uses Python for data cleaning and visualisation, with a focus on understanding what drives revenue and profitability across regions, products, and sales channels.

---

## Dataset
The dataset contains transactional sales data for Adidas products across multiple U.S. regions. Each row represents a single sales transaction with the following columns:

| Column | Description |
|---|---|
| `Retailer` | Name of the retailer |
| `Retailer ID` | Unique ID assigned to each retailer |
| `Invoice Date` | Date of the sales invoice |
| `Region` | Region where the sale took place |
| `State` | State within the region |
| `City` | City where the sale occurred |
| `Product` | Name of the Adidas product sold |
| `Price per Unit` | Price per unit of the product |
| `Units Sold` | Quantity of units sold |
| `Total Sales` | Total sales amount for the transaction |
| `Operating Profit` | Profit generated from the sale |
| `Operating Margin` | Profit margin for the transaction |
| `Sales Method` | Method used for the sales transaction (In-store / Outlet / Online) |

---

## Setup & Installation

### Prerequisites
- Python 3.x
- VS Code with the Jupyter extension

### Steps

1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/adidas-sales.git
   cd adidas-sales
   ```

2. Create and activate a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate   # Mac/Linux
   venv\Scripts\activate      # Windows
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Open the notebook:
   - Launch VS Code in the project folder: `code .`
   - Open `analysis.ipynb`
   - Select the `venv` Python interpreter when prompted

---

## Project Structure

```
adidas-sales/
├── Adidas Sales Dataset.csv   # Raw dataset
├── analysis.ipynb             # Main Jupyter notebook with all analysis
├── requirements.txt           # Project dependencies
└── README.md                  # This file
```

---

## Analysis & Key Findings

### 1. Sales Trend by Region
A line chart was used to compare total sales across the five U.S. regions. The **West region leads in total sales**, followed by the **Northeast**. The **South and Midwest regions** recorded the lowest total sales figures.

### 2. Products Sold by Volume
A horizontal bar chart was used to compare units sold per product type. **Men's Street Footwear** is the top-selling product by volume, followed by **Women's Apparel** and **Men's Athletic Footwear**. **Men's Apparel** and **Women's Athletic Footwear** are the lowest-selling categories.

### 3. Price per Unit vs. Operating Profit
A scatter plot was used to explore the relationship between price and profitability. Products priced between **$45 and $65** — predominantly **Men's Street Footwear** — generate both the highest sales volume and the highest operating profit, suggesting a sweet spot in pricing strategy.

### 4. Operating Margin by Sales Method
A box plot was used to compare operating margin distributions across the three sales methods. **Online sales** generate the highest operating margins, with a significant portion reaching **70–80%**. **In-store** sales are more consistent but plateau around 40–50%. **Outlet** sales show the most variability, with some transactions achieving high margins and others performing poorly.

---

## Tools & Libraries

- **pandas** — data loading, cleaning, and transformation
- **matplotlib** — base plotting library
- **seaborn** — statistical visualisations (line, bar, scatter, box plots)
- **Jupyter Notebook** — interactive analysis environment

---

## Author
Chukwuemeka Okonkwo
