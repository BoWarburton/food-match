# food-match
Food database machine learning
Food items, items that are usually sold in stores.
## Dataset A
### Fields
- UPC Code (UID)
- Description
- Food Category (not always accurate and sometimes missing)
- Ingredients
- Serving Size (in text)
### URL
The base data I am using is from here:  https://fdc.nal.usda.gov/  I am only using the branded food data portion.  Approximately 300k items.  There are some duplicates.  I have this data in DB format and deduped already

Now each Food item belongs to an "FDA" (RACC) category.  This differs from "Food Category" above.
https://www.fda.gov/media/102587/download -> I have this data in DB format but this is for reference.

## Dataset B
### Fields
- UID
- FDA Main Category
- FDA Sub Category
- Product Examples
- RACC Amount (usually in grams)
## Goals
So for an item in DATA SET A I need to find which category (about 182 categories) it falls into in DATA SET B.
I have hand mapped these using a variety of methods.
My goals for this are:
1. Create a predictive algorithm so when I add new items in it can predict the correct FDA/RACC category an item belongs.
2. Back test the currently assigned items and predict where there is a mistake
3. If possible use the Microsoft ML.Net machine learning framework.
That is it on a high level.  Let me know where the questions are.
Rob Combis
Senior Technology Consultant
rcombis@ensatina.com
203.820.9016
