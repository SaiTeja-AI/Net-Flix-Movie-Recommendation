# Net-Flix-Movie-Recommendation
<h1>1. Business Problem </h1>
<h2> 1.1 Problem Description </h2>
<p>
Netflix is all about connecting people to the movies they love. To help customers find those movies, they developed world-class movie recommendation system: CinematchSM. Its job is to predict whether someone will enjoy a movie based on how much they liked or disliked other movies. Netflix use those predictions to make personal movie recommendations based on each customer’s unique tastes. And while <b>Cinematch</b> is doing pretty well, it can always be made better.
</p>
<p>Now there are a lot of interesting alternative approaches to how Cinematch works that netflix haven’t tried. Some are described in the literature, some aren’t. We’re curious whether any of these can beat Cinematch by making better predictions. Because, frankly, if there is a much better approach it could make a big difference to our customers and our business.</p>
<p> Credits: https://www.netflixprize.com/rules.html </p>
<h2> 1.2 Problem Statement </h2>
<p>
Netflix provided a lot of anonymous rating data, and a prediction accuracy bar that is 10% better than what Cinematch can do on the same training data set. (Accuracy is a measurement of how closely predicted ratings of movies match subsequent actual ratings.) 
</p>
<h2>1.2 Real world/Business Objectives and constraints  </h2>
<p> Objectives </p>
<ol>
  <li> Predict the rating that a user would give to a movie that he ahs not yet rated.</li>
  <li> Minimize the difference between predicted and actual rating (RMSE and MAPE). </li>
</ol>
<p> Constrains </p>
<ol>
  <li> Some form of interpretability. </li>
</ol>
<h1>2. Machine Learning Problem </h1>
<h3>2.1 Data format </h3>
<p> for each movie id there is corresponding CUSTOMERID,RATING,DATE and Movie Ids ranges form 1 to 17770 </p>
<p> CustomerIDs range from 1 to 2649429, with gaps. There are 480189 users.
Ratings are on a five star (integral) scale from 1 to 5.</p>
<h2>2.2 Mapping the real world problem to a Machine Learning Problem </h2>
<p>
For a given movie and user we need to predict the rating would be given by him/her to the movie. The given problem is a Recommendation problem It can also seen as a Regression problem 
</p>
<h3>2.2.2 Performance Metric </h3>
<ul>
<li> Mean Absolute Percentage Error: https://en.wikipedia.org/wiki/Mean_absolute_percentage_error </li>
<li> Root Mean Square Error: https://en.wikipedia.org/wiki/Root-mean-square_deviation </li>
</ul>
<h3> 2.2.3 Machine Learning Objective and Constraints </h3>
<ol>
  <li> Minimize RMSE. </li>
  <li> Try to provide some interpretability </li>
</ol>
<h3>
NEW Modification
</h3>
