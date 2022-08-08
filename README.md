# MichaelScottvisualization
This is visualisation of the character from the tv show "The Office" - "Michael Scott"

I've decided to analyze main character of the great show - ‘Michael Scott”<br>
For the next visualizations I have used few datasets, that I get from kaggle.<br>
First dataset providing spoken text lines during the show for all characters. There are 5 attributes:
<ul>
  <li>index</li>
  <li>character</li>
  <li>line</li>
  <li>season</li>
  <li>episode_number</li>
</ul>
While working with this dataset I have found that some eposides have been missing, but amount of the lost episodes is small enough for continue working with this dataset. </br>
Second dataset gibe us more general information, such as title of the episode, director, writers, original air date.The attributes for this dataset are:
<ul>
  <li>season</li>
  <li>episode number of season</li>
  <li> episode number in series</li>
  <li>title of the episode</li>
  <li>director</li>
  <li>writers</li>
  <li>original air date</li>
  <li>production coded</li>
  <li>US viewers on orignal air date</li>
</ul>
As for the third dataset it's pretty much the same as the second one this dataset providing general information. The only attributes, that we are looking for is **Average IMDd rating**.
For connection of all of those dataset I joined using two attributes - ***'season***' and ***'episode number'*** <br>
Because data, that have been provided can’t be directly used for the questions,that I want to answer,I had to preprocessed it. Because I wanted to see the appearance of the famous Michael Scott line ***‘That’s what she said’*** during the show, I had to store in which episodes are this line appeared and who said that with use of first dataset. As a result we have dataset that provide to us every appearance of this line during the show with next attributes:
<ul>
  <li>season</li>
  <li>episode</li>
  <li> character</li>
</ul>. 
Also using first dataset, I have counted amount of lines from Michael Scott during the show. As a result I had dataset with next attributes:
<ul>
  <li>season</li>
  <li>episode</li>
  <li> Michael count (count of Michaels line in this episode)</li>
As for my first visualisation “‘that’s what she said’ line” I used ‘season’ as column and ‘episode’ and ‘character’ as rows. To separate Michael from other characters, I’ve made a set with this character and used it as a marks. The visualisation is a Gantt one.

<img width="620" alt="Screenshot 2022-08-04 at 17 30 42" src="https://user-images.githubusercontent.com/46090129/182814212-21831223-727d-4c64-8b3d-63f251f9c9d3.png">

For the second visualisation - “Michael appearance during the show” I used ‘Season’ as a column, and sum of Michael lines for the seasons with sum of US viewers as a rows. Also I’m marking median IMBd rating for the each season. The plot type is dual lines.

<img width="555" alt="Screenshot 2022-08-04 at 17 32 04" src="https://user-images.githubusercontent.com/46090129/182814446-d8440854-7674-45e1-9153-faa49017918b.png">

For the last visualisation I’ve made text visualisations using “character” attribute from the ‘the-office-lines’ dataset.
<img width="610" alt="Screenshot 2022-08-04 at 17 32 30" src="https://user-images.githubusercontent.com/46090129/182814697-ce5692e6-67b6-4f5c-90b3-248ea891a7e9.png">



