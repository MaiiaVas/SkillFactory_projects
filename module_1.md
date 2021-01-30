```python

import pandas as pd #impost library pandas
movie_bd = pd.read_csv('movie_bd_v5.csv') #convert our file to dataframe
display(movie_bd) #show our dataframe


```


<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>imdb_id</th>
      <th>budget</th>
      <th>revenue</th>
      <th>original_title</th>
      <th>cast</th>
      <th>director</th>
      <th>tagline</th>
      <th>overview</th>
      <th>runtime</th>
      <th>genres</th>
      <th>production_companies</th>
      <th>release_date</th>
      <th>vote_average</th>
      <th>release_year</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>tt0369610</td>
      <td>150000000</td>
      <td>1513528810</td>
      <td>Jurassic World</td>
      <td>Chris Pratt|Bryce Dallas Howard|Irrfan Khan|Vi...</td>
      <td>Colin Trevorrow</td>
      <td>The park is open.</td>
      <td>Twenty-two years after the events of Jurassic ...</td>
      <td>124</td>
      <td>Action|Adventure|Science Fiction|Thriller</td>
      <td>Universal Studios|Amblin Entertainment|Legenda...</td>
      <td>6/9/2015</td>
      <td>6.5</td>
      <td>2015</td>
    </tr>
    <tr>
      <th>1</th>
      <td>tt1392190</td>
      <td>150000000</td>
      <td>378436354</td>
      <td>Mad Max: Fury Road</td>
      <td>Tom Hardy|Charlize Theron|Hugh Keays-Byrne|Nic...</td>
      <td>George Miller</td>
      <td>What a Lovely Day.</td>
      <td>An apocalyptic story set in the furthest reach...</td>
      <td>120</td>
      <td>Action|Adventure|Science Fiction|Thriller</td>
      <td>Village Roadshow Pictures|Kennedy Miller Produ...</td>
      <td>5/13/2015</td>
      <td>7.1</td>
      <td>2015</td>
    </tr>
    <tr>
      <th>2</th>
      <td>tt2908446</td>
      <td>110000000</td>
      <td>295238201</td>
      <td>Insurgent</td>
      <td>Shailene Woodley|Theo James|Kate Winslet|Ansel...</td>
      <td>Robert Schwentke</td>
      <td>One Choice Can Destroy You</td>
      <td>Beatrice Prior must confront her inner demons ...</td>
      <td>119</td>
      <td>Adventure|Science Fiction|Thriller</td>
      <td>Summit Entertainment|Mandeville Films|Red Wago...</td>
      <td>3/18/2015</td>
      <td>6.3</td>
      <td>2015</td>
    </tr>
    <tr>
      <th>3</th>
      <td>tt2488496</td>
      <td>200000000</td>
      <td>2068178225</td>
      <td>Star Wars: The Force Awakens</td>
      <td>Harrison Ford|Mark Hamill|Carrie Fisher|Adam D...</td>
      <td>J.J. Abrams</td>
      <td>Every generation has a story.</td>
      <td>Thirty years after defeating the Galactic Empi...</td>
      <td>136</td>
      <td>Action|Adventure|Science Fiction|Fantasy</td>
      <td>Lucasfilm|Truenorth Productions|Bad Robot</td>
      <td>12/15/2015</td>
      <td>7.5</td>
      <td>2015</td>
    </tr>
    <tr>
      <th>4</th>
      <td>tt2820852</td>
      <td>190000000</td>
      <td>1506249360</td>
      <td>Furious 7</td>
      <td>Vin Diesel|Paul Walker|Jason Statham|Michelle ...</td>
      <td>James Wan</td>
      <td>Vengeance Hits Home</td>
      <td>Deckard Shaw seeks revenge against Dominic Tor...</td>
      <td>137</td>
      <td>Action|Crime|Thriller</td>
      <td>Universal Pictures|Original Film|Media Rights ...</td>
      <td>4/1/2015</td>
      <td>7.3</td>
      <td>2015</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>1884</th>
      <td>tt0120903</td>
      <td>75000000</td>
      <td>157299717</td>
      <td>X-Men</td>
      <td>Patrick Stewart|Hugh Jackman|Ian McKellen|Hall...</td>
      <td>Bryan Singer</td>
      <td>Evolution Begins</td>
      <td>Two mutants, Rogue and Wolverine, come to a pr...</td>
      <td>104</td>
      <td>Adventure|Action|Science Fiction</td>
      <td>Twentieth Century Fox Film Corporation|Donners...</td>
      <td>7/13/2000</td>
      <td>6.6</td>
      <td>2000</td>
    </tr>
    <tr>
      <th>1885</th>
      <td>tt0192255</td>
      <td>22000000</td>
      <td>13555988</td>
      <td>The Little Vampire</td>
      <td>Richard E. Grant|Jonathan Lipnicki|Jim Carter|...</td>
      <td>Uli Edel</td>
      <td>They're not just best friends, they're blood b...</td>
      <td>Based on the popular books, the story tells of...</td>
      <td>95</td>
      <td>Horror|Family|Foreign</td>
      <td>New Line Cinema</td>
      <td>10/27/2000</td>
      <td>6.4</td>
      <td>2000</td>
    </tr>
    <tr>
      <th>1886</th>
      <td>tt0131704</td>
      <td>76000000</td>
      <td>35134820</td>
      <td>The Adventures of Rocky &amp; Bullwinkle</td>
      <td>Rene Russo|Jason Alexander|Piper Perabo|Randy ...</td>
      <td>Des McAnuff</td>
      <td>This summer it's not the same old bull.</td>
      <td>Rocky and Bullwinkle have been living off the ...</td>
      <td>88</td>
      <td>Adventure|Animation|Action|Comedy|Family</td>
      <td>Universal Pictures|Capella International|KC Me...</td>
      <td>6/30/2000</td>
      <td>4.0</td>
      <td>2000</td>
    </tr>
    <tr>
      <th>1887</th>
      <td>tt0162983</td>
      <td>40000000</td>
      <td>36037909</td>
      <td>Hanging Up</td>
      <td>Meg Ryan|Diane Keaton|Lisa Kudrow|Walter Matth...</td>
      <td>Diane Keaton</td>
      <td>Every family has a few hang-ups.</td>
      <td>A trio of sisters bond over their ambivalence ...</td>
      <td>94</td>
      <td>Comedy|Drama</td>
      <td>Laurence Mark Productions|Columbia Pictures Co...</td>
      <td>2/16/2000</td>
      <td>5.2</td>
      <td>2000</td>
    </tr>
    <tr>
      <th>1888</th>
      <td>tt0163676</td>
      <td>15000000</td>
      <td>5217498</td>
      <td>The In Crowd</td>
      <td>Susan Ward|Lori Heuring|Matthew Settle|Nathan ...</td>
      <td>Mary Lambert</td>
      <td>What would you do to get in?</td>
      <td>A mentally disturbed young woman takes a job a...</td>
      <td>105</td>
      <td>Thriller</td>
      <td>Warner Bros. Pictures</td>
      <td>7/19/2000</td>
      <td>5.2</td>
      <td>2000</td>
    </tr>
  </tbody>
