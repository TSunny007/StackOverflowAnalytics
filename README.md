# StackOverflowAnalytics

# Wikipedia Structure Analysis
Using stack overflow Q/A data to perform feature analysis in the field of Computer Science

Poster:
![Poster](https://github.com/TarunSunkaraneni/StackOverflowAnalytics/blob/master/outputs/DM-poster.pdf)

[Dataset Used](https://www.kaggle.com/stackoverflow/stacksample)

[Reduction & Cleaning](https://nbviewer.jupyter.org/github/TarunSunkaraneni/StackOverflowAnalytics/blob/master/Notebooks/reduction_and_cleaning.ipynb): In this notebook I had to pre-process all questions and answers asked by people, and determine which questions can be deemed relevant. Finally, a cleaned, new dataset which only contains relevant questions is generated.

[Tag Network](https://nbviewer.jupyter.org/github/TarunSunkaraneni/StackOverflowAnalytics/blob/master/Notebooks/tag_network.ipynb): In this notebook I used links beteen all tags (ex. prevalance of AngularJS questions being also Javasctipt questions) to make a web depicting [topic relationships](https://github.com/TarunSunkaraneni/StackOverflowAnalytics/blob/master/Notebook/tag_links.png)

[User Question Mapping](https://nbviewer.jupyter.org/github/TarunSunkaraneni/StackOverflowAnalytics/blob/master/Notebooks/user_question_mapping.ipynb): In this notebook I mapped all users who asked questions into a high-dimensional point. The metrics considered were (1) A weighted score average per question (2) a simple counter of questions asked per category. It should be obvious that the resulting Matrix will be VERY sparse. In the end, the count metric ended up winning, but in the future, score should definitely a factor.

[Score-Question Relation](https://nbviewer.jupyter.org/github/TarunSunkaraneni/StackOverflowAnalytics/blob/master/Notebooks/score_tag_relation.ipynb): In this notebook I examined a relation between the number of questions a user asked, and the overall scores they got from the questions. It turned out that a `score` is a very turbulent factor, and that it doesn't speak a person's expertise very well i.e. a high score in a question doesn't necessarily mean that score reflects on their knowledge of topics. Perhaps it would make more sense with answers instead of questions. 

