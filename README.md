# sentiment-analysis-of-youtube-comments
TextBlob is a Python (2 and 3) library for processing textual data. It provides a consistent API for diving into common natural language processing (NLP) tasks such as part-of-speech tagging, noun phrase extraction, sentiment analysis, and more.
The sentiment property returns a namedtuple of the form Sentiment(polarity, subjectivity). The polarity score is a float within the range [-1.0, 1.0]. The subjectivity is a float within the range [0.0, 1.0] where 0.0 is very objective and 1.0 is very subjective.

I used a python module "openpyxl" which is used for doing operations on excel sheets.
I used this for importing data from excel sheets to array.

Arrays are very useful in handling data one by one.
Every sentence or data is fed to Text Blob as input and polarity of every data is given out as output.

Every output is stored in another array.
Three classification are chosen according to the polarity:
1.Bad if polarity is below zero.
2.neutral if polarity is zero.
3.good if polarity is greater than zero.

then according to classification we draw a piechart by use of a python module called "matplotlib.pyplot".

Output:-
total comments:bad=99,neutal=1162,good=700

bad comments are: ['These are all false. Enquire in the market before practicing such work', 'I want to learn more about chicken farming please help me', 'I also did banjara poultry faming at small lavel', ' Where is the training center in Kisanganj Bihar', '521 did not like this vedeo, it is very sad, such people do not give respect to the farmer.', 'Chicken name', 'This video is fake', 'vanaraja breed is not an active one. what should we feed it to become sexually active?', 'Chicken name', 'Chicken name']

good comments are: ['Hi, i am from Bangladesh. I am also a Youtuber on Agriculture. I always follow your channel. I learn many things from you! Pray for you.... Go ahead! My friend.💚💚', 'Thanks bro', 'Good', 'excellent. keep it up.', 'Thanks sir', 'Good knowledge, thank you sir', 'Nice', 'Thanks', 'Good farming', 'Wahhh.. proud of you']

