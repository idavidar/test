# US Abortion Debate: how do different groups frame the 'abortion issue'?
Group project in Digital Methods by Ida Vidar Kristensen, Faridoddin Pesteh and Ana Radomirescu
## Introduction
2022 has been a tumultuous year for the abortion debate in America. With the Supreme Court overturning *Roe v. Wade* in June this year, a ruling that provided the constitutional right to abortion, the legal battle has [shifted to individual states](https://apnews.com/article/supreme-court-abortion-ruling-states-a767801145ad01617100e57410a0a21d). As of 12 December 2022, [13 states instituted total abortion bans and many others have tightened their abortion policies](https://www.nytimes.com/interactive/2022/us/abortion-laws-roe-v-wade.html). Groups on both sides of the debate have fiercely campaigned and [protested](https://en.wikipedia.org/wiki/2022_abortion_protests) for their causes.

The timeline of the main events: 
- 1973: The US Supreme Court decision on *Roe v. Wade* made abortion a constitutional right throughout the US.
- 2022, May 3rd: a leaked draft majority opinion of the Supreme Court in *Dobbs v. Jackson* indicated that the Court would overturn *Roe*.
- 2022, June 24th: *Roe v. Wade* overturned by the Supreme Court: abortion is no longer a constitutional right.

Our group project analyses how different groups/organizations in the United States discussed and framed the 'abortion issue' on Twitter, specifically since the leaked Supreme Court draft opinion on *Dobbs v. Jackson* which sought to overturn *Roe*. We looked at American groups that fight for a variety of social issues to see how they framed the subject. First and foremost, we were interested in the framing differences between pro-choice and pro-life groups (which clearly have different stances on the matter). Further, we wanted to see how other relevant equity-seeking groups and religious groups frame the issue of abortion: whether their chosen framing promotes and reflects their stance on the social issue that is their main focus, and whether or not certain groups use similar framing.

We chose to examine the tweets of 5 types of groups, and selected 10 organizational accounts representing each group (except the minority group, where we only found 8 accounts that were sufficiently diverse, relevant and active, so we had 48 accounts in total):
- Pro-Choice groups (pro-abortion)
- Pro-Life groups (anti-abortion)
- LGBTQ2S+ groups (organizations seeking equity for people with different sexual orientations, genders etc.)
- Racial minority groups (organisations that fight for the rights of African-Americans, Latino-Americans and Asian-Americans)
- Christian religious groups (Catholics, Protestants, and Mormons).

<img width="1257" alt="Skærmbillede 2022-12-18 kl  14 20 26" src="https://user-images.githubusercontent.com/115983285/208300656-78315994-0af4-4baf-ace7-aeb8265f35fb.png">

![New Project](https://user-images.githubusercontent.com/115983448/208984994-1c631d35-1c3e-43f9-9a78-a135bb66c8ba.png)


### Hypotheses
We had multiple preliminary expectations of the outcomes of our analysis.

First, we expected the pro-choice and pro-life groups to use different terms and hashtags to frame the abortion debate, with the exception of neutral terms like ‘Roe v. Wade’ and ‘Supreme Court.’ This is because pro-choice groups support abortion rights, with few or no limits, and are therefore likely not to discuss abortion in a negative way, whereas pro-life groups oppose abortion rights, with few or no exceptions, and are therefore likely to paint abortion in a negative light.
* _H1_ (pro-choice/pro-life)_: the pro-choice and pro-life groups use different terms and hashtags to frame the abortion debate, with the exception of neutral terms like ‘Roe v. Wade’ and ‘Supreme Court.’_

Second, we expected LGBTQ2S+ groups and minority groups to use similar terms in their tweets as the pro-choice groups use, whereas the Christian religious groups to use words common in both the pro-choice and the pro-life groups. Regarding LGBTQ2S+ groups, many are likely to [fear that the removal of the constitutional right to abortion may lead to a rollback of the rights of LGBTQ2S+ people, including that of same-sex marriage](https://www.pbs.org/newshour/politics/after-supreme-court-abortion-decision-some-fear-rollback-of-lgbtq-and-other-rights), although it should be noted that there are [some LGBTQ2S+ people that clearly are anti-abortion](https://www.nbcnews.com/nbc-out/out-news/anti-abortion-lgbtq-groups-roes-reversal-human-rights-victory-rcna35716). Regarding minority groups, they are likely to fear that the removal of the constitutional right to abortion [disproportionately affects minorities, as these groups are more likely than others to be those receiving abortions](https://www.pbs.org/newshour/nation/black-and-hispanic-people-have-the-most-to-lose-if-roe-is-overturned). In contrast, there are both Christian religious groups that [support and others that oppose abortion rights](https://www.pewresearch.org/fact-tank/2016/06/21/where-major-religious-groups-stand-on-abortion/).
* _H2_ (affinities)_: LGBTQ2S+ and minority groups use similar terms in their tweets as the pro-choice groups use, whereas the Christian religious group uses words common in both the pro-choice and the pro-life groups._

Furthermore, given that the non-abortion-focused groups (LGBTQS2+, minority and Christian religious) have a different main focus, we expect them to mix their own-issue-specific terms and hashtags with those used by pro-choice and pro-life groups.
* _H3_ (themes)_: the non-abortion-focused groups (LGBTQS2+, minority and Christian religious) will include their own-issue-specific terms and hashtags in their tweets on abortion._

Finally, we expect the non-abortion-focused groups to mostly tweet about abortion on the day of the leaked Supreme Court opinion draft and on the day of the Dobbs decision that overturned Roe, but very little otherwise. This is because the 'abortion issue' is not the main, direct focus area of the organizations that are not in the pro-choice and pro-life groups, so they are likely to seldom tweet about abortion unless there are big events that attract attention to this issue.
* _H4_ (temporal)_: non-abortion-focused groups mostly tweet about abortion on the day of the leaked Supreme Court opinion draft and on the day of the_ Dobbs _decision that overturned_ Roe, _but very little otherwise._


## Data Collection
### Search query
We chose to collect data from Twitter, a popular social media platform, because i) we expect the subject of abortion to be heavily discussed there, ii) the types of groups we chose to analyse are often very active on this platform, and iii) their interactions are public. We scraped our data using minet.

