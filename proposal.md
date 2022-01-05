### **Question/need:**

- What is the framing question of your analysis, or the purpose of the model/system you plan to build?

This project answers the question: where should street performers in the NYC area perform in order to maximize the amount of foot traffic that would see their performances?

- Who benefits from exploring this question or building this model/system?

This question is specifically aimed at street performers, but it would be helpful to all who are interested in knowing which MTA stations have the most foot traffic. Street performers would be interested in knowing the most popular stations, especially during the daytime.

### **Data Description:**

- What dataset(s) do you plan to use, and how will you obtain the data?

Because these street performers are interested in performing as soon as possible, I will be using the last three months of data available at the time of the start of the project. This is especially important in that the pandemic of the last two years has changed MTA foot traffic. 

- What is an individual sample/unit of analysis in this project? What characteristics/features do you expect to work with?

One four-hour block in a turnstile of an MTA station is the individual unit of analysis. The number of turns in the turnstile, station location, date, and time will all be relevant information to this project. I expect to use the sum of entries and exits for a time slot for all turnstiles in a particular station to determine the total foot traffic in that area.

### **Tools:**

- How do you intend to meet the tools requirement of the project?

I will extract, transform, and load the raw data into DB Browser for SQLite, and then query from that database into Python via SQLAlchemy. I will make a column for combined date and time, group the data frame by station, and calculate the difference between the entries value of one four-hour period and the next in order to calculate the net number of people entered in that four-hour period. I will use pandas and either matplotlib or seaborn to analyze and visualize the data.

- Are you planning in advance to need or use additional tools beyond those required?

I do not plan on using additional tools. 

### **MVP Goal:**

- What would a [minimum viable product (MVP)](https://github.com/thisismetis/Metis_Fundamentals/blob/main/project_deliverable_templates/mvp.md) look like for this project?

An MVP for this project would be an analysis of three months of turnstile data and a table, with accompanying graphs, of the top five stations with the most foot traffic. 

To go beyond this, I would include analysis of weekends versus weekdays, and the most populated days and times at particular stations. Additional data I could add to improve this project would be pedestrian-only streets in NYC, which provide another parameter other than foot traffic in subway stations that would be relevant to street performers.
