### CS 416: Narrative Visualization, Supplementary Essay \


The visualization is available here: [https://akshatvn.github.io/f1/constructors_histories.html](https://akshatvn.github.io/f1/constructors_histories.html)


#### **Messaging**

Looking at the last 70 years’ F1 race victory data, we can compare constructors and drivers. We can also understand the impact of individual drivers' movements across constructors.


#### **Narrative Structure**

The structure of the visualization is a drill-down story, with a few annotations to make the viewer understand how to interpret the slides.

Each scene (except the last) has elements that can be clicked on to take the viewer deeper into the scene. From an overview of all constructors, to a single constructor’s view, to a single driver’s view.


#### **Visual Structure**

Each constructor has been assigned a unique color, which is consistent across scenes. As is described at the top of each page, the viewer can navigate to deeper levels by clicking on marks - lines or bubbles. The best performing drivers on the constructor level have been labeled, drawing attention. The breadcrumbs line at the top of the page puts the scene in context, allowing the user to understand how they landed on the scene, while also affording the capability of going back to previous scenes.

All 3 pages main scenes are charts with year on the x axis and number of wins on the y axis. The last page, which is the driver history page, is a stacked bar chart to better portray the transition of the driver between constructors.


#### **Scenes**

The first scene is an overview of all F1 constructors' win histories plotted as lines. There is a button on the top right to switch the format to totals, reducing the information into bubbles and taking time (year) out of the picture. Hovering over the lines or bubbles gives some aggregated information about the constructor, and clicking leads to the next scene, specific to the chosen constructor.

The second scene is that of a particular constructor's history. All lines on this scene are of a single color, representing that this graph corresponds only to one constructor. For example, even though Kimi Raikonen has raced for Mclaren, Ferrari and Team Lotus, landing on this scene by clicking on Ferrari will only include Kimi Raikonen's Ferrari (red) wins. Once again, clicking on the line or the bubble takes the viewer to the next scene, specific to the chosen driver.

The third scene is of a particular driver's history. It shows all the years the driver won any races, with bars colored as per constructor. This can be interesting to the viewer, for example when landing on Lewis Hamilton's scene, it is clear that Mercedes has far outperformed Mclaren's track record.


#### **Annotations**

Some points of interest are annotated, in order to ease understanding the intent of use. The viewer is encouraged to make their own observations as well.


#### **Parameters and States**

Parameters are chosen constructor, chosen driver, scene template. Each scene is a combination of the template, the chosen constructor (if any) , a chosen driver (if any) and the view mode. The parameters all come from the URL, and define the template, the text, and the breadcrumbs line.


#### **Triggers**

Triggers. What are the triggers that connect user actions to changes of state in the narrative visualization? What affordances are provided to the user to communicate to them what options are available to them in the narrative visualization?

Bringing the mouse pointer over any data item opens a tooltip displaying more information "on demand". Some elements can be clicked on, as is highlighted by changing the cursor to a pointer, enlarging the bubbles.

The navigation links in the breadcrumbs line change color on mouse over too, suggesting that they can be clicked on


### Appendix


#### **Data Source**

The data was downloaded from here: [https://www.kaggle.com/rohanrao/formula-1-world-championship-1950-2020](https://www.kaggle.com/rohanrao/formula-1-world-championship-1950-2020?select=races.csv)

As for the preprocessing, all data from races in 2021 was removed, as the data was plotted with a year granularity. Each constructor was also assigned a unique color, trying to keep in mind what color that constructor is generally associated with. 


#### **Code Source**

[https://github.com/akshatvn/f1](https://github.com/akshatvn/f1)