Below is an example of the search query we used (in this case, for the pro-choice group):

```
! minet tw scrape tweets '(abortion OR roe OR pro-life OR pro-choice OR reproductive OR birth OR pregnant OR pregnancy) 
from:@NARAL OR from:@PPFA OR from:@NatAbortionFed OR from:@NationalNOW OR from:@ACLU OR from:@ReproRights OR 
from:@AbortionFunds OR from:@PPact OR from:@womensmarch OR from:@nwlc lang:en until:2022-11-16 since:2022-05-01' 
> tweets_abortion_pro-choice.csv
```

- Words included in the query: We needed to strike a balance between capture as many of the tweets related to the abortion debate made by these accounts as possible, while not capturing irrelevant tweets. We did this by including terms that were obviously linked to the abortion debate, such as "abortion" and "Roe" (referring to _Roe v. Wade_), but also more general words (birth, pregnant etc.) that we assumed to be related to this debate in our specific time period. We refined our query by making several changes, for instance by removing "Supreme Court" from the query, since we noticed that some of the tweets extracted when querying this term referred to other decisions made by the Supreme Court which were not related to abortion. Based on the qualitative checks of tweets we collected, we felt quite confident that the words remaining in our query provided us with most of the tweets relevant for our project. 
- Time period: We chose to scrape data spanning a period of 7 months, from a couple of days before the leak of the Supreme Court draft opinion on _Dodd_ (start date: May 1st, 2022) until the day of our analysis (end date: November 16th, 2022). We chose this extended time period beyond the date when _Roe_ was overturned in order to be able to analyse the post-decision debate too, and see if there were some interesting developments over time. Further, abortion resurfaced as an important issue during the US Midterm election season in November. 
- Language: We scraped and analysed tweets written only in English.

### How did we choose our groups?
Our choice of Twitter accounts within each of our 5 different groups was dependent on several things. We searched the internet for relevant and widely-known United States groups/organizations within each of our 5 groups. We then searched for these groups on Twitter and looked at a number of relevant factors, most importantly how many followers they had and how active they had been on Twitter in our time period (prioritizing accounts that actually Tweet in order to give us more data). We then chose the top 10 Twitter accounts to include within each of our groups (e.g. pro-choice, LGBTQ2S+, etc - aside from minority group where we had only 8). The selection of our total of 48 Twitter accounts gives us a corpus of roughly 10,000 tweets, with a distribution as in the table below:

<img width="604" alt="Skærmbillede 2022-12-20 kl  10 12 35" src="https://user-images.githubusercontent.com/115983285/208628898-42166c24-0ad2-437b-9531-3621e38e28ef.png">

- The size of the corpus of each group varies, and some of the corpuses are very small. Of course, both the pro-choice and pro-life groups tweeted a lot on the issue of abortion within our time period, since abortion is their main policy-focus (5672 and 3750 tweets respectively), and our search query captures around 50-60% of these groups' total tweets in this period.
- The other groups (LGBTQ2S+, minority, and Christian religious groups) made very few tweets about the abortion issue within the chosen time period - these tweets only make up about 5-6% of the total number of tweets within this time period from the accounts. This is to be expected, since the 'abortion issue' is not the main, direct focus area of these organizations, so they are likely to seldom tweet about abortion unless there are big events that attract attention to this issue, such as the overturning of _Roe v. Wade_ (in which case we would expect them to tweet about this issue on this day, but not very much afterwards). 

## Analysis approach

