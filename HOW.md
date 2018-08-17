# How was this chart made?

Most of the charts follow the same routine. Let's use our [Hands-On Machine Learning](https://anvaka.github.io/greview/hands-on-ml/1/)
chart as a reference.

[![hands-on-chart](https://i.imgur.com/a3Gjzgp.png)](https://anvaka.github.io/greview/hands-on-ml/1/)

Starting from the "Hands-On ML", I collected from Amazon 10 books that are most often bought together (I used Amazon’s product advertising api to fetch the graph).

Then, for each found book, I collected 5 more books that are most often bought together with them. Finally, I did this one more time for each found book.

After that, I ran my own algorithm to make a city from these books. 

The algorithm tends to group similar books into districts. You can find advanced theoretical books like Deep Learning and Probabilistic Graphical Models clustered together in the North West. "For Dummies" series clustered on the East. North regions are taken by financial machine learning, and South is occupied by Python/Data Science books.

The roads on the map have symbolic meaning. The thicker the road, the more books are connected through it.

# What is that city like algorithm?

It's not publicly available yet, as I haven't figured everything out yet. It involves lots of tweaking
and ad-hoc modification. I hope by making more of these visualization I'll improve the algorithm
and release it one day. At the moment it's not ready.