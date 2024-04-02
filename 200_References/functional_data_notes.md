

```dataview
TABLE
	title as Title,   
	Author as Author,
	Year as Year,  
	itemType as Item,   
	Citekey as Citekey,
	Aim as Aim,
	Type as Type,
	Dependency as Dependence,
	Smoothing as Smoothing,
	Contribution as Contribution
FROM "200_References/papers" AND #functional-data-analysis
SORT Year
```
 