We conducted the our corpus analysis in CorText. Our analysis consists of two main parts. In the first part we worked with the 5 data corpuses from our 5 different groups separately. Within each of these 5 corpuses we conducted several analyses to shed light on the way each group framed the 'abortion issue.' We first extracted the most frequently used 10 terms and 10 hashtags by each of these groups in their tweets about abortion. When extracting the terms, monograms were forbidden in order to have phrases, which are more interesting in giving a clearer picture of framing, otherwise we would  see single words like 'abortion' that give little insight. We also put together different forms of  clearly-connected terms (such as 'overturning roe,' 'overturning of roe', 'overturned roe,' etc.) under the same main form (partly this was done automatically, partly manually) in order not to have duplicates. We also extracted the 10 most-liked tweets in each of the corpuses. These results will be presented below for each group separately and will shed light on how the different groups discuss and frame the abortion debate. It will allow us to test hypotheses H1, H2 and H3. Furthermore, we conduct a temporal analysis that tests H4.

In the second part of our analysis we combined the 5 corpuses together into one corpus, in order to focus specifically on the connections between groups. Using this combined corpus we conducted a network analysis and a contingency matrix.


## Empirical results
### Pro-Choice groups
#### Most frequent terms

<img width="655" alt="Skærmbillede 2022-12-17 kl  18 04 55" src="https://user-images.githubusercontent.com/115983285/208253136-af2286ef-078b-4545-a624-8248cabff9ee.png">

