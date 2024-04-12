This project was created by Zhai Jia Hong. https://github.com/JH-Zhai

Feel free to contribute to this project.

This project is open-source and free to use. You are welcome to modify and distribute it.

GLHF

1. Version Introduction

	chart json: Python code, can be directly executed, fastest speed, strongest scalability, needs command-line execution. For detailed usage instructions, refer to ./chart json/ReadMe.txt.
	
	chart Windows/chart MacOS: intel-chip Mac not supported. Please use the version that suits your operating system. Click to run, no command needed.
	
2. chart Windows/chart MacOS Usage Instructions:

	The raw data file is ./dist/data.xlsx. This file serves as a template, replace it with your own data while adhering to the template format. The template can generate a simple example chart, which helps understand the usage of data.xlsx.
	
	After editing data.xlsx, run generator.exe or generator in the same folder to generate the image page. It takes about 10 seconds to generate a new chart.
	
	After generation, the image page will open automatically (MacOS defaults to using Safari browser, Windows defaults to using Edge browser). You only need to generate a chart once, afterward, you can double-click graph.html to use the chart independently (can be opened in any browser).
	
	When updating data.xlsx, a new chart will be generated in place and replace the old one. Before generating a new chart, make sure to save the old one.

3. data.xlsx Explanation:

	The node sheet in data.xlsx is for nodes, and the edge sheet is for relationships. Pay attention not to exceed 12 digits in the ID of nodes, otherwise, bugs may occur.
	
	Node Sheet:
	Pay attention not to exceed 12 digits in the ID of nodes to avoid bugs.
	The color item can use any color recognized by HTML (approximately 140+ colors), or hex color codes, see: https://htmlcolorcodes.com/.
	The shape item can be one of the following: circle, rectangle, roundRect, triangle, diamond, pin, arrow.
	The size item is self-explanatory.
	The y, x coordinates can be set arbitrarily since the node position supports mouse dragging.
	The note item is for node annotations, leave it blank if there's none.
	
	Edge Sheet:
	SourceID/targetID indicates the direction of the relationship (from which node to which node).
	The note item is for relationship annotations, leave it blank if there's none.