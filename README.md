# Jumia Product Performance Analysis

Excel-based exploratory analysis of **109 products** listed on Jumia, focusing on pricing, discounts, ratings, and customer engagement (reviews).

## Overview

This project examines relationships between:

- Current price vs. old price and discount depth  
- Product ratings and review volume  
- Discount category (Low / Medium / High) and customer response  

The goal is to surface pricing and promotion patterns that correlate with better ratings and higher engagement.

## Dataset Summary

| Metric | Value |
|--------|-------|
| Total products | 109 |
| Total reviews | 723 |
| Average current price | ~1,208 |
| Average old price | ~1,838 |
| Average discount | ~36.4% |
| Average rating | ~3.89 / 5 |

### Price extremes
- **Least expensive:** 3PCS Single Head Knitting Crochet Sweater Needle Set — **38**
- **Most expensive:** 32PCS Portable Cordless Drill Set With Cyclic Battery Drive — **3,750**

## Key Findings

### 1. Ratings by discount category
| Discount Category | Avg Rating | Avg Reviews | Product Count |
|-------------------|------------|-------------|---------------|
| Medium Discount   | **4.17**   | ~10.9       | 31            |
| Low Discount      | 3.87       | ~2.6        | 19            |
| High Discount     | 3.75       | ~5.7        | 59            |

**Insight:** Medium-discount products earn the highest average ratings and the strongest review engagement. Deep discounts do not automatically translate into better ratings or more reviews.

### 2. Rating distribution
| Rating Category | Count |
|-----------------|-------|
| Excellent       | 23    |
| Average         | 69    |
| Below Average   | 17    |

### 3. Discount vs. review volume
Higher discount bands (especially 0.41–0.51) contain the largest number of products that received reviews. However, the relationship is not strictly linear — medium discounts still show stronger average engagement per product.

### 4. Rating vs. review volume
| Rating Band | Total Reviews |
|-------------|---------------|
| 4–5         | 485           |
| 2–3         | 169           |
| 3–4         | 69            |

Higher-rated products attract the large majority of reviews.

### 5. Notable products

**Top products by reviews**
- 120W Cordless Vacuum Cleaners Handheld Electric Vacuum Cleaner — 69 reviews  
- 137 Pieces Cake Decorating Tool Set Baking Supplies — 55 reviews  
- Electronic Digital Display Vernier Caliper — 49 reviews  

**Highest-rated (5.0)** examples  
- Anti-Skid Absorbent Insulation Coaster  
- Bedroom Simple Floor Hanging Clothes Rack  
- Classic Black Cat Cotton Hemp Pillow Case  
- Konka Healthy Electric Kettle  
- LASA Aluminum Folding Truck Hand Cart  

**Lowest-rated** examples  
- Wall-mounted Sticker Punch-free Plug Fixer — 2.0  
- 5-PCS Stainless Steel Cooking Pot Set — 2.1  
- Electric LED UV Mosquito Killer Lamp — 2.1  

## Workbook Structure

The Excel file contains multiple analysis sheets / pivot views, including:

- Overall averages (price, discount, rating)
- Most & least expensive products
- Average rating by discount category
- Product distribution by rating category
- Relationship between discount % and number of reviews
- Relationship between rating and number of reviews
- Discount category vs. review flag
- Top 10 highest-discount products
- Top 10 most-reviewed products
- Top 5 / Bottom 5 rated products
- High- vs low-discount comparison
- Full product-level data table (`Excel_jumia`) with calculated fields:
  - Discount amount
  - Rating Category
  - Discount Category
  - Price Flag (Least / Most Expensive)

## How to Use

1. Open `jumia Product Performance.xlsx` in Microsoft Excel, Google Sheets, or LibreOffice Calc.
2. Explore the pivot tables and summary sheets for the insights above.
3. Filter or sort the main product table (`Excel_jumia`) by rating, discount, or review count for deeper investigation.
4. Extend the analysis by adding new products or recalculating categories as needed.

## Suggested Next Steps

- Segment by product category (home, tools, kitchen, etc.) if category data becomes available.
- Test whether medium-discount products also convert better (sales volume) once sales data is added.
- Build a simple dashboard (Power BI / Tableau / Excel dashboard) from the existing pivots.
- Track the same products over time to measure rating and review growth after discount changes.

## License

This project is provided for portfolio / educational use. Product names and figures are derived from public listing data and are used for analytical demonstration only.

---

**File:** `jumia Product Performance.xlsx`