When looking at the top 10 most frequently used terms in the tweets from the pro-choice groups, they naturally first and foremost refer to _Roe v. Wade_, the fact that an "abortion ban" will be passed in several states, and also mention the "Supreme Court". Hereafter, it is worth noticing that the abortion issue is almost always mentioned using the terms "rights", "freedom" or "care". This shows that they strongly frame the issue of abortion as a fundamental human right, and that they believe that the overturning of _Roe_ will have consequences for both the care and health of pregnant women. All in all, these terms highly align with the expected stances of pro-choice groups. In fact, pro-choice groups often prefer to be called Pro-Reproductive Rights, since they find this term [less polarizing](https://www.plannedparenthood.org/learn/ask-experts/can-you-explain-what-pro-choice-means-and-pro-life-means-im-supposed-to-do-it-for-a-class-thanks). This is also reflected in their most frequently used terms, where the word "reproductive" recurs several times. 

#### Most frequent hashtags

<img width="646" alt="Skærmbillede 2022-12-17 kl  18 04 41" src="https://user-images.githubusercontent.com/115983285/208253157-859ce3c2-b842-4db2-94ef-bdc788b01057.png">

In the top 10 most frequent hashtags from the pro-choice groups there is again a clear focus on freedom, which is an aspect of the abortion discussion that pro-choice groups find essential and often highlight. This recurring theme can be seen in the 3 most frequent hashtags #fightbackforfreedom, #bansoffourbodies and #reprofreedomvoter. Again there are also some hashtags clearly linking the tweets to the _Roe_ case (#scotus, #roevwade and #roe). 

One of the most frequently used hashtags is #whpa which refers to the so-called [Women's Health Protection Act](https://actforwomen.org/the-womens-health-protection-act/). The WHPA is a piece of federal legislation proposed by the House of Representatives multiple times the last 10 years that seeks to expand the abortion rights established in _Roe_ by protecting the right to access abortion care throughout the US, even in case _Roe_ is overturned. The WHPA was proposed by Democrats in the House and passed through the House (which had a Democratic majority) in early 2022, but was rejected by the Senate (which did not have a Democratic majority) both in February and on May 3rd, 2022 - the same day of the leaked draft opinion of the Supreme Court. Pro-choice organizations used this hashtag in tweets both at the time when the WHPA was blocked by the Senate, but also subsequently, throughout our entire period of analysis, in order to highlight the importance of voting for the Democrats in the midterm elections in November 2022, since this could flip the majority in the Senate in the Democrats' favour, making it possible to pass the WHPA. This is illustrated in the following tweet from NARAL Pro-Choice America on July 15th:
- “These anti-choice Republicans just voted against #WHPA. We know who’s to blame for this abortion access crisis—and we won’t forget in November. Join us and help mobilize #ReproFreedomVoters across the country”

#### Top tweets

The picture below illustrates 4 of the top 10 most-liked tweets from the pro-choice corpus. These 4 tweets mirror the framing of the issue found in the terms and tweets above, but also illustrate the different events that occurred during our chosen time period of analysis. The tweet by Planned Parenthood (bottom right) is made on the very day where the leaked draft Supreme Court opinion came out, which implied that an overturn of _Roe_ was likely. Here, Planned Parenthood is trying to inform people that it is still possible to access abortions, and where to find help. The two tweets in the top are both from the day _Roe_ was overturned, and therefore have a much more angry and indignant tone. The last tweet chosen in the bottom left is from the end of our time period (November) and shows the effects of overturning _Roe_, where the various states suddenly had to make their own laws on abortion.


<img width="857" alt="Skærmbillede 2022-12-18 kl  12 13 30" src="https://user-images.githubusercontent.com/115983285/208295198-8cfae82b-c50b-45a8-841b-98f6ed2ec5f8.png">

### Pro-Life groups
#### Most frequent terms

<img width="647" alt="Skærmbillede 2022-12-17 kl  18 04 09" src="https://user-images.githubusercontent.com/115983285/208253169-e38a575e-1f43-4544-8668-7c8c01d2c6bc.png">

When looking at the 10 most frequent terms used by the pro-life organisations it is clear that their framing of the abortion issue is, as expected, highly different from the pro-choice groups. Instead of framing abortion in terms of "rights" and "care," as the pro-choice groups do, the pro-life organizations use terms such as “abortion extremism,” “abortion industry” and "abortion on demand," suggesting that the abortion rules had spiralled out of hand, and that it was inappropriately easy to access abortion "on demand." This is in line with hypothesis H1. 

Interestingly, there is also a frequent mention of Planned Parenthood, suggesting a clear targeting of the organization by pro-life groups. 

The most frequently used term by these group is "pregnancy centers" which refers to pregnancy resource centers (sometimes also known as pro-life pregnancy centers), established by anti-abortion groups to persuade pregnant women to chose other options than abortion by providing support, guidance, diapers etc. In pro-life group tweets, these centers are often mentioned as a response to the criticism that 'pro-lifers' do not give options to pregnant women. In relation to this, a lot of these tweets also refer to specific situations where pro-choice demonstrators have blocked or vandalized these pregnancy centers around the US, as a reaction to _Roe_ being overturned. A last term worth mentioning is "human life," which is also key to understanding the different stances of the pro-choice and pro-life organizations. An important argument for the pro-life stance is that an unborn foetus should be considered a human life with rights on equal terms with the pregnant mother already from conception. 

#### Most frequent hashtags

<img width="655" alt="Skærmbillede 2022-12-17 kl  18 10 14" src="https://user-images.githubusercontent.com/115983285/208253328-e35d2481-ea5c-411b-a510-0ea9ee6dff37.png">

The framing discerned from the above-mentioned terms list is further elucidated when looking at the top 10 hashtags. Here it is even clearer that the pro-life groups indeed see the abortion issue as a matter of protecting the rights of the unborn humans with the hashtags #prolife, #lifeisahumanright and #lifewins22. Both the pro-life and the pro-choice groups refer to rights when discussing the subject, but focus on rights for different groups of people (unborn children vs mothers). 

The hashtag [#cantstaysilent](https://www.cantstaysilent.com) is used as part of a movement where pro-life organizations encourage women who have earlier had an abortion (often forced by their partners, families etc.) to share how this has affected their life and the regret and trauma it has caused them. An example of such a tweet can be seen below, where a woman uses her abortion story to try to convince others to give their babies up for adoption instead of having an abortion:
- "I had an abortion with my first pregnancy on October 26, 1985. I had it on a Saturday morning & then went to my cousin's wedding that evening!! Since my abortion I had two other children, a girl and a boy, and I…put both of them up for adoption. I am 58 years old now. My birth daughter is 32, and my birth son is 31, & I keep in touch with both of them. I can't tell you the joy I feel over seeing my 2 birth children, & the depression I feel (& the tears I have cried) over the one child I aborted. #CantStaySilent"

The rest of the most frequent hashtags are primarily references to the Supreme Court cases (#scotus, #supremecourt, #roevwade and #dobbsvjackson). 

#### Top tweets

The picture below illustrates 3 of the 10 most-liked tweets on the abortion issue by the pro-life groups. As was evident in both the terms and the hashtags, here it is also clear in the tweet by Students for Life of America that they see the fact that _Roe_ was overturned as a victory and something to celebrate. In addition to this, the tweet from March for Life also shows that a great deal of the communication in the debate is directed towards the opposing pro-choice groups. A frequently used pro-abortion argument is that abortion and family planning make it easier for women to pursue education and career opportunities, since they would not be forced to stay at home with their children. However, in this tweet, March for Life tries to counter-argue this classic feminist argument by saying that women can easily be successful without having abortions. 

<img width="923" alt="Skærmbillede 2022-12-18 kl  14 07 46" src="https://user-images.githubusercontent.com/115983285/208300109-1a4fc67e-6da0-440c-8fcf-fdceb8d5c25f.png">

### Minority groups
#### Most frequent terms

<img width="645" alt="Skærmbillede 2022-12-17 kl  18 24 56" src="https://user-images.githubusercontent.com/115983285/208253899-cf40f88b-75f8-4f6d-8199-b6a222514890.png">

We are now turning towards the 10 most frequently used terms by the organizations fighting for racial minorities. At first sight, we see that these racial equity seeking groups use a framing much more similar to the pro-choice groups than the pro-life groups, since they also have several terms that refer to abortion as a 'rights issue' and also often mention the subsequent “abortion bans” that were instituted in many states since _Roe_ was overturned. This is consistent with hypothesis H2. In addition to this, consistent with H3, it appears that these groups do refer to the abortion issue in a way that links back to, and further emphasises, the issues they normally focus on - in this case racial equality and the treatment of minorities. This is clearly seen from the fact that some of the most frequently used terms are “Black people”, “Black women” and “racial justice issue.” They specifically frame the abortion issue as an important issue for the black community and black women. 

#### Most frequent hashtags

<img width="638" alt="Skærmbillede 2022-12-17 kl  18 26 48" src="https://user-images.githubusercontent.com/115983285/208253974-e8fddf20-0d67-4ca4-b85e-a085f47f9cfa.png">

Within the 10 most frequently used hashtags by these groups supporting racial minorities are some of the same hashtags used by the pro-choice groups, namely #bansoffourbodies, in line with H2. In general, these minority groups strongly emphasise the right to make decisions about one's own body, clearly shown in several other top hashtags such as #liberatedbodies and #bodilyautonomy. Although not as evident as in the terms list, the racial equity agenda is also represented in the hashtags through #aapi, which stands for Asian Americans and Pacific Islanders, who are specifically mentioned in some of the tweets, such as the one below:
- "#ReproductiveRights are a civil & human right. This is all our responsibility.At @NAPAWF & @EthnicMediaSvc's briefing, our President & Executive Director @johncyangdc discussed what is at stake for the #AAPI community if Roe v. Wade is overturned"

Furthermore, the hashtag #nodataforcops illustrates that these groups have a focus on protecting the racial minorities from discrimination in relation to the abortion issue. The tweets using this hashtags argue that the 'big tech' companies should ensure that the police are not able to access data on which women are pregnant or have previously had abortions, since this can lead to further discrimination, especially of racial minority women. Here, the organizations' primary focus on racial equity is again very clear, in line with H3. 

#### Top tweets

Below we show 3 of the 10 most-liked tweets made by these minority groups on the abortion issue. Generally, the indications from the terms and hashtags that these groups have a similar stance on the abortion debate as pro-choice groups are confirmed when looking at the tweets. All 3 tweets indicate fear of harm and concern with the Supreme Court’s decision. 2 of the 3 tweets clearly frame the issue in relation to the rights of Black Americans and how the Supreme Court's decision will especially affect this group, but, as the bottom-left tweet indicates they also highlight how it will affect other minority groups, in this case sexual minorities. 

<img width="1040" alt="Skærmbillede 2022-12-18 kl  15 34 15" src="https://user-images.githubusercontent.com/115983285/208304232-567a4f54-c8b8-4e0a-9053-12ef3464f41a.png">

### LGBTQ2S+ groups
#### Most frequent terms

<img width="628" alt="Skærmbillede 2022-12-17 kl  18 30 28" src="https://user-images.githubusercontent.com/115983285/208254176-f4005100-2fbb-489e-933b-5b5a983d94a7.png">

We now turn towards the 10 most frequently used terms by the LGBTQ2S+ groups that fight for the rights of people with different sexualities, genders etc. The framing of the abortion issue by these groups is highly aligned with that of the pro-choice groups, consistent with hypothesis H2, since 7 of the 10 terms overlap between the groups. Like the pro-choice groups, and also the racial minority groups, they frame the abortion issue in terms of “rights,” “care” and “health.” They clearly perceive abortion as an indisputable “reproductive right,” important for health concerns. Just like the racial minority groups, LGBTQ2S+ groups also have some group-specific terms on their top 10 list, namely “trans people” and “LGBTQ+ rights.” This again shows that these groups talk about the issue in a way that highlights their own target audience and how they will be affected by _Roe_ being overturned, consistent with H3. 

#### Most frequent hashtags

<img width="619" alt="Skærmbillede 2022-12-17 kl  18 33 19" src="https://user-images.githubusercontent.com/115983285/208254182-69ad3cb1-e279-4a38-b421-82c37d5dc24c.png">

When looking at the 10 most frequent hashtags of the LGBTQ2S+ groups there is a notable overlap with the pro-choice and racial minority groups in the use of the #bansoffourbodies hashtag. These groups also use the #WHPA (referring to the Women Health Protection Act previously mentioned). However, most of the hashtags used by the LGBTQ2S+ organisations are group-specific and refer to the group’s primary cause, consistent with H3 (#lgbtq, #transgender, #queeringrepro and #nonbinary). A lot of the tweets using the aforementioned hashtags mention the fact that the organizations are fearful that the Supreme Court's decision to overturn _Roe_ will be followed by other more conservative legislation that will deprive LGBTQ2S+ people of other reproductive rights such as fertility treatment. This is, for instance, seen in the tweet below:
- "Repro tech is at risk for LGBTQ families!🔬 State Senator @ZachWahls tells us about how his two moms used artificial reproductive technology (ART) to have children and create a family.🟣 Why do you think politicians are trying to put an end to LGBTQ families?"

Thereby, the abortion debate is both relevant for these groups because they fear for the rights and health of LGBTQ2S+ people who are pregnant, but also because they fear other restrictions on LGBTQ2S+ rights in the future. 

#### Top tweets

Below are 3 of the 10 most liked tweets from these groups on the abortion issue. From these tweets it is also evident that the LGBTQ2S+ groups  definitely see the abortion issue as an issue for their target group. As mentioned in the hashtag section, the groups are also worried how this will affect future Supreme Court decisions on LGBTQ2S+ people’s rights. For example, the tweet on the right mentions that one of the Supreme Court justices, Justice Thomas, had spoken some [“alarming” words](https://outinjersey.net/what-happens-if-scotus-repeals-obergefell-v-hodges-when-court-resumes/) on other rulings (_Obergefell v. Hodges_ and _Lawrence v. Texas_). These rulings are essential for LGBTQ2S+ people’s guaranteed right to same-sex marriage. This tweets thus clearly shows that these groups see the abortion issue as an issue that can lead to other subsequent negative effects on their target group in the future. 

<img width="944" alt="Skærmbillede 2022-12-18 kl  19 04 03" src="https://user-images.githubusercontent.com/115983285/208312356-a1f62b92-51e5-49dc-9b89-ad29e57a21b0.png">

### Christian religious groups
We now turn to analyse the corpus of tweets from Christian religious groups. We chose to focus on Christian groups only for three reasons. First, Christianity is the majority religion in the US ([around 70% of Americans are Christians](https://www.pewresearch.org/religion/religious-landscape-study/)). Second, we expected to see some interesting results with even just this seemingly narrow group, since even within Christianity there are [variations in religious groups' positions on abortion](https://www.pewresearch.org/fact-tank/2016/06/21/where-major-religious-groups-stand-on-abortion/). Third, what we wanted to analyse was not the language that these groups used because they aligned themselves explicitly with either the pro-choice or pro-life stand on abortion, but rather, to see if there is specific language that they use in framing 'abortion issue' because they are _religious_ groups. Given that our hypothesis is that they would use some religious-specific terms like "God" or "church," mixing together tweets in the same corpus from completely different religions would likely have created too much noise to see these specific terms and would not have added much to our analysis given that what we were looking for was the presence of religion-specific terms.

#### Most frequent terms

<img width="735" alt="Skærmbillede 2022-12-20 kl  15 37 58" src="https://user-images.githubusercontent.com/115983285/208692354-db96757c-8f22-45e2-b64a-748869bb7604.png">

When looking at the 10 most frequent terms used by Christian groups, we see some repetitions of terms used by both pro-choice and pro-life groups. This finding is as expected, since, as mentioned, Christian groups vary in their stand on the ‘abortion issue,’ and the corpus of tweets includes those with both pro-life and with pro-choice stands. For example, "support abortion" (a main form which in fact encompasses multiple similar phrases like "support abortion" and "support for abortion" and "abortion support") and "reproductive healthcare" are terms indicative of a pro-choice stance. The affinity with pro-life groups, on the other hand, can be seen most evidently from the fact that religious groups often mention the "pro-life movement" directly. Both Christian and pro-life groups also often mention "pregnancy centres" and "abortion extremism."

In line with our hypothesis, we also see some religious-themed terms, like "Catholic churches," however, not as many as we would have expected.

This is also the first time we see mention of "Joe Biden," which may suggest that the Christian groups are willing to politicise the issue of abortion in their discourse. However, it is likely to also be because one of our groups is CatholicVote, which is likely to be a more politically-active organisation than others in our sample, given that it is "[organized as a 501(c)4 grassroots lobbying organization with a connected political action committee … [that enables it to] lobby Congress in favor of (or against) legislation … [and] endorse (or oppose) candidates for elective office](https://catholicvote.org/mission-learn-more)."


#### Most frequent hashtags

<img width="735" alt="Skærmbillede 2022-12-20 kl  15 37 48" src="https://user-images.githubusercontent.com/115983285/208692307-12de284b-4690-4168-8f63-483b3990bd9f.png">


In contrast to the most frequent terms, the most frequent hashtags exhibit a clearer similarity with pro-life groups (rather than pro-choice) and more religion-themed terms. Most clearly, we see the #prolife hashtag mentioned often. Interestingly, these groups still want to frame themselves as being ‘pro’ something, reflecting the [change that the ‘pro-life’ movement itself undertook](https://en.wikipedia.org/wiki/United_States_anti-abortion_movement#History) from ‘anti-abortion’ to ‘pro-life,’ so they use the hashtags #prowoman and #profamily, both of which are associated with a pro-life, anti-abortion stance. We see many religious-themed hashtags, like ‘catholic’ and ‘rosary.’ Three other popular hashtags are:
- #sbc22, which stands for the [2022 annual meeting of the Southern Baptist Convention](https://sbcannualmeeting.net/events/) (held on 11-15 June, during our chosen time period for sampling),
- #ewtn (Eternal World Television Network) which is a Catholic television network,
- #pcusa (Presbytarian Church USA).
Although these are also technically religious-themed hashtags, they are better thought of as being the contexts for the tweets (in fact, ewtn and pcusa are two of the accounts whose tweets we are analysing, and probably hashtag themselves), rather than helping to elucidate the ways in which the religious groups frame the abortion issue.


#### Top tweets
Below are 3 of the 10 most liked tweets from Christian religious organisations on the abortion issue. They illustrate most clearly the way that these organisations use religious language when talking about the abortion debate - for example, “PRAISE GOD!” (right) and “Roe overturned on the day we celebrate the Sacred Heart” (top left).
The phrase “culture of life” is featured in the bottom-left tweet, and is common in tweets from Christian religious organisations and pro-life organisation. It is a term that [originated in moral theology, especially that of the Catholic Church, and refers to a belief that human life at all stages from conception to death is sacred](https://en.wikipedia.org/wiki/Culture_of_life) (thus, opposing abortion).

<img width="600" alt="Skærmbillede 2022-12-20 kl  15 30 15" src="https://user-images.githubusercontent.com/115983285/208690627-5c73fb8c-d43b-4a43-8e6d-903ba30addb2.png">


### Temporal analysis

![demography graph](https://user-images.githubusercontent.com/115983448/208968192-bf35fb7f-2fbd-4010-b1b3-cfbe344e876e.png)

The temporal graph shows the number of tweets made on the issue of abortion by the organisations in each of our 5 groups on each day. The numbers are in absolute values (not normalised) and not stacked. As expected, and as shown in our table above when introducing the groups, the pro-choice and pro-life groups have a much higher number of tweets on abortion than the other groups. Also as expected, there are peaks of the number of tweets on days with significant events relating to the issue of abortion, such as the leaked Supreme Court draft opinion on 3 May, the _Dobbs_ decision on 24 June and the midterm elections on 8 November where abortion was [one of the main campaign issues](https://www.nytimes.com/2022/11/10/us/abortion-ballot-midterm-elections.html).

In line with hypothesis H4, the graph shows that non-abortion-focused groups tweet very little on abortion other than around the main events of the leaked Supreme Court draft opinion and the _Dobbs_ decision. There is also a barely perceptible peak of tweets from these groups during the midterm elections, most likely because they have different issue areas that they focus on and want to campaign for.


### Network map

![Screenshot 2022-12-20 at 17 13 37](https://user-images.githubusercontent.com/115983448/208720616-9c83fd93-0392-437f-a1ff-d0b28f5f6842.png)

The network above is of all 5 groups together (pro-choice, pro-life, minority, LGBTQ2S+ and Christian religious). The nodes are terms and hashtags, from a combined list of 100 most frequently used terms and 100 most frequently used hashtags in the combined corpus. The number of nodes in the map was restricted to 100 in order to strike a balance between making the map feasible to interpret, and having too few nodes which would result in the joining together of clusters and thus losing important and interesting information. The 5 organisations best associated with each cluster are projected onto the map (an organisation is strongly associated with a cluster if its tweets feature a higher proportion of the terms/hashtags of that cluster than do the tweets of other organisations). In interpreting the map, there is a link (edge) between terms/hashtags if they are mentioned in a tweet together. The larger the size of a node, the more times that term/hashtag is mentioned in the complete corpus of tweets.

Some of the information shown in the network map mirrors what we found in the above analysis. It shows that pro-choice and pro-life organisations use different language when discussing the ‘abortion issue.’ This can be seen by the fact that the yellow and orange clusters are only associated with pro-choice organisations, whereas the turquoise and lime green clusters are only associated with pro-life organisations. 

The fact that NARAL is the only organisation associated with the orange cluster indicates that it has its own very specific way of framing the ‘abortion issue.’ Nevertheless, it is associated with the dark green cluster together with other organisations, showing that it does overlap with others in its framing, especially with regards to the Women Health Protection Act (to which all of #whpa, #actforabortionaccess and "health protection act" refer). It is interesting to see that LGBTQ2S+ organisations are associated with pro-choice organisations only in this dark green cluster, perhaps implying that the WHPA is one of the main issues of interest of these organisations. This mirrors our findings above, where the pro-choice and LGBTQ2S+ organisations were the only ones in which #whpa and "health care" featured in the top 10 hashtags and terms, respectively.

The red cluster is more difficult to interpret. At first glance it seems surprising that it is associated with both the pro-choice organisation 40 days for life, as well as minority, LGBTQ2S+ groups and the United Church of Christ which appears strongly [pro-choice](https://www.ucc.org/lets-talk-about-abortion/). We suspect this is because the cluster includes not only popular pro-life hashtags (#prolife, #abortionist) but also some neutral hashtags such as #abortion, #dobbsvjackson, #supremecourt and #scotus, which are probably used by both pro-life and pro-choice stances and therefore link otherwise opposing organisations together to this one cluster.

Finally, it is interesting to note the link between the pro-choice and pro-life clusters occurs through the node "dobbs decision." This makes sense, as it is both a neutral and a very important term, as both sides undoubtedly have a lot to say about the Supreme Court’s decision.



### Contingency Matrix (Top Terms vs. Hashtags)

<img width="783" alt="Capture d’écran 2022-12-22 à 06 52 12" src="https://user-images.githubusercontent.com/115983366/209066531-aa86ac7d-85d8-4340-8d88-e909e1cc3413.png">

The contingency matrix above showcases the joint distribution of the two variables, namely the top 10 terms and top 10 hashtags in the corpus. The corpus for this analysis was composed of the Tweets from all 5 groups (i.e. pro-choice, pro-life, LGBTQ2S+, minority, Christian religious). The number of nodes selected was restricted to 10, keeping the table easy to interpret while also highlighting the top terms and hashtags that have a stronger correlation. To ensure that smaller deviations are not overshadowed by the larger deviations, and to make the comparison between the contingency matrix blocks easier, the log scale was added during the analysis stage on Cortext. Further, the parameters of the script were set such that the statistically insignificant blocks have been crossed out (i.e. where the p-value is larger than 0.05 and the correlation is not significant, a cross marks the cell block). 

Some interesting correlations can be seen in the matrix, which also reflect and support the above analysis. There are several dark red blocks indicating a high correlation between some terms and hashtags, such as "pregnancy centres" and #cantstaysilent, which makes sense since both are likely to be mentioned by pro-life organisations encouraging women to consider not having abortions. Some of the correlations might be expected and may even seem intuitive. For instance, tweets mentioning the terms "supreme court" also mention #scotus and #roevwade more frequently. One interesting finding is that the hashtag #prolife does not have a statistically significant correlation with either of the top 10 terms listed in the matrix. On the other hand, the term "abortion rights" has a significant positive correlation only with the hashtag #abortionisessential. Broadly speaking, the matrix shows a general pattern that there are specific terms and hashtags that tend to appear together very frequently, however they do so in a smaller number of tweets within our corpus. This also shows that users who frame the issue from a particular angle tend to use terminologies and hashtags that are very specific to their perspective. For instance, tweets that use the terms "reproductive freedom" tend to also include hashtags that only refer to freedom (e.g. #reprofreedomvoter and #fightbackforfreedom).   



## Conclusion

Our analysis aimed to shed light on the way that different groups in the US discussed and framed the 'abortion issue.' We analysed the language used in tweets by many pro-choice, pro-life, minority, LGBTQ2S+ and Christian religious organisations between May 1st and November 16th, 2022. Broadly, our empirical findings were consistent with our hypotheses:
- Our finding that the pro-choice and pro-life groups use different terms and hashtags to frame the abortion debate, with the exception of neutral terms like "Roe v. Wade" and "Supreme Court," are consistent with hypothesis H1. 
- Furthermore, in line with H2, we indeed found that LGBTQ2S+ and minority groups use similar terms in their tweets as the pro-choice groups use, whereas the Christian religious group uses words common in both the pro-choice and the pro-life groups. 
- The non-abortion-focused groups (LGBTQS2+, minority and Christian religious) included their own-issue-specific terms and hashtags in their tweets on abortion, as expected in H3. 
- Finally, our temporal analysis showed that non-abortion-focused groups mostly tweet about abortion on the day of the leaked Supreme Court opinion draft and on the day of the _Dobbs_ decision that overturned _Roe_, but very little otherwise, consistent with H4. It also gave rise to the interesting finding that non-abortion-focused groups did not tweet much about the abortion debate during the November 2022 midterm elections, in contrast to the pro-life and pro-choice groups.

The network analysis and contingency analysis helped to bring out further nuances to the ones we had found in our top terms, hashtags and tweets analysis. The network map showed graphically the affinity of LGBTQ2S+ groups with pro-choice groups, as well as the former’s interest in the Women Health Protection Act. It also illustrated that natural terms such as "dobbs decision" are the only link between the otherwise polarised language of pro-choice and pro-life stances. The contingency matrix showed that there are specific terms and hashtags that tend to appear together very frequently, however they do so in a smaller number of tweets within our corpus. It also showed that users who frame the issue from a particular angle tend to use terminologies and hashtags that are very specific to their perspective.


