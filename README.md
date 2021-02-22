# Thank you for your interest in CO 
This is a small problem that we would like you to solve so that we can get an idea of your coding ability. Your submission will be run in a clean environment to see if it produces the expected output. Please be sure to provide instructions for installing any dependencies. 

### What we look for 
We will be looking at the quality and professionalism of your work. In particular we look for clean, well-designed (OBJECT-ORIENTED DESIGN), maintainable code. Although this is a rather small task, it should be approached as you would an actual task for a customer. 

### When you are finished 
Please zip and send the entire directory including the .git folder. 

# The Problem 
We want you to create a command-line application that will  updates the price of products of our business unit, Car Insurance, based on rules explained bellow.

### Input/output 
The input can be text or CSV. The output will be text.
Your solution should parse the provided sample-input.txt file via stdin (pipe or redirect) or by parsing a file passed by name on the command line. That will be the initial status of the prices of the products and the remaining days.
Your solution should output the correct result via stdout to the console.
The input contains information about different products, one per line. 

Here you have a description of the products:
- All Products have a sellIn value which denotes the number of days we have to sell the product.
- All Products have a price value which denotes how much the product cost.
- At the end of each day our system lowers both values for every product.

See sample-input.txt for details. 
The output should be the result of each daily iteration where prices are updated, ordered from day zero, following the format specified in expected-output.txt.

A daily price update process for 30 days could be considered.

You can expect that the input will be well-formed. There is no need to add special handling for malformed input files.

### The rules 
- Once the sell by date has passed, price degrades twice as fast.
- The price of a product is never negative.
- "Full Coverage" actually increases in price the older it gets.
- The price of a product is never more than 50.
- "Mega Coverage", being a legendary product, never has to be sold or decreases in price.
- "Special Full Coverage", like full coverage, increases in price as its sellIn value approaches:
a) price increases by 2 when there are 10 days or less and by 3 when there are 5 days or less but.
b) price drops to 0 when no more days left (and the product is not valid anymore).
- "Super Sale" Products degrade in price twice as fast as normal Products.
- Just for clarification, a product can never have its price increase above 50, however "Mega Coverage" is a legendary product and as such its price is 80 and it never alters.

### Guidelines 
This should be implemented in a language with which you are familiar. We strongly prefer that you use ruby. 
Your solution should be able to be run (and if applicable, built) from the command line. Please include appropriate scripts and instructions for running your application and your tests. 
If you use other libraries installed by rubygems/bundler it is not necessary to commit the installed packages. 
We write automated tests and we would like you to do so as well. 
We appreciate well factored, object-oriented or functional designs. 
Please document any steps necessary to run your solution and your tests. 

### Platform support 
This will be run in a unix-ish environment (OS X). 
### Questions? 
Please email lecheverri@comparaonline.com  if you have any questions