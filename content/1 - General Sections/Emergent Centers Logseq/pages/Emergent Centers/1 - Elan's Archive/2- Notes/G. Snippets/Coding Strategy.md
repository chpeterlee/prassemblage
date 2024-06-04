> 1. Every Snippet or Task becomes a Module
>		1. Each snippet has an outlet to MongoDB
> 		1. Define a checking function to wrap it. 
> 2. Define Modules as functional building blocks for Rock Paper Scissors Recipes. 	
> 3. Have 3 Tier (double-ended) meta-transformation recipes.

Output to MongoDB Collection? >>> Check the outputs.
Recipes of 3 or more blocks. >>> Export a Combo.
	- Building Block Compiled (.js) >>> Export a combo.
		- Snippet + Snippet + Snippet. >>> Export all.
				- Snippets
					- Stable
					- Sketches

----
# Export Procedure:

**Filename: cal.js**
	`function` `sum(x, y) {`
	
	    `return` `(x + y);`
	
	`}`
	
	`function` `sub(x, y) {`
	
	    `return` `(x - y);`
	
	`}`
	
	`function` `mul(x, y) {`
	
	    `return` `(x * y);`
	
	`}`
	
	`module.exports = { add, sub, mul, div };`

----

**Use the Functions**
	`//requiring cal.js file`
	
	`const cal = require(``"./cal.js"``)`  
	
	`//Using the functions from cal.js` 
	
	`const sum = cal.sum(2, 2);`
	
	`console.log(sum);` 
	
	`const sub = cal.sub(10, 5);`
	
	`console.log(sub);` 
	
	`const product = cal.mul(2, 3);`
	
	`console.log(product);`


-----

1. Standardize a function template
2. 3 layers of loops with variables to chop in and out.
3. Export the functions.
----
1. Initiate Scripts | Boot-up Scripts
2. Refresh Scripts | Loop & Monitor Scripts
3. Run Scripts | Run on Condition Scripts
4. Log Scripts | Monitor Scripts
5. Self-Healing | Flip Switches Scripts