</table>
<p>1889 rows × 14 columns</p>
</div>



```python
#Вопрос 1. У какого фильма из списка самый большой бюджет?

#we already import library and file, so we can go right to finding necessary information 
movie_bd.loc[movie_bd.budget == movie_bd.budget.max()] #finding what row contains the biggest budget for the film
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>imdb_id</th>
      <th>budget</th>
      <th>revenue</th>
      <th>original_title</th>
      <th>cast</th>
      <th>director</th>
      <th>tagline</th>
      <th>overview</th>
      <th>runtime</th>
      <th>genres</th>
      <th>production_companies</th>
      <th>release_date</th>
      <th>vote_average</th>
      <th>release_year</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>723</th>
      <td>tt1298650</td>
      <td>380000000</td>
      <td>1021683000</td>
      <td>Pirates of the Caribbean: On Stranger Tides</td>
      <td>Johnny Depp|PenÃ©lope Cruz|Geoffrey Rush|Ian M...</td>
      <td>Rob Marshall</td>
      <td>Live Forever Or Die Trying.</td>
      <td>Captain Jack Sparrow crosses paths with a woma...</td>
      <td>136</td>
      <td>Adventure|Action|Fantasy</td>
      <td>Walt Disney Pictures|Jerry Bruckheimer Films|M...</td>
      <td>5/11/2011</td>
      <td>6.3</td>
      <td>2011</td>
    </tr>
  </tbody>
</table>
</div>




```python
#Вопрос 2. Какой из фильмов самый длительный (в минутах)?

movie_bd.loc[movie_bd.runtime == movie_bd.runtime.max()] #finding what row contains the longest film
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>imdb_id</th>
      <th>budget</th>
      <th>revenue</th>
      <th>original_title</th>
      <th>cast</th>
      <th>director</th>
      <th>tagline</th>
      <th>overview</th>
      <th>runtime</th>
      <th>genres</th>
      <th>production_companies</th>
      <th>release_date</th>
      <th>vote_average</th>
      <th>release_year</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1157</th>
      <td>tt0279111</td>
      <td>56000000</td>
      <td>12923936</td>
      <td>Gods and Generals</td>
      <td>Stephen Lang|Jeff Daniels|Robert Duvall|Kevin ...</td>
      <td>Ronald F. Maxwell</td>
      <td>The nations heart was touched by...</td>
      <td>The film centers mostly around the personal an...</td>
      <td>214</td>
      <td>Drama|History|War</td>
      <td>Turner Pictures|Antietam Filmworks</td>
      <td>2/21/2003</td>
      <td>5.8</td>
      <td>2003</td>
    </tr>
  </tbody>
