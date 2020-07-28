# NZPowerBi
My pick for the Power BI final project was “environmental protection expenditure account by 2009-18” dataset. <br/>
  In general, Environmental  protection expenditure term used to describe all goods and services aimed at protecting the environment and  <br/> encourage 
the sustainable use of natural resources. I am close to this topic, and one of citizens who cares about the environment. And my first thought was <br/>
that analyzing New Zealand, could be a good example of how to save the environment for future generation.
Hypothesis and what I expected 
When I started Data cleaning part, I was interested in 6 unique parameters in class column.  
It consisted from Total, Wastewater, Solid waste/refuse, Air and water quality, Flood, river, land, Pest management includes both animal and plant.
And let me explain each of them individual.
-	Wastewater reticulation of sewage, sewerage treatment: oxidation ponds and on land disposal, stormwater (the water that runs off surfaces such as roads, driveways, 
footpaths, and rooftops).
-	Solid waste/refuse includes collection and disposal.
-	Air and water quality includes any measurement and analysis of air and/or water quality and education. Also includes dairy effluent.
-	Flood, river, land and soil management.
-	Pest management includes both animal and plant. Pests are defined as organisms that serious adverse and unintended effect on people and/or the environment.
-	Total – I guess it to identify all possible source of environmental pollution.

And my hypothesis was that Air and Water quality is major priority for New Zealand. And they will spend most of their money on it. 
Next hypothesis was based on sector column. 
This column had Local, General and Central government parameters. My hypothesis was in that General government spend the most money on Environmental protection. 
This hypothesis in comparison with previous was based on the reading about New Zealand Government system. I found out that General Government comprises the New Zealand Treasury 
and other central and local government entities. Which means that their in charge for everything. 
Central government and General government made every year the same amount of investment, and its 6 times. However Local Government made it 26 times every year, 
but Local has only 10% of budget ever made in this country. 
To summarize columns I used DAX formula: 
Dax budget by year = SUMMARIZECOLUMNS('environmental protection'[year];'environmental protection'[budget])
This formula gave me opportunity to use these two columns separately. 
Moreover, I made another three metrics 
•	Budget Local = SUMX(FILTER('environmental protection';'environmental protection'[sector]="Local Government"); 'environmental protection'[budget])
•	Budget General = SUMX(FILTER('environmental protection';'environmental protection'[sector]="General government"); 'environmental protection'[budget])
•	Budget Central = SUMX(FILTER('environmental protection';'environmental protection'[sector]="Central government");'environmental protection'[budget])

And thanks to these, I Could find out how much money they spend on environment in separate years. 
Environment plays an important role in the healthy living of human beings. it matters because it is the only home that animals have, and it provides air, food, 
and other needs. Each country is responsible for its nature and must allocate money to preserve it.

