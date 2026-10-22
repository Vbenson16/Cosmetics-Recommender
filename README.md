# Cosmetics-Recommender# Chemical Content-Based Cosmetics Recommendation System
**MedTourEasy Traineeship · March 2026**

*Guided project (DataCamp), completed as part of the MedTourEasy traineeship. I wrote the code for each task; the project structure and instructions were provided.*

**Tools:** Python, Pandas, NumPy, Scikit-Learn (t-SNE), Bokeh

A content-based recommender that maps Sephora products by their ingredients, so users can find products with a similar chemical makeup to ones they already like.

## Data
- 1,472 Sephora products across 6 categories (moisturizer, cleanser, face mask, treatment, eye cream, sun protection) and 5 skin types
- Focus for this analysis: **190 moisturizers for dry skin**

## Approach
- Split each product's ingredient list into tokens (2,233 unique ingredients)
- Built a product × ingredient matrix (190 × 2,233) with one-hot encoding
- Reduced it to 2 dimensions with **t-SNE**: products close together have similar ingredients
- Built an interactive **Bokeh** scatter plot with hover details (name, brand, price, rating)

## Key result
Two products that sit close together on the map have very similar ingredients:

| Product | Brand | Price | Rating |
|---|---|---|---|
| Color Control Cushion Compact SPF 50+ | AmorePacific | $60 | 4.0 |
| BB Cushion Hydra Radiance SPF 50 | Laneige | $38 | 4.3 |

The Laneige product is **37% cheaper** and **rated higher**. That's a useful alternative for the same skin needs.

## Files
- [Cos_rec_notebooks_final.ipynb](Cos_rec_notebooks_final.ipynb): full analysis
- [Project report (PDF)](Data%20Science%20Final%20Project-%20Cosmetics%20PDF%20F.pdf)
