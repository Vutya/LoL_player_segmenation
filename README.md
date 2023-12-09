# LoL player segmenation
This is exploratory clusterization of the averaged match data in LoL. Data for season 2020 was extracted for 2048 players of different ranks, 100 ranked solo queue matches each. Complex features were divided into simpler ones, uninformative features (std < 0.5) were removed, data was normalized, multicollinearity threat was diminished. Analysis is [here](https://github.com/Vutya/LoL_player_segmenation/blob/main/AnalysisData.ipynb).

After that t-SNE algorithm was used for averaged data over all players. It turned out that in this way players are grouped by most picked role in the last 100 matches rather than ranks. However, most players of lower ranks did not fall into any role cluster indicating that they did not choose their favourite role yet or they do not know yet how to play different roles.

![tsne-role](https://github.com/Vutya/LoL_player_segmenation/blob/main/clusters/tsne_role.png)
![tsne-rank](https://github.com/Vutya/LoL_player_segmenation/blob/main/clusters/tsne_rank.png)

k-means clustering in general reproduced this pattern:
![kmeans](https://github.com/Vutya/LoL_player_segmenation/blob/main/clusters/kmeans.png)

Centroids of clusters also indicate the most and least important features for each of the roles (e.g., vision score for supports, magical damage dealt to champions for mid lane)
![Jungle centroid](https://github.com/Vutya/LoL_player_segmenation/blob/main/clusters/jungle.png)
![Mid lane centroid](https://github.com/Vutya/LoL_player_segmenation/blob/main/clusters/mid.png)
![ADC centroid](https://github.com/Vutya/LoL_player_segmenation/blob/main/clusters/adc.png)
![Support centroid](https://github.com/Vutya/LoL_player_segmenation/blob/main/clusters/support.png)
![Top lane centroid](https://github.com/Vutya/LoL_player_segmenation/blob/main/clusters/top.png)
![Versatile centroid](https://github.com/Vutya/LoL_player_segmenation/blob/main/clusters/vers.png)

OSF link to the full raw dataset: https://osf.io/gpnkb

# Some very random and interesting links:
* [Escharts](https://escharts.com/) - esports media, but in a data-driven way
* [Mobalytics](https://mobalytics.gg/) - company that supports data-driven approach to improve ones performance
* [Newzoo](https://newzoo.com/) - analytics for game industry
* [Comprehensive review and classification of game analytics](https://doi.org/10.1007/s11761-020-00303-z) 
* [Book Game Analytics. Maximizing the Value of Player Data](https://link.springer.com/book/10.1007/978-1-4471-4769-5) 
* [Role Identification for Accurate Analysis in Dota 2](https://doi.org/10.1609/aiide.v15i1.5235) 
* [Time to Die 2: Improved in-game death prediction in Dota 2](https://www.sciencedirect.com/science/article/pii/S2666827023000191) 
* [Using API Data to Understand Learning in League of Legends: A Mixed Methods Study](https://doi.org/10.1080/09523987.2019.1614250)
* [Profiling Successful Team Behaviors in League of Legends](http://dx.doi.org/10.1145/3126858.3126886)
* [Smart kills and worthless deaths: eSports analytics for League of Legends](https://doi.org/10.1515/jqas-2019-0096)
* [Determinants of victory in Esports - StarCraft II](https://doi.org/10.1007/s11042-022-13373-2)
* [Classification of Player Roles in the Team-Based Multi-player Game Dota 2](https://doi.org/10.1007/978-3-319-24589-8_9)
* [MOBA Coach: Exploring and Analyzing Multiplayer Online Battle Arena Data](https://doi.org/10.1007/978-3-030-90439-5_16)
* [From Chess and Atari to StarCraft and Beyond: How Game AI is Driving the World of AI](https://doi.org/10.1007/s13218-020-00647-w)
* [Who belongs in the family?](https://doi.org/10.1007/BF02289263) - for elbow method
* Visualizing Data using t-SNE ([PDF](https://www.jmlr.org/papers/volume9/vandermaaten08a/vandermaaten08a.pdf))
* Identifying Patterns in Combat that are Predictive of Success in MOBA Games ([PDF](https://ciigar.csc.ncsu.edu/files/bib/Yang2014-MOBASucessPatterns.pdf))
* [DOTA 2 match prediction through deep learning team fight models](https://ieeexplore.ieee.org/document/9893647)
* Player Skill Modeling in Starcraft II ([PDF](https://ojs.aaai.org/index.php/AIIDE/article/download/12682/12530/16199))
* Masters of Control: Behavioral Patterns of Simultaneous Unit Group Manipulation in StarCraft 2 ([PDF](https://jeffhuang.com/papers/MastersOfControl_CHI15.pdf))
* [Game Data Science](https://academic.oup.com/book/39142) book
* Василий Сабиров [“Игра в цифры” ](https://habr.com/ru/companies/ruvds/articles/546306/)
* [20 Best Books for Game Analysts](https://www.devtodev.com/education/articles/en/154/20-best-books-for-game-analysts)




