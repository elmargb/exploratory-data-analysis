It consists of segmenting the data according to some criteria and carrying out the previous analyzes considering this separation of the data into segments.

Segmenting the data, a priori, can be done considering 2 main criteria and different approaches to analyze different circumstances of the data:

- Segment the target. Segment the target variable into N groups. In this way, there is implicit segmentation in the data and we can see what characteristics can influence more or less different segments of the target variable.
- Segment characteristics by some business condition. Some business condition or condition of some key characteristic can be considered which segments the data into groups that according to expert knowledge are different groups.

In both cases, when performing data segmentation, what is needed is to have a column in the dataframe with categorical values that represent the data segmentation. This column with categorical values can be strings, and it is recommended that they be so that in the generated graphs you can interpret what the different categories into which the data was separated are.

To segment the data, different techniques can be used, from segmenting by expert knowledge of the business that the data represents as mentioned above or also segmenting by percentiles, etc.