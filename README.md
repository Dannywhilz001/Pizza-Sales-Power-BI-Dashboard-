# 🍕 Pizza Sales Power BI Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-success?style=for-the-badge)

> Comprehensive sales analytics dashboard for pizza restaurant chain performance analysis

## 📊 Overview

This Power BI project provides detailed analysis of pizza sales performance across 2025, delivering actionable insights into revenue patterns, customer behavior, and product performance. The dashboard enables data-driven decision-making for restaurant operations and marketing strategies.

### **Key Metrics:**
- 💰 **Total Revenue**: $817.86K
- 🍕 **Total Pizzas Sold**: 50K
- 📦 **Total Orders**: 21K
- 📊 **Avg Pizza Per Order**: 2.32
- 💵 **Avg Order Value**: $38.31

## 📸 Dashboard Pages

### Page 1: Product Performance
![Product Performance](https://ibb.co/q3nMJgpb)
- Top 5 & Bottom 5 pizzas by revenue, quantity, and orders
- Performance comparison across all metrics

### Page 2: Sales Trends & Patterns
![Sales Trends](https://ibb.co/ZRKjMX1n)
- Monthly and quarterly order trends
- Sales distribution by category and size
- Temporal pattern analysis

## ✨ Key Insights

### **Busiest Days & Times**
📅 **Days**: Orders peak on **weekends** (Friday/Saturday evenings)
📆 **Monthly**: Maximum orders occur in **July and January**

### **Product Performance**

**Top 5 Pizzas by Revenue:**
1. The Thai Chicken - $43K
2. The Barbecue Chicken - $43K
3. The California Chicken - $41K
4. The Classic Deluxe - $38K
5. The Spicy Italian - $35K

**Bottom 5 Pizzas by Revenue:**
1. The Brie Carre - $12K
2. The Green Garden - $14K
3. The Spinach (multiple varieties) - $15-16K
4. The Mediterranean - $15K

### **Category Analysis**
- **Classic**: 26.91% of sales, 15K pizzas
- **Supreme**: 25.46% of sales, 12K pizzas
- **Chicken**: 23.96% of sales, 11K pizzas
- **Veggie**: 23.68% of sales, 12K pizzas

### **Size Distribution**
- **Large (L)**: 45.89% - Most popular
- **Medium (M)**: 30.49%
- **Small (S)**: 21.77%
- **XL/XXL**: 1.72% combined - Least ordered

### **Quarterly Trends**
- Q1 & Q2: Steady ~5,200-5,400 orders
- Q3: Peak performance
- Q4: Decline to ~5,000 orders

## 🎯 Business Recommendations

1. **Staff Optimization**: Increase staffing on weekends and Friday/Saturday evenings
2. **Menu Optimization**: Consider removing or repositioning bottom 5 performers
3. **Promotional Focus**: 
   - Push large size pizzas (highest demand)
   - Create combo deals for slow months (September-December)
   - Promote XL/XXL sizes with special offers
4. **Seasonal Campaigns**: Leverage July and January peaks with targeted marketing
5. **Category Balance**: Classic and Supreme categories drive revenue - maintain quality

## 🛠️ Features

### **Interactive Elements:**
- 📅 Date range filters (customizable start/end dates)
- 🏷️ Price/Pizza category slicers
- 📊 Cross-filtering across all visuals
- 🎯 Dynamic KPI cards

### **Visualizations:**
- Horizontal bar charts for product rankings
- Column charts for monthly trends
- Area charts for quarterly performance
- Donut charts for category/size distribution
- Custom KPI cards with icons

### **Advanced DAX Measures:**
- Total Revenue calculation
- Average order value
- Pizzas per order ratio
- Top/Bottom N rankings
- Month-over-month growth
- Category percentage calculations
- Size distribution analysis

## 💻 Tech Stack

- **Power BI Desktop** - Dashboard creation
- **DAX** - Calculated measures and KPIs
- **Power Query** - Data transformation
- **Data Modeling** - Relationships and hierarchies

## 📂 Repository Structure
```
```

## 🚀 How to Use

### **Prerequisites:**
- Power BI Desktop ([Download](https://powerbi.microsoft.com))

### **Setup:**

1. Clone the repository:
```bash
git clone https://github.com/Dannywhilz001/pizza-sales-powerbi-dashboard.git
   
```

2. Open `Pizza_Sales_Reports.pbix` in Power BI Desktop

3. Refresh data if needed (Home → Refresh)

4. Use filters to explore:
   - Select date ranges
   - Filter by pizza/price category
   - Click visuals for cross-filtering

## 📊 DAX Measures
```dax
Total Revenue = SUM(Orders[Revenue])

Total Orders = COUNT(Orders[Order_ID])

Total Pizzas Sold = SUM(Orders[Quantity])

Avg Pizza Per Order = 
DIVIDE([Total Pizzas Sold], [Total Orders], 0)

Avg Order Value = 
DIVIDE([Total Revenue], [Total Orders], 0)

Top 5 Revenue = 
CALCULATE(
    [Total Revenue],
    TOPN(5, ALL(Pizza[Name]), [Total Revenue], DESC)
)
```

## 📈 Use Cases

- 🍕 **Restaurant Management**: Optimize menu and operations
- 📊 **Portfolio Project**: Showcase BI skills
- 🎓 **Learning**: Study sales analytics techniques
- 💼 **Business Analysis**: Template for retail analytics

## 🤝 Contributing

Contributions welcome! Please fork and submit pull requests.

## 📄 License

MIT License - feel free to use for learning and portfolio purposes.

## 👤 Author

**[Oladotun Olawale]**
- LinkedIn: [http://www.linkedin.com/in/oladotun-olawale]
- Portfolio: [https://github.com/Dannywhilz001]
- Email: oladotunolawale29@yahoo.com

## 🌟 Acknowledgments

- Dashboard design inspired by restaurant analytics best practices
- Power BI community for DAX optimization techniques

---

⭐ **If you find this helpful, please star the repo!**

📧 **Questions?** Open an issue or connect on LinkedIn
```


- Setup instructions and usage guide
- Business recommendations based on analysis
