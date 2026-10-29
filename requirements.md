## Console (one customer)
Customer c101 (Wanjiru) bought: {p04, p08}
Most similar customers:
  c117  jaccard=0.50
  c109  jaccard=0.33
  c113  jaccard=0.17
Recommendations:
  1. Festive Bread (Bakery)  score=0.533  because 3 similar customers bought it
  2. Pampers Size 3 (Baby)  score=0.502  because 1 similar customer bought it
  3. Kienyeji Eggs (tray) (Fresh)  score=0.255  because 1 similar customer bought it

## output/recommendations.csv
customer_id,customer_name,rank,product_id,product_name,category,score,supporting_customers
c101,Wanjiru,1,p03,Festive Bread,Bakery,0.533,c117;c109;c113
c101,Wanjiru,2,p10,Pampers Size 3,Baby,0.502,c117
c101,Wanjiru,3,p01,Kienyeji Eggs (tray),Fresh,0.255,c113
c102,Otieno,1,p07,Royco Mchuzi Mix,Pantry,0.562,c114
...
c107,Chebet,,,,,,
...
# One row per (customer, rank). Customers with no possible recommendation still appear
# once with blank product columns, so nobody silently disappears from the file.

## Run summary
Purchases read: 63 | used: 61 | rejected: 2
Customers: 20 | Products: 15 | Recommendations written: 43
