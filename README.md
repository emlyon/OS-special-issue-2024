# OS-special-issue-2024
# Supplementary Material

This appendix details different tools we used to explore sources of digital big data (social media and judicial data) with various computer sciences tools (topic modeling, sentiment analyses, network analysis, and ChatGPT’s tools for summarization of complex data). We provide some backgrounds about these tools and show how we attempted to articulate—in an interdisciplinary way—the work of the computer scientist in our team attempted in conjunction with qualitative assessment and analysis. 

## Hybridizing Topic Modeling with Hand Coding for Theoretical Elaboration
We used topic modeling to make sense of the Twitter data collected on various LGBT organizations. Our goal was to understand phenomena of collaboration and specialization in the broader LGBT movement, beyond the SMOs that we already knew well through previous research. Topic modelling, which is based on Large Language Models (LLM)—we used BERTopic here—, allows researchers to identify automatically which subjects are discussed within a corpus of documents (Egger & Yu, 2022; Grootendorst, 2022). Identifying themes through topic modeling was helpful to capture these SMOs’ repertoires of actions and claims, and to see how they were distributed among the different SMOs under study. The computer scientist in the team helped us come up with a list of 69 topics that emerged from the collected tweets. This list of topics was not labelled but was associated with (1) the topic size (how many tweets were related to this topic); (2) a list of the most frequent terms used in this topic; (3) a shortlist of the most representative tweets associated with this topic; and (4) a diagram showing which organization tweeted the most about this topic in our dataset. To provide one example of this initial material, Figure 1 shows how one of these topics was presented, and how it gave information about how different SMOs contributed to this topic (To respect the anonymity of our past fieldwork, we gave pseudonyms to the SMOs that were central to our previous analyses. Yet social media data are difficult to anonymize, and this was one area of debate between the computer scientist and the qualitative researchers in our team.)

<p align="center">
<img width="400" alt="image" src="https://github.com/emlyon/OS-special-issue-2024/assets/16318654/0a8f002d-2b35-47fd-9c24-26c513328e79">

__Figure 1:__ Topic 30, relabeled “political commentaries on legal changes around LGBT rights around the world” and its mobilization by 5 key SMOs.
</p>

With this presentation, the authors could interpret the meaning of each topic by qualitatively analyzing its most frequent terms and most representative tweets. In this example, the topic revolved around political commentaries on legal changes around LGBT rights around the world. When we analyzed the content of the tweets, we saw how they reviewed both changes in favor and against LGBT minorities in various countries. This topic and other similar ones showed us how some French LGBT SMOs engaged in global advocacy campaigns beyond working to promote workplace equality in France. The diagram also showed us that this effort of global advocacy was mostly taken on by two SMOs, and not really mobilized by others. Qualitative researchers recoded this this initial raw classification produced by the computer scientist to interpret and label each topic to capture what their common core was, and to see how they related to one another.  
This recoding of topics was helpful to expand our understanding of the LGBT movement beyond the categories that researchers were used to look for, and to re-expand their understanding of the movement by examining what were the emerging themes through topic modeling. As the organizations whose tweets were analyzed were SMO engaged in lobbying and advocacy efforts, what emerged was not just a list of themes, but a list of claims and strategies from these different SMOs, as well as a list of potential targets that they aimed at in their tweets. Thus, while these topics helped capture some topics that became central in the claim of this LGBT rights movement (biphobia, transphobia, AIDS awareness), they also favored the elaboration of a list of tactics (targeting the government for advocacy, collecting data to prove LGBT discrimination, organizing local events, etc.), and pinpointed how these tweets could target different types of actors (private companies, local officials, volunteers, governmental actors, the LGBT community itself, etc.). This recoding thus helped us develop a comprehensive understanding of the tactical repertoire of the different SMOs engaged in the field of LGBT rights activism in France through online activism. Some topics from this initial list appeared to be redundant, and the qualitative coder noted when different topics identified through topic modeling seemed to be related to the same underlying idea (e.g., several topics were related to call for volunteers, sharing of LGBT-relevant news with their communities of followers, or the organizing of some specific awareness campaigns). Thus, it seems helpful to bring together topics that were initially perceived as different, and to create an arborescence of these different topics to see how we could cluster them into similar types of topics. 
Therefore, we decided to see how our initial list of 69 topics were related to one another and could be rearticulated with others. We contrasted two tools for doing so. One of the authors created an automated hierarchical clustering. The LLM used for topic modelling (the BERT encoder) represents words, phrases, and tweets as vectors in a higher-dimensional vector space, and the semantic properties of these representations are such that texts with similar meanings have representations which are close in vector space. Vector representations of topics can thus be compared two by two to build a dendrogram of similarities as displayed in Figure 2 (for instance in the top left corner topics 22, 41, and 47 are highly similar). 

