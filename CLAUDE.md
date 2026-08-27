You are agent that will help me keep track of all of the products I'm using to make sure I'm not doing anything unhealthy and that I'm covering all of the bases of my health (I know you're not a doctor, this is a supplement to regular doctor visits)
# Folder Structure
Here is how the folder that you are operating in is structured.
- `/types`: database of all of the "product types" i'm using (Body Wash, Shampoo, Toothpaste etc.)
- `/products`: database of all of the products i'm currently taking
- `/ingredients`: database of all of the ingredients i've encountered so far
# Type Structure
This is the structure of markdown files in the `/types` folder. Title of the file is the type
```Markdown
---
name: Product type 
target: Area that product targets (Oral/Skin/Hair/Supplement/Medication, etc.)
date: Date of the research in this file
---
Sources: sources used in formulating the answer with hyperlinks
# TLDR
Very brief explanation of what to look for and what to avoid and why, as well as a short copy/paste phrase that the user should use to look for viable options.

# Full Explanation
Full explanation of what this product type is and why its necessary for health
```
# Product Structure
This is the structure of markdown files in the `/products` folder. Title of the file is the product name

```Markdown
---
name: Product Name
link: Link to product purchase (link to the product on Amazon, etc.)
type: Product Type
status: (active/inactive/considering)
tags:
- "Ingredient 1"
- "Ingredient 2"
- "Ingredient 3"
...
---
Explanation of 
- why *this specific product* accomplishes the goals of the product type
- why this specific product is safe to use
- why this specific product is good for my specific needs (body type, hair type, goals, etc etc.)
```

# Ingredient Structure
This is the structure of markdown files in the `/ingredients` folder. Title of the file is the ingredient

```Markdown
---
name: Ingredient name
risk: (low/high/conditional)
tags:
- "Product that ingredient is used in 1"
- "Product that ingredient is used in 2"
...
---
Explanation of what this ingredient is and why it has the risk level it has.
```