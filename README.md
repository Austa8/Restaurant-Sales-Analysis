# Restaurant-Sales-Analysis

## Project Overview
This project aims to analyze the sales performance of a restaurant within a timeframe based on certain criteria like category of menu cuisines, to provide data driven solution for business decisions. 

## Business Model
- Research:
We based our research on the total number of items on the menu, based on the various categories, time trends, the least and most ordered item.
- Abstract:
We believe that data driven solutions can greatly improve the bedrock of any business and so, it should be treated with integrity.
- Design:
The tools used for this analysis are, MySQL, PowerPoint and Tableau for visualization.

## Business Questions
1. What were the least and most ordered items? What categories were they in?
   
2.What do the highest spend orders look like? Which items did they buy and how much did they spend?

3. Were there certain times that had more or less orders?

4. Which cuisines should we focus on developing more menu items for based on the data?

## Tools
- Excel
- MySQL
- Tableau

## Source Data
### Order Table

<img width="485" alt="Screen Shot 2024-06-02 at 7 02 53 PM" src="https://github.com/Austa8/Restaurant-Sales-Analysis/assets/142371168/86a0eac9-93bc-422e-b78e-48802f595a59">

### Menu Table

<img width="384" alt="Screen Shot 2024-06-02 at 7 27 52 PM" src="https://github.com/Austa8/Restaurant-Sales-Analysis/assets/142371168/8ea4b13b-b737-4748-a6b2-a2e18da57cd3">



## MySQL Script and Output

```
-- 2. What are the least and most expensive items on the menu
{
SELECT item_name, price FROM menu_items
WHERE price = (SELECT MIN(price) FROM menu_items)
OR price = (SELECT MAX(price) FROM menu_items);
}
```
(<img width="389" alt="Screen Shot 2024-06-02 at 6 51 46 PM" src="https://github.com/Austa8/Restaurant-Sales-Analysis/assets/142371168/8a4a89cf-bcb8-465a-920f-b7d954c6a96a">)
