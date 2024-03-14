

```dataview
TABLE
	title as Title,   
	Author as "Author",   
	Year as Year,  
	itemType as Item,   
	Citekey as Citekey,   
	Smoothing as Smoothing,
	Contribution as Contribution
FROM "200_References/papers" AND #functional-data-analysis
SORT Smoothing, Year
```
 