<h1> Assigment A2 : Bias in Data</h1>

<h3>The objective of this analysis to determine whether the Wikipedia Talk corpus contains bias or the characteristics of that bias and highlight its potential consequences</h3>

Data source link (Figshare datasets) - https://figshare.com/projects/Wikipedia_Talk/16731

Detox wiki page - https://meta.wikimedia.org/wiki/Research:Detox

Perspective API repository on GitHub - https://conversationai.github.io/

For the purpose of this analysis, I have only utilized Aggression Datasets

<h3> EDA included investigating following questions:</h3>
<ul>
    <li> Is there a bias in dataset from age-group represenatin perspective? And is there a difference between average aggression scores provided by crowdworkers in different age-groups?</li>
<li> Is there a bias in dataset from English language preference perspective? And is there a difference between average aggression scores provided by crowdworkers who have english language as their first language vs who don't? </li>
    </ul>

<h3> Results </h3>
<ul>
    <li>Distribution of age-group in aggression dataset suggests that crowdworker age-group was biased towards young age-group as we see 48% of crowdworkers belonging to age-group '18-30' years. This could potentially introduce bias due to theor view in political, gender, age or sexual orientation</li>
    <li>the distribution of average aggression rating among different age groups , we notice that over 60 age group is more biased towards rating comment as aggressive , whereas age group '18-30' seems pretty balanced in the rating spectrum. </li>
    <li>Distribution of comments rated by crowdworkers according to their first language, we notice that 86% of workers do not have english language as preffered language and since all the comments are english language, their could potentially be a lot bias introduced due to technical aspects of language and various perspective differences</li>
    <li>When combining both age group and forst language, we can clearly observe that first language plays a major role in extreme age buckets 'Under 18' and 'Over 60'. The Mean aggression score for these groups are very different on the basis of their first language</li>
    </ul>
    
<h3> Implications> </h3>
Potential bias introduced by the inaccurate sampling of crowdworkers which are not representation of true population can introduce a lot of bias into the system. Skewed annotator population i.e. demographics of crowd-workers might impact rating due to bias in political, gender, age or sexual orientation. Also, Topic biasing in the data - if all examples of a particular topic were rated as toxic by crowd-workers, the trained model will always consider comments related to that topic biased. This type of bias would be especially likely for controversial topics. Moreover the model will not performe well when- 
<ul>
<li>When language is not English -  The dataset is based on English language, hence any model trained on this data cannot be applied to other languages. This is a very big limitation as only less than 5% of the world population has English as their native language.</li>

<li>Identifying the sentiment of the user - As the dataset is customised to identify aggression, the model based on this data may not perform very well in identifying the sentiment of a comment, i.e whether the comment is in favour or against the premises. For example, a sports team may want to identify whether the user commenting on their website is a fan of their team or not. Since fans can be aggressive both while defending or attacking the team, the model based on this data may not be able to make that distinction. </li>

<li>Identifying virality and controversial nature - Many of the NLP models used in media are focussed on identifying the topics which are controversial or have the potential to become viral. This dataset does not have enough depth to support these use cases. </li>
 </ul>
