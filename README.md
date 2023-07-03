# SOA
This repository contains all the necessary files and source code required to repeat the proof of concept evaluation of our service oriented architecture for discovering and accessing prediction methods

Populate the LPG in Neo4j with prediction methods information:
***************************************************************
1. To start, download and install Neo4j Desktop, with version 1.4.2 being the recommended version.
2. Upon launching the interface, you will need to provide a username (typically set as neo4j) and password.
3. Next, create a new DBMS by selecting a name and a password.
4. Open the 'graph test example.txt' file and execute all the Cypher queries included in the file using Neo4j, which will create a complete graph.
5. Verify that the graph was successfully created by running the Cypher query 'match (n) return (n)', which should show 61 nodes and 96 relationships.

Run the Python application to discover and invoke prediction REST APIs:
******************************************************************************

1. Open the 'service matching code.zip' folder using Pycharm or any other compatible editor.
2. Open the 'authenticationParameters.py' file and change the authentication parameters by your username and password.
2. Locate the main.py file and modify the service characteristics (lines 10 to 16) to match your search criteria. Save the changes and run the page.
Note: before running this page you should start you DBMS where the prediction property graph is stored. This is required to allow the Python application to execute the constructed Cypher query over the graph.
3. The console will display the constructed Cypher query, along with a list of available and discovered services, their characteristics, inputs, outputs, and parameters.
4. Select the desired service ID from the list.
5. The corresponding URL for the selected service will be displayed.

Invoke the REST APIs:
******************************************************************************
The three implemented REST APIs code as well as the required instruction for downloading the project and calling the REST APIs could be found in the following link: 
https://github.com/ralphbn1995/Web-Service-Oriented-Architecture-for-Discovering-and-Accessing-Predictive-Methods-