</table>
</div>




```python
#Вопрос 3. Какой из фильмов самый короткий (в минутах)?

movie_bd.loc[movie_bd.runtime == movie_bd.runtime.min()] #finding what row contains the fastest film
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>imdb_id</th>
      <th>budget</th>
      <th>revenue</th>
      <th>original_title</th>
      <th>cast</th>
      <th>director</th>
      <th>tagline</th>
      <th>overview</th>
      <th>runtime</th>
      <th>genres</th>
      <th>production_companies</th>
      <th>release_date</th>
      <th>vote_average</th>
      <th>release_year</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>768</th>
      <td>tt1449283</td>
      <td>30000000</td>
      <td>14460000</td>
      <td>Winnie the Pooh</td>
      <td>Jim Cummings|Travis Oates|Jim Cummings|Bud Luc...</td>
      <td>Stephen Anderson|Don Hall</td>
      <td>Oh Pooh.</td>
      <td>During an ordinary day in Hundred Acre Wood, W...</td>
      <td>63</td>
      <td>Animation|Family</td>
      <td>Walt Disney Pictures|Walt Disney Animation Stu...</td>
      <td>4/13/2011</td>
      <td>6.8</td>
      <td>2011</td>
    </tr>
  </tbody>
</table>
</div>




```python
#Вопрос 4. Какова средняя длительность фильмов?

movie_bd.runtime.mean() #finding what is the average movie length in our DataFrame
```




    109.6585494970884




```python
#Вопрос 5. Каково медианное значение длительности фильмов?

movie_bd.runtime.median() #finding what is the median of movie length
```




    107.0




```python
#Вопрос 6. Какой фильм самый прибыльный?

movie_bd['profit'] = movie_bd['revenue'] - movie_bd['budget'] #creating new column
movie_bd.loc[movie_bd.profit == movie_bd.profit.max()] #finding what row contains the most profitable film
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>imdb_id</th>
      <th>budget</th>
      <th>revenue</th>
      <th>original_title</th>
      <th>cast</th>
      <th>director</th>
      <th>tagline</th>
      <th>overview</th>
      <th>runtime</th>
      <th>genres</th>
      <th>production_companies</th>
      <th>release_date</th>
      <th>vote_average</th>
      <th>release_year</th>
      <th>profit</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>239</th>
      <td>tt0499549</td>
      <td>237000000</td>
      <td>2781505847</td>
      <td>Avatar</td>
      <td>Sam Worthington|Zoe Saldana|Sigourney Weaver|S...</td>
      <td>James Cameron</td>
      <td>Enter the World of Pandora.</td>
      <td>In the 22nd century, a paraplegic Marine is di...</td>
      <td>162</td>
      <td>Action|Adventure|Fantasy|Science Fiction</td>
      <td>Ingenious Film Partners|Twentieth Century Fox ...</td>
      <td>12/10/2009</td>
      <td>7.1</td>
      <td>2009</td>
      <td>2544505847</td>
    </tr>
  </tbody>
</table>
</div>




```python
#Вопрос 7. Какой фильм самый убыточный?

#we already create new column in the previous step, so we can go right to finding necessary information 
movie_bd.loc[movie_bd.profit == movie_bd.profit.min()] #finding what row contains the most unprofitable film
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>imdb_id</th>
      <th>budget</th>
      <th>revenue</th>
      <th>original_title</th>
      <th>cast</th>
      <th>director</th>
      <th>tagline</th>
      <th>overview</th>
      <th>runtime</th>
      <th>genres</th>
      <th>production_companies</th>
      <th>release_date</th>
      <th>vote_average</th>
      <th>release_year</th>
      <th>profit</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1245</th>
      <td>tt1210819</td>
      <td>255000000</td>
      <td>89289910</td>
      <td>The Lone Ranger</td>
      <td>Johnny Depp|Armie Hammer|William Fichtner|Hele...</td>
      <td>Gore Verbinski</td>
      <td>Never Take Off the Mask</td>
      <td>The Texas Rangers chase down a gang of outlaws...</td>
      <td>149</td>
      <td>Action|Adventure|Western</td>
      <td>Walt Disney Pictures|Jerry Bruckheimer Films|I...</td>
      <td>7/3/2013</td>
      <td>6.0</td>
      <td>2013</td>
      <td>-165710090</td>
    </tr>
  </tbody>
</table>
</div>




```python
#Вопрос 8. У скольких фильмов из датасета объем сборов оказался выше бюджета?

