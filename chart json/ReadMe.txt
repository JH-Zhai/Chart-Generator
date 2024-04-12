This project was created by Zhai Jia Hong. https://github.com/JH-Zhai

Feel free to contribute to this project.

This project is open-source and free to use. You are welcome to modify and distribute it.

GLHF

This program generates JSON raw data from an xlsx file and then generates a relational graph from the JSON file.

data.xlsx is the sample data table.
The node sheet records node information. The node ID length cannot exceed 12 characters, otherwise bugs may occur. The shape options include circle, rectangle, roundRect, diamond, and pin. Note is the annotation information for the node, leave it blank if there is no annotation.
The edge sheet records relationship information, representing the arrows in the relational graph. The size is uniformly set to 3. Note is the annotation information for the arrow, leave it blank if there is no annotation.

generator.py is responsible for generating the JSON file.
Make sure generator.py and data.xlsx are in the same folder.
Installing dependencies may be required for the first run of generator.py.
After running, it generates the data.json file.

Place the data.json file in the graph_generator folder.

Open graph.html in a browser.

Note that when running graph.html locally, it may remain in a loading state, and CORS policy interception may be visible in the browser console.
Three possible solutions are: 1. Host the JSON file online (most direct, but requires a server) 2. Install the Allow-Control-Allow-Origin plugin 3. Use the http-server program on MacOS to generate a local proxy, and similar functionality on Windows.