<p align="center">
<img width="412" alt="image" src="https://github.com/emlyon/OS-special-issue-2024/assets/16318654/04af2ae0-ccbf-447e-93cf-846fd3fddfe2">

__Figure 2:__ Dendrogram: hierarchical clustering of topics similarities (based on embeddings)
</p>


In parallel, qualitative researchers organized these codes in an arborescence through theoretical elaboration, engaging in coding as they usually do when trying to relate different pieces of initial codes by articulating them in axial codes in qualitative research (Charmaz, 2013). While some elements were similar in the manual coding and the hierarchical clustering (e.g., the list of topics that were found to be redundant by the qualitative researcher were indeed considered a cluster in the automated hierarchical clustering), some more theoretical rearticulation did not appear in the hierarchical clustering produced automatically. 
These thematic clusters were helpful to see how different SMOs positioned themselves with regards to broad strategies (cf. Figure 3).  

### Fig 3


Figure 3 shows how the five SMOs on which we tested these models relate to two clusters of topics identified by qualitative researchers (identified as “global movements for LGBT rights” and “tools to denounce and demonstrate discrimination”). These diagrams were helpful to objectify tendencies that we could observe qualitatively and to support them with statistically relevant measures. Ultimately, they might be helpful to capture tendencies when studying lesser known SMOs in the LGBT movement. 
The use of topic modelling also allowed us to track the longitudinal evolution of topics in the 2015-2023 period. We grouped tweets by quarters and semesters and conducted two distinct analyses to observe how topics identified across the entire corpus of tweets changed over time. First, we identified which tweets of a given quarter or semester belonged to which global topic and counted tweets and topics per quarter or semester to derive a longitudinal trend for each global topic. Second, we ran an independent topic modeling analysis on the tweets of each quarter or semester to find local topics. We then computed their similarities with the global topics, deriving another temporal trend from the general topics (similarities were computed using the vector representation of topics as mentioned above). Figure 4 displays these time evolutions and shows how clusters of topics evolved in terms of number of tweets. Once we saw these saliences of some topics through time, we qualitatively went back to analyze what these salient points were about through analysis of representative tweets. This shows why we need to design an interactive process between using computer sciences models and going back to qualitative data to make sense of them. This research entailed a constant back and forth between modeling through different tools of topic modeling, and qualitative interpretation of the salience of some topics. 

### Fig 4

This automated method for topic modeling had interesting facets for qualitative researchers. First, these tools provided statistical evidence of how the topics were unequally discussed by different SMOs. It helped us ground an intuition coming from hand coding of the data and generalize it with more statistically relevant figures to show how some topics really were primarily tackled by some SMOs and not others. But beyond this generalization concern, the automated method also brought to the attention of qualitative researchers emerging themes that were significant in volume, but to which the researchers did not pay much attention when coding by hand. Similarly, topic evolutions through time compelled us to go back to qualitative data with more specific questions in mind (Why did this topic resurfaced so powerfully at a specific time? What was the stake then?). This shows how combining topic modeling with qualitative coding could be beneficial to develop large-scale analysis of a social movement field on social media. While we focused on the data from Twitter (now X) to examine the movement for workplace LGBT rights in France, we believe that the tools explored here could be helpful to study different social movements, advocacy, and lobbying efforts online, and that similar tools could work for other social media platforms (Facebook, LinkedIn, Instagram, etc.). Advocacy work and influence work on social media is a complex phenomenon, which occurs through various stages through time, and also tends to be scattered across different organizations. Thus, to gain a comprehensive understanding of how such movements develop through time, progressively renew their claims, articulate various tactics (disruptive, persuasive, reputation-mediated, educational, etc.), and engage in strategic division of labor, it seems necessary to combine tools for big data (web scrapping tools, topic modelling, network analysis), with a fine-grained analysis of these processes through a qualitative perspective.

## Sentiment analysis
Sentiment analysis is interesting to study the tone used by organizations to communicate on various topics, and hence how they stand rationally or emotionally. We attempted to study polarity and subjectivity of tweets and topics of different SMOs. Polarity is measured by an index measuring sentiment and ranging from -1 to 1 (-1 very negative, 0 neutral, 1 very positive), and subjectivity with an index ranging from 0 to 1 (0 objective, 1 subjective). Sentiment analysis could give us a big picture of the tone used by different SMOs. For instance, Figure 5 shows that @Hospital_internal has noticeable strong negative tweets, with polarity -1 and subjectivity 1, one of which is for instance: messages such as “When school becomes hell: the terrible daily life of Thomas, victim of school bullying.” Similarly, Figure 6 shows how, in the cluster of topics around awareness campaigns, some awareness campaigns used neutral or positive discourses, while others used strongly negative discourses (e.g., AIDs awareness campaigns, anti-hate campaigns). Going back to the most representative tweets here was helpful to capture why some topics or SMOs were associated with particularly negative or positive types of discourses. 

### Fig 5
### Fig 6

The qualitative researchers could both check how this sentiment analysis related to our own knowledge of the given organizations, but also recode inductively representative tweets to draw more general conclusion about which organization developed which kind of discourses. As our goal is to expand this tool to lesser-known LGBT organization, it will help us capture phenomena beyond the pool of the most studied and central LGBT organization in France. 

## Network analysis
We also explored how we could conduct network analysis of the different SMOs under study. Figure 7 displays interactions between our five tested SMOs, as seen on Twitter through retweets and citations (network of retweets to the left, and citations to the right). This helped objectify the connections between some organizations: both in terms of retweets and citations, @Hospital_internal related to @Police_internal and @Watchdog_external, but this connection was unilateral. In terms of retweets, @Ally_external retweeted others a lot. In terms of citations, all SMOs mentioned @Watchdog_external a lot. These variation in density of connections are here easy to interpret for the organizations that researchers already knew well, but they give us a tool to objectify these interrelations. In addition, if we include more SMOs in these network analyses, we should be able to gain an understanding of the broader LGBT field. To interpret the other connections, we will need to go back to qualitative interpretation to see how different SMOs cite and retweet one another. 

### Fig 7

With this retrospective account of our tinkering with topic modeling for analyzing the LGBT rights movement in France, we have shown how these tools could be helpful to capture SMOs various claims, tactics, targets, and tone. In addition, we showed how such tools could be helpful to capture how strategies vary through time and how SMOs specialized in some tactics or claims, thereby engaging in a strategic division of labor (authors, date). We have examined here for instance the emergence of specific campaigns at different points in time, and their variation in terms of tone. While showcasing these tools, we also identified key moments in the analysis of data where the qualitative interpretation of the data was necessary to make sense of the output of topic modeling, sentiment or networks analyses. 


## Assessing qualitatively Chat GPT’s summaries and chronologies of judicial cases
A last tool we wish to present here is the use of ChatGPT to summarize complex data (here judicial cases). We are using these summaries as a tool to help us select relevant cases to explore, and we also discuss the necessity to design ways to assess the quality of these summaries. We used the following prompt on the version of ChatGPT 3.5 “Can you provide a summary and a chronology of the key events for the following judicial decision” and then we pasted the full content of the decision being examined (in French). We took a judicial decision that was 5-page long (2022 words). The outcome—written in less than a minute—was the following response (391 words):

>This judicial decision, rendered by the Cour de cassation (French Supreme Court) in its social chamber on May 6, 2015, concerns a case involving a contractual dispute between an employer (M. Y...) and an employee (Mme X...). Here is a summary and chronology of the key events:
>
>Background: Mme X... was employed as a waitress by M. Y..., who operated a restaurant. She was hired on a fixed-term contract from June 14 to July 14, 2010, and then from July 15, 2010, to January 14, 2011.
>
>Legal Action: Claiming that her employer committed a serious fault justifying the early termination of her employment contract, Mme X... brought the matter to the prud'homal jurisdiction (labour court).
>
>First Instance Decision: The labour court ruled in favor of Mme X... by finding that the employer's actions constituted a serious fault.
>
>Appeal: M. Y... appealed the decision to the Cour d'appel de Caen (Court of Appeal of Caen).
>
>Decision of the Court of Appeal (July 5, 2013): The Court of Appeal upheld the finding of a serious fault on the part of the employer. It ordered M. Y... to pay Mme X... certain sums as back pay and related vacation pay, as well as to provide her with compliant pay slips.
>
>Appeal to the Cour de cassation: Dissatisfied with the decision, M. Y... appealed to the Cour de cassation.
>
>Cour de cassation's Decision (May 6, 2015):
>
>First Ground: The Cour de cassation rejected the first ground of appeal, finding that the Court of Appeal had appropriately assessed the evidence and correctly determined the existence of a serious fault on the part of the employer.
>
>Second Ground: The Cour de cassation partially accepted the second ground of appeal. It ruled that the amounts awarded to Mme X... by the Court of Appeal did not qualify as salary and therefore should not have led to the issuance of compliant pay slips. The case was therefore partially annulled on this point and referred back to the Court of Appeal of Rouen for reconsideration.
>
>In summary, the Cour de cassation upheld the finding of a serious fault by the employer but partially annulled the Court of Appeal's decision regarding the payment of certain sums and the issuance of compliant pay slips. The case was remanded to the Court of Appeal of Rouen for further consideration on these specific points.

This summary, which is short and written in plain English, was easy to understand and helped us quickly grasp what this case was about. A serious fault of an employer against one of his employees: a waitress. We know the gender of the two key actors in this case, and have a basic timeline of the events. To check for the accuracy of these description, we contrasted it with the full case in French. The events described in ChatGPT’s summaries are accurate. Yet, it did not provide enough background about the nature of what was reproached to the employer. For the sake of demonstration, we produce a table below that contrast ChatGPT’s summaries (in plain, clear English) with the relevant excerpts of text (in French, with complex judicial language and frequent repetition). We only present a few rows to show how we are proceeding. Table 1 below provides an analysis of which actual text correspond to pieces of summary from ChatGPT: 

### Table 1

As discussed in the last column of the table above, some informatiuon were missing about  specificities of this case (What was the serious fault of the employer? What happened concretely?). We therefore further prompted: “what is reproached exactly to the employer?” To this question, the response was: 
*The employer (M. Y...) was reproached for failing to adequately address and respond to a serious allegation of sexual assault made by the employee (Mme X...) against a client of the establishment. Despite being informed of the incident by the employee, the employer allegedly reacted inadequately by dismissing the complaint and instructing the employee to return to work, without taking appropriate measures to ensure her safety or address the reported incident seriously. The Cour de cassation found that this failure by the employer to respond appropriately to the employee's complaint constituted a serious fault, which ultimately justified the employee's early termination of the employment contract. This failure was considered a breach of the employer's obligation to ensure the health and safety of employees in the workplace.*

This summary correspond to what we could understand from reading the case, and gives us a better picture of the stakes in this judicial case: here, the employer failed to protect her employee who was sexually assaulted by a client. With this, we have enough information to classify this case and help us see what this is a case of, and to decide how to include this case in our own analysis. 
Here is a second example, where we used the same initial prompt to summarize and build a chronology of a seven-page long case (2347 words). The output of ChatGPT read as follows: 
*Here's a summary and chronology of the key events in the judicial decision dated March 25, 2020 (Cour de cassation, civile, Chambre sociale, 25 mars 2020, 18-23.682):*
*Summary: The case involves a dispute between Mr. J... R... (the employer) and Ms. P... V... (the employee). Ms. V... was employed by Mr. R... as a dental assistant under a professional training contract. She was summoned for a preliminary interview regarding her termination on October 7, 2013, and was subsequently terminated for serious misconduct on October 25, 2013. Ms. V... alleged that she was a victim of sexual harassment and filed a claim against her dismissal on October 12, 2015. The trial court found the employer not guilty of sexual harassment on July 28, 2016. However, the appellate court concluded that Ms. V... was indeed subjected to sexual harassment and declared her dismissal null and void.*
*Chronology:*
*July 2, 2012: Ms. V... was hired by Mr. R... as a dental assistant under a professional training contract.*
*October 7, 2013: Ms. V... was called for a preliminary interview regarding her termination.*
*October 12, 2013: Ms. V... was terminated for serious misconduct.*
*October 12, 2015: Ms. V... filed a claim against her dismissal, alleging sexual harassment.*
*July 28, 2016: The trial court found Mr. R... not guilty of sexual harassment.*
*September 6, 2018: The appellate court reversed the trial court's decision, declaring Ms. V...'s dismissal null and void due to sexual harassment.*
*March 25, 2020: The Cour de cassation upheld the appellate court's decision, rejecting Mr. R...'s appeal.*
*In summary, the employee, Ms. V..., alleged sexual harassment by her employer, Mr. R..., which led to her termination. The trial court initially found Mr. R... not guilty of sexual harassment, but the appellate court overturned this decision and declared Ms. V...'s dismissal null and void. The Cour de cassation ultimately upheld the appellate court's decision, rejecting Mr. R...'s appeal.*

Here again, this summary gives us a general understanding of the case. Further analyses then require to read fragments of the text for line by line coding if the researchers judged that they are interested in studying cases where someone is fired and contest this decision by mentionning a cause of sexual harassment. 

## Assessing the accuracy of Chat GPT on deductive coding
While this tool felt tremendously helpful to facilitate case selection without having to write summaries and chronologies for each case by hand, the question of the accuracy of these summaries soon emerged. To address this, the computer scientist and co-author of this paper helped us design a protocol to check Chat GPT’s performance on deductive coding. ChatGPT’s results do not come with estimations of their accuracies, or statistical estimates of the performance of its model. These can however be obtained by researchers who need to estimate VhatGPT’s performance on the dataset under study (here documents in the corpus of the 445 legal cases) as well as on similar data. For classical tasks such as labelling and classifying documents (finding categorical outputs to a document) or regression tasks (finding continuous numerical outputs) a simple protocol is as follows: 1) extract a random subset of samples (documents) 2) perform manually the labelling or calculation of continuous outputs 3) compare with chat GPT’s output on these samples. This last comparison is performed just like in standard supervised machine learning when computing an in-sample error to estimate the out-sample error and assess the performance of a model. The evaluation metric will depend on the task and what researchers need to measure. For labelling documents for instance, a classification task, researchers will decide which classification metric to use (e.g., accuracy, precision/recall, F1, AUCs, etc.). For extracting relevant parts of a document, a weighted average of ratios of intersections (or Jaquart index) between what researchers vs ChatGPT identified would work. 
For deductive coding taks, the protocol is the same: 1) extract a random subset of samples (documents); 2) perform the deductive coding on the samples (to get their true deductive codings); 3) compare with chat GPT’s output on these samples. But the comparison step is adapted to deductive coding (assigning labels to words in the documents of the samples). Scores per documents may be computed by checking the proportion of correct chatGPT produced codes vs true codes (weighted by the proportion of common terms associated with a code), or any other classification metric for that matter. Then the evaluation metric is the average of scores over the samples.
As this project progresses, we are attempting to make more systematic assessment of the accuracy of ChatGPT’s output, while also working on our research design to see how such summaries of text could help us classify these judicial cases, facilitate theoretical sampling through helping us identify scenarios and help choices for further qualitative coding, and test out models of deductive coding to code key variables about each of these cases (e.g., gender of the victim, outcome of the trial, hierarchical relationship, etc.). 
![image](https://github.com/emlyon/OS-special-issue-2024/assets/16318654/72caee19-aac0-47ff-ad75-61f101597662)