movie_bd.loc[movie_bd.revenue > movie_bd.budget] #finding the amount of films where revenue was higher than the budget(we can see the amount of rows-this is the answer)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>imdb_id</th>
      <th>budget</th>
      <th>revenue</th>
      <th>original_title</th>
      <th>cast</th>
      <th>director</th>
      <th>tagline</th>
      <th>overview</th>
      <th>runtime</th>
      <th>genres</th>
      <th>production_companies</th>
      <th>release_date</th>
      <th>vote_average</th>
      <th>release_year</th>
      <th>profit</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>tt0369610</td>
      <td>150000000</td>
      <td>1513528810</td>
      <td>Jurassic World</td>
      <td>Chris Pratt|Bryce Dallas Howard|Irrfan Khan|Vi...</td>
      <td>Colin Trevorrow</td>
      <td>The park is open.</td>
      <td>Twenty-two years after the events of Jurassic ...</td>
      <td>124</td>
      <td>Action|Adventure|Science Fiction|Thriller</td>
      <td>Universal Studios|Amblin Entertainment|Legenda...</td>
      <td>6/9/2015</td>
      <td>6.5</td>
      <td>2015</td>
      <td>1363528810</td>
    </tr>
    <tr>
      <th>1</th>
      <td>tt1392190</td>
      <td>150000000</td>
      <td>378436354</td>
      <td>Mad Max: Fury Road</td>
      <td>Tom Hardy|Charlize Theron|Hugh Keays-Byrne|Nic...</td>
      <td>George Miller</td>
      <td>What a Lovely Day.</td>
      <td>An apocalyptic story set in the furthest reach...</td>
      <td>120</td>
      <td>Action|Adventure|Science Fiction|Thriller</td>
      <td>Village Roadshow Pictures|Kennedy Miller Produ...</td>
      <td>5/13/2015</td>
      <td>7.1</td>
      <td>2015</td>
      <td>228436354</td>
    </tr>
    <tr>
      <th>2</th>
      <td>tt2908446</td>
      <td>110000000</td>
      <td>295238201</td>
      <td>Insurgent</td>
      <td>Shailene Woodley|Theo James|Kate Winslet|Ansel...</td>
      <td>Robert Schwentke</td>
      <td>One Choice Can Destroy You</td>
      <td>Beatrice Prior must confront her inner demons ...</td>
      <td>119</td>
      <td>Adventure|Science Fiction|Thriller</td>
      <td>Summit Entertainment|Mandeville Films|Red Wago...</td>
      <td>3/18/2015</td>
      <td>6.3</td>
      <td>2015</td>
      <td>185238201</td>
    </tr>
    <tr>
      <th>3</th>
      <td>tt2488496</td>
      <td>200000000</td>
      <td>2068178225</td>
      <td>Star Wars: The Force Awakens</td>
      <td>Harrison Ford|Mark Hamill|Carrie Fisher|Adam D...</td>
      <td>J.J. Abrams</td>
      <td>Every generation has a story.</td>
      <td>Thirty years after defeating the Galactic Empi...</td>
      <td>136</td>
      <td>Action|Adventure|Science Fiction|Fantasy</td>
      <td>Lucasfilm|Truenorth Productions|Bad Robot</td>
      <td>12/15/2015</td>
      <td>7.5</td>
      <td>2015</td>
      <td>1868178225</td>
    </tr>
    <tr>
      <th>4</th>
      <td>tt2820852</td>
      <td>190000000</td>
      <td>1506249360</td>
      <td>Furious 7</td>
      <td>Vin Diesel|Paul Walker|Jason Statham|Michelle ...</td>
      <td>James Wan</td>
      <td>Vengeance Hits Home</td>
      <td>Deckard Shaw seeks revenge against Dominic Tor...</td>
      <td>137</td>
      <td>Action|Crime|Thriller</td>
      <td>Universal Pictures|Original Film|Media Rights ...</td>
      <td>4/1/2015</td>
      <td>7.3</td>
      <td>2015</td>
      <td>1316249360</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>1871</th>
      <td>tt0171433</td>
      <td>30000000</td>
      <td>37036004</td>
      <td>Keeping the Faith</td>
      <td>Ben Stiller|Edward Norton|Jenna Elfman|Anne Ba...</td>
      <td>Edward Norton</td>
      <td>If you have to believe in something, you may a...</td>
      <td>Best friends since they were kids, Rabbi Jacob...</td>
      <td>127</td>
      <td>Comedy</td>
      <td>Spyglass Entertainment|Touchstone Pictures|Tri...</td>
      <td>4/14/2000</td>
      <td>5.7</td>
      <td>2000</td>
      <td>7036004</td>
    </tr>
    <tr>
      <th>1875</th>
      <td>tt0219854</td>
      <td>65000000</td>
      <td>69700000</td>
      <td>The Kid</td>
      <td>Bruce Willis|Spencer Breslin|Emily Mortimer|Li...</td>
      <td>Jon Turteltaub</td>
      <td>Nobody ever grows up quite like they imagined.</td>
      <td>Powerful businessman Russ Duritz is self-absor...</td>
      <td>104</td>
      <td>Fantasy|Comedy|Family</td>
      <td>Walt Disney Pictures</td>
      <td>7/7/2000</td>
      <td>5.9</td>
      <td>2000</td>
      <td>4700000</td>
    </tr>
    <tr>
      <th>1877</th>
      <td>tt0199725</td>
      <td>20000000</td>
      <td>27728118</td>
      <td>Love &amp; Basketball</td>
      <td>Chris Warren, Jr.|Kyla Pratt|Sanaa Lathan|Omar...</td>
      <td>Gina Prince-Bythewood</td>
      <td>All's fair in love and basketball.</td>
      <td>A young African-American couple navigates the ...</td>
      <td>124</td>
      <td>Action|Comedy|Drama|Romance</td>
      <td>40 Acres &amp; A Mule Filmworks</td>
      <td>4/21/2000</td>
      <td>7.3</td>
      <td>2000</td>
      <td>7728118</td>
    </tr>
    <tr>
      <th>1883</th>
      <td>tt0122459</td>
      <td>24000000</td>
      <td>36609995</td>
      <td>Return to Me</td>
      <td>David Duchovny|Minnie Driver|Carroll O'Connor|...</td>
      <td>Bonnie Hunt</td>
      <td>A comedy straight from the heart</td>
      <td>It took a lot of cajoling to get Bob (Duchovny...</td>
      <td>115</td>
      <td>Romance|Comedy|Drama</td>
      <td>Metro-Goldwyn-Mayer (MGM)|JLT Productions</td>
      <td>4/7/2000</td>
      <td>5.5</td>
      <td>2000</td>
      <td>12609995</td>
    </tr>
    <tr>
      <th>1884</th>
      <td>tt0120903</td>
      <td>75000000</td>
      <td>157299717</td>
      <td>X-Men</td>
      <td>Patrick Stewart|Hugh Jackman|Ian McKellen|Hall...</td>
      <td>Bryan Singer</td>
      <td>Evolution Begins</td>
      <td>Two mutants, Rogue and Wolverine, come to a pr...</td>
      <td>104</td>
      <td>Adventure|Action|Science Fiction</td>
      <td>Twentieth Century Fox Film Corporation|Donners...</td>
      <td>7/13/2000</td>
      <td>6.6</td>
      <td>2000</td>
      <td>82299717</td>
    </tr>
  </tbody>
</table>
<p>1478 rows × 15 columns</p>
</div>




```python
#Вопрос 9. Какой фильм оказался самым кассовым в 2008 году?

movie_bd_new = movie_bd[movie_bd.release_year==2008] #creating the new dataset with films of only 2008 year
movie_bd_new.loc[movie_bd_new.revenue == movie_bd_new.revenue.max()] #row with highest grossing film in 2008
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>imdb_id</th>
      <th>budget</th>
      <th>revenue</th>
      <th>original_title</th>
      <th>cast</th>
      <th>director</th>
      <th>tagline</th>
      <th>overview</th>
      <th>runtime</th>
      <th>genres</th>
      <th>production_companies</th>
      <th>release_date</th>
      <th>vote_average</th>
      <th>release_year</th>
      <th>profit</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>599</th>
      <td>tt0468569</td>
      <td>185000000</td>
      <td>1001921825</td>
      <td>The Dark Knight</td>
      <td>Christian Bale|Michael Caine|Heath Ledger|Aaro...</td>
      <td>Christopher Nolan</td>
      <td>Why So Serious?</td>
      <td>Batman raises the stakes in his war on crime. ...</td>
      <td>152</td>
      <td>Drama|Action|Crime|Thriller</td>
      <td>DC Comics|Legendary Pictures|Warner Bros.|Syncopy</td>
      <td>7/16/2008</td>
      <td>8.1</td>
      <td>2008</td>
      <td>816921825</td>
    </tr>
  </tbody>
</table>
</div>




```python
#Вопрос 10. Самый убыточный фильм за период с 2012 по 2014 годы (включительно)?

movie_bd_new2 = movie_bd[(movie_bd.release_year >= 2012) & (movie_bd.release_year <= 2014)] #new dataset with films release beatween 2012 and 2014 inclusive
movie_bd_new2.loc[movie_bd_new2.profit == movie_bd_new2.profit.min()] #row with most unprofitable film between 2012 and 2014
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>imdb_id</th>
      <th>budget</th>
      <th>revenue</th>
      <th>original_title</th>
      <th>cast</th>
      <th>director</th>
      <th>tagline</th>
      <th>overview</th>
      <th>runtime</th>
      <th>genres</th>
      <th>production_companies</th>
      <th>release_date</th>
      <th>vote_average</th>
      <th>release_year</th>
      <th>profit</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1245</th>
      <td>tt1210819</td>
      <td>255000000</td>
      <td>89289910</td>
      <td>The Lone Ranger</td>
      <td>Johnny Depp|Armie Hammer|William Fichtner|Hele...</td>
      <td>Gore Verbinski</td>
      <td>Never Take Off the Mask</td>
      <td>The Texas Rangers chase down a gang of outlaws...</td>
      <td>149</td>
      <td>Action|Adventure|Western</td>
      <td>Walt Disney Pictures|Jerry Bruckheimer Films|I...</td>
      <td>7/3/2013</td>
      <td>6.0</td>
      <td>2013</td>
      <td>-165710090</td>
    </tr>
  </tbody>
</table>
</div>




```python
#Вопрос 11. Какого жанра фильмов больше всего?

#divide genres by symbol and expand the resulting lists using the explode function
movie_bd.genres.str.split('|').explode().value_counts()
```




    Drama              782
    Comedy             683
    Thriller           596
    Action             582
    Adventure          415
    Crime              315
    Romance            308
    Family             260
    Science Fiction    248
    Fantasy            222
    Horror             176
    Mystery            168
    Animation          139
    Music               64
    History             62
    War                 58
    Western             19
    Documentary          8
    Foreign              2
    Name: genres, dtype: int64




```python
#Вопрос 12. Фильмы какого жанра чаще всего становятся прибыльными?

df = movie_bd[movie_bd.profit > 0][['genres']] #new dataset with only profitable films by genres
df.genres = df.genres.str.split('|') #divide genres by symbol
df = df.explode('genres') #expand the resulting lists using the explode function
df.genres.value_counts()
```




    Drama              560
    Comedy             551
    Thriller           446
    Action             444
    Adventure          337
    Romance            242
    Crime              231
    Family             226
    Science Fiction    195
    Fantasy            188
    Horror             150
    Animation          120
    Mystery            119
    Music               47
    History             46
    War                 41
    Western             12
    Documentary          7
    Name: genres, dtype: int64




```python
#Вопрос 13. У какого режиссёра самые большие суммарные кассовые сборы?

director_df = movie_bd.copy() #new dataset
director_df['director'] = director_df.director.str.split('|') #divide directors by symbol
director_df2 = director_df.explode('director') #expand the resulting lists using the explode function
director_df2.groupby(['director'])['revenue'].sum().sort_values(ascending=False).index[0] 
#sort our dataset for directors by revenue to find the director with the highest sum of films' gross
```




    'Peter Jackson'




```python
#Вопрос 14. Какой режиссер снял больше всего фильмов в стиле Action?

movie_bd[movie_bd.genres.str.contains('Action')].director.str.split('|').explode().value_counts()
#find rows with action and then find the director who is more ofthen makes such films
```




    Robert Rodriguez       9
    Paul W.S. Anderson     7
    Michael Bay            7
    Ridley Scott           6
    Antoine Fuqua          6
                          ..
    Julie Anne Robinson    1
    Eli Roth               1
    Patrick Lussier        1
    Christian Alvart       1
    Pitof                  1
    Name: director, Length: 364, dtype: int64




```python
#Вопрос 15. Фильмы с каким актером принесли самые высокие кассовые сборы в 2012 году?

cast_df = movie_bd[movie_bd.release_year == 2012].copy() #creating the new dataset with films of only 2008 year
cast_df['cast'] = cast_df.cast.str.split('|') #divide cast by symbol 
cast_df2 = cast_df.explode('cast') #expand the resulting lists using the explode function
cast_df2.groupby(['cast'])['revenue'].sum().sort_values(ascending=False).index[0]
#sort our dataset for actors by revenue to find the actor with the highest sum of films' gross
```




    'Chris Hemsworth'




```python
#Вопрос 16. Какой актер снялся в большем количестве высокобюджетных фильмов? Примечание: в фильмах, где бюджет выше среднего по данной выборке.

actor_df = movie_bd[movie_bd.budget > movie_bd.budget.mean()].copy() #creating the new dataset with films with high budget, more then average
actor_df['cast'] = actor_df.cast.str.split('|') #divide cast by symbol
actor_df2 = actor_df.explode('cast') #expand the resulting lists using the explode function
actor_df2.groupby(['cast'])['budget'].count().sort_values(ascending=False)
#sort our dataset for actors by budget to find the actor who avting in the biggest ammount of high budget films
```




    cast
    Matt Damon           18
    Adam Sandler         17
    Angelina Jolie       16
    Eddie Murphy         15
    Samuel L. Jackson    15
                         ..
    Leslie Bibb           1
    Leonard Nimoy         1
    Lennie James          1
    Lena Olin             1
    50 Cent               1
    Name: budget, Length: 1505, dtype: int64




```python
#Вопрос 17. В фильмах какого жанра больше всего снимался Nicolas Cage?

movie_bd[movie_bd.cast.str.contains('Nicolas Cage')].genres.str.split('|').explode().value_counts()
#find genre in which Nicolas Cage acting more ofthen by finding cast that contains his name and creating list of genres
```




    Action             17
    Thriller           15
    Drama              12
    Crime              10
    Fantasy             8
    Adventure           7
    Comedy              6
    Science Fiction     4
    Family              3
    Animation           3
    Mystery             3
    History             2
    Horror              1
    Romance             1
    War                 1
    Name: genres, dtype: int64




```python
#Вопрос 18. Самый убыточный фильм от Paramount Pictures?

production_df = movie_bd[movie_bd.production_companies.str.contains('Paramount Pictures')] 
#creating the new dataset with films that was created by Paramount Picture by finding production_companies that contains this name
production_df.groupby(['original_title'])['profit'].min().sort_values(ascending=True)
 #finding most unprofitable of Paramount Pictures
```




    original_title
    K-19: The Widowmaker                                  -64831034
    Timeline                                              -60519261
    Next                                                  -51788987
    Alfie                                                 -46604061
    Twisted                                               -24805000
                                                            ...    
    Mission: Impossible - Ghost Protocol                  549713380
    Transformers                                          559709780
    Indiana Jones and the Kingdom of the Crystal Skull    601636033
    Transformers: Revenge of the Fallen                   686297228
    Transformers: Dark of the Moon                        928746996
    Name: profit, Length: 122, dtype: int64




```python
#Вопрос 19. Какой год стал самым успешным по суммарным кассовым сборам?

movie_bd.groupby(['release_year'])['revenue'].sum().sort_values(ascending=False).index[0]
#sort our dataset for release_year by revenue sum to find the most grossing year
```




    2015




```python
#Вопрос 20. Какой самый прибыльный год для студии Warner Bros?

warner_df = movie_bd[movie_bd.production_companies.str.contains('Warner Bros')]
#creating the new dataset with films that was created by Warner Bros by finding production_companies that contains this name
warner_df.groupby(['release_year'])['profit'].sum().sort_values(ascending=False).index[0]
#sort our dataset for release_year by profit sum to find the most profitable year for Warner Bros
```




    2014




```python
#Вопрос 21. В каком месяце за все годы суммарно вышло больше всего фильмов?

month_df = movie_bd.copy() #creating the new dataset
month_df['release_date'] = pd.to_datetime(month_df['release_date'], format = '%m/%d/%Y')
#give the data formate to release date column
month_df.release_date = month_df.release_date.apply(lambda x: x.strftime('%B')) #transform date to the non-number months 
month_df.groupby(['release_date'])['original_title'].count().sort_values(ascending=False)
#sort our dataset for release_date by original_title to find in which month the most films were released for all years
```




    release_date
    September    227
    December     190
    October      186
    August       161
    March        156
    April        149
    June         147
    November     146
    July         142
    May          140
    February     135
    January      110
    Name: original_title, dtype: int64




```python
#Вопрос 22. Сколько суммарно вышло фильмов летом (за июнь, июль, август)?


sdata = month_df.groupby(['release_date'])['original_title'].count().sort_values(ascending=False)
summer_df = sdata.reset_index() #creating the new dataset with from the data in the previous step, months and titles
summer_df[(summer_df.release_date == 'June') | (summer_df.release_date == 'July') | (summer_df.release_date == 'August')].original_title.sum()
#finding how many films were released in summer for all years

```




    450




```python
#Вопрос 23. Для какого режиссера зима — самое продуктивное время года

winter_df = month_df.copy()#creating the new dataset
winter_df[(winter_df.release_date == 'December') | (winter_df.release_date == 'January') | (winter_df.release_date == 'February')].director.str.split('|').explode().value_counts()
#finding how many films were released in winter for all years by directotrs, wivh were deviding by symbol and expand the resulting lists using the explode function
```




    Peter Jackson        7
    Clint Eastwood       6
    Steven Soderbergh    6
    Adam Shankman        4
    Martin Scorsese      4
                        ..
    Richard Loncraine    1
    MÃ¥ns MÃ¥rlind       1
    Ericson Core         1
    Mennan Yapo          1
    Tyler Gillett        1
    Name: director, Length: 358, dtype: int64




```python
#Вопрос 24. Какая студия даёт самые длинные названия своим фильмам по количеству символов?


filmLen_df = movie_bd.copy()#creating the new dataset
filmLen_df['length_title'] = filmLen_df.original_title.str.len() #creating the new column with the lenght of the film titles
filmLen_df['production_companies'] = filmLen_df.production_companies.str.split('|') #deviding production companies by symbol
filmLen_df2 = filmLen_df.explode('production_companies') #expand the resulting lists using the explode function
filmLen_df2.groupby(['production_companies'])['length_title'].mean().sort_values(ascending=False)
#sort our dataset for production_companies by length_title to find in which company usualy gives the biggest names for the film

```




    production_companies
    Four By Two Productions       83.0
    Jim Henson Company, The       59.0
    Dos Corazones                 47.0
    Museum Canada Productions     46.0
    Polsky Films                  46.0
                                  ... 
    Everest Entertainment          3.0
    Berlanti Productions           3.0
    XM2 Productions                2.0
    Ixtlan Productions             2.0
    Global Entertainment Group     2.0
    Name: length_title, Length: 1771, dtype: float64




```python
#Вопрос 25. Описания фильмов какой студии в среднем самые длинные по количеству слов?

overviewLen_df = movie_bd.copy() #creating the new dataset
overviewLen_df['length_overview'] = overviewLen_df.overview.apply(lambda x: len(x.split())) 
#creating the new column with the lenght of the amount of words in the overview by deviding overview by symbol and using lambda to count the amount of words 
overviewLen_df['production_companies'] = overviewLen_df.production_companies.str.split('|') #deviding production companies by symbol
overviewLen_df2 = overviewLen_df.explode('production_companies') #expand the resulting lists using the explode function
overviewLen_df2.groupby(['production_companies'])['length_overview'].mean().sort_values(ascending=False)
#sort our dataset for production_companies by llength_overview to find in which company usualy gives the biggest overviews by words ammount


```




    production_companies
    Midnight Picture Show                    175.0
    Room 9 Entertainment                     161.0
    98 MPH Productions                       159.0
    Heineken Branded Entertainment           159.0
    Brookwell-McNamara Entertainment         156.0
                                             ...  
    London Boulevard                          13.0
    Phantom Four                              13.0
    Henceforth                                13.0
    Empire Pictures                           11.0
    Motion Picture Corporation of America     11.0
    Name: length_overview, Length: 1771, dtype: float64




```python
#Вопрос 26. Какие фильмы входят в один процент лучших по рейтингу?

raiting_df = movie_bd.copy()#creating the new dataset
raiting_df.groupby(['original_title'])['vote_average'].max().sort_values(ascending=False).head(18) 
#sort our dataset for original_title by vote_average to have it from the biggest to smallest
#then take the first 19 because it will be 1percent of the top rated films 
```




    original_title
    The Dark Knight                                  8.1
    The Imitation Game                               8.0
    Inside Out                                       8.0
    Interstellar                                     8.0
    Room                                             8.0
    The Grand Budapest Hotel                         7.9
    The Pianist                                      7.9
    Guardians of the Galaxy                          7.9
    Memento                                          7.9
    The Wolf of Wall Street                          7.9
    Inception                                        7.9
    Gone Girl                                        7.9
    12 Years a Slave                                 7.9
    The Lord of the Rings: The Return of the King    7.9
    Prisoners                                        7.8
    The Fault in Our Stars                           7.8
    Eternal Sunshine of the Spotless Mind            7.8
    The Prestige                                     7.8
    Name: vote_average, dtype: float64




```python
#Вопрос 27. Какие актеры чаще всего снимаются в одном фильме вместе?

#import libraries
from collections import Counter
from itertools import combinations

actorsBFF_dt = movie_bd.copy() #make copy of our dataframe
pairs = Counter() #introduce the variable pairs
for i in range(0, len(actorsBFF_dt)):
    actors = actorsBFF_dt.cast[i].split('|') #devide our cast by symbol for separate actors repeat it for all cast cells
    for j in list(combinations(actors, 2)): #making pairs from the actors
        if j not in pairs:
            pairs[j] = 1 #if actors not in pair, nothing changes
        else:
            pairs[j] += 1 #if actors in pair, we increase the frequency of actors playing together for 1
pairs.most_common(5)
#finding 5 most common pairs
```




    [(('Daniel Radcliffe', 'Rupert Grint'), 8),
     (('Daniel Radcliffe', 'Emma Watson'), 8),
     (('Rupert Grint', 'Emma Watson'), 7),
     (('Ben Stiller', 'Owen Wilson'), 6),
     (('Johnny Depp', 'Helena Bonham Carter'), 6)]




```python

```


```python

```
