README.md

Important notes about the visualization -
This visualization takes its data from the kaggle dataset on the titanic, which can be found here - https://www.kaggle.com/c/titanic. The visualization is constructed using the data from 1046 of the passengers who have complete age, sex and class information. 

Summary -

The purpose of this visualization is to allow the reader to explore the effect of demographics on survival rate for titanic passengers. A key takeaway is the large difference in survival rate between gender and class. 

Design -

The graphic starts with an animation that shows the highest and lowest survival rates among 1st class women and third class men respectively. I decided to go with the martini glass style of visualization talked about in the class, where there is an opening animation with some explanatory information which then opens up to user interaction. The animation starts with introductory text about the titanic. Time is given to read this text and engage the reader before any data is displayed. I chose to use a horizontal stacked bar to present the data, with a dark blue representing the survival rate. A lighter blue bar is first presented to represent 100% of the data and give some context for when the darker blue bar appears. In the first part of the animation the bar appears, representing the survival rate of females in first class. In this animation sequence, the introductory text turns gray to avoid distracting attention. The text that explains the bar appears below in black to draw the eye. After several seconds, the bar and text change to represent males in third class. The percentage to the right of the bar is the same color as the bar in order to show relation. Finally, there is a transition to the interactive phase, in which the parameters menu appears (not present during animation to avoid distraction), the introductory text disappears, and the explanatory text turns gray to deemphasize. 

In the parameter menu the buttons turn blue on click to help the reader keep track of the categories they have selected. The buttons are originally black because black is commonly associated with off. The buttons turn blue to match the color of the bar chart, again for the implied relation. All the text is in arial font for easy reading. 

I chose to include the "select at least one parameter" text originally out of convenience based on the way I coded the button functionality. Because the buttons change color on click, I thought it would be confusing for the reader if a category like age was not selected (all the buttons would be black) but then actually represent all ages. A workaround to this would have all the buttons turn blue upon updating, but that could also be confusing in its own way. 

From earlier drafts of the visualization I have chosen to remove some of the unecessary information included, such as the footnotes and link to the kaggle website, including it instead at the top of the readme. This is to prevent the reader from getting overwhelmed by chartjunk. 


Feedback -

1) The total number of people shown in the text below the circle does not add up to the total number of datapoints being used as shown in the footnote. Caused by some rows of data having missing values for age. Fixed by assigning age of 0 to all missing rows. Added disclaimer to graphic explaining this

2) Animation not distinct enough from interactive portion. Originally no difference in color of circle or buttons. Fixed by changing the color of the buttons and circle during the animation to gray and green respectively to indicate difference. Also added "select parameters" text at the end of the animation to explicitly tell reader to begin interactive phase.

3) When no buttons in a group are selected, no circle showed up and "0 out of 0" text appeared. Fixed text to say "Please select at least one of each parameter"

4) Using a circle changing in size to encode the information was unclear because it seemed to represent 100% of the data all the time. Changed to a horizontal stacked bar in order to make the 100% explicitely noticeable.

5) Some chartjunk, such as footnotes and a link were distracting. Removed and added to README file instead. 

6) Included datapoints without listed ages in the 0-20 category. This represented about a fifth of the dataset. Decided to remove these from the visualization altogether in order to avoid confusion and bias. 

Resources -

http://www.w3schools.com/js/
http://stackoverflow.com/
