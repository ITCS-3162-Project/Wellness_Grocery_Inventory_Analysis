# Q1 (Column Meanings): Define each column and summarize strong correlation groups via Annotations.
Data.Carbohydrate: Amount of carbohydrates in the food
Data.Fiber: Amount of dietary fiber
Data.Kilocalories: Calories (energy content)
Data.Protein: Amount of protein
Data.Sugar: Total	Amount of sugar
Data.Water: Amount of water
Data.Fat.Saturated Fat: Amount of saturated fat
Data.Fat.Total Lipid: Total fat content

1.Kilocalories ↔ Water = -0.891
Foods with more water tend to have fewer calories.

2. Kilocalories ↔ Total Lipid = 0.806
Foods with more fat tend to have more calories.

3. Saturated Fat ↔ Total Lipid = 0.762
Foods with more total fat tend to contain more saturated fat.

# Q2 (Feature Selection): If you had to pick only 3 features to classify your inventory, which would they be? Test with a scatter plot.
The three selected features were Data.Water, Data.Fat.Total Lipid, and Data.Protein. These variables capture important nutritional differences 
among foods, including moisture content, fat content, and protein content. The scatter plot of Water versus Total Lipid shows clear separation 
between products with high water content and products with high fat content. Protein was selected as the third feature because it helps distinguish 
meats and other protein rich foods from fruits, vegetables, and sweets.

# Q3 (Outlier Detection): Identify "misfit" rows that appear misclassified and speculate on whether they are labeling errors, if applicable.
Several outlier observations were identified using a scatter plot of Data.Water versus Data.Fat.Total Lipid. Rows 631 (FAT, TURKEY), 
651 (MEAT DRIPPINGS, LARD), 714 (OIL, VEGETABLE OIL HIGH OLEIC CANOLA OIL), and 717 (MARGARINE) appeared far from the main cluster because they contain 
extremely high fat content and very little water. These rows can be considered misfit observations when compared to the majority of food products in 
the inventory. However, they do not appear to be labeling errors. Their nutritional profiles are consistent with the types of foods they represent, since 
animal fats, oil, lard, and margarine naturally contain high levels of fat and minimal water content.
