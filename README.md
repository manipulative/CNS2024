# The neural architecture of interpersonal cultural conflicts

## Research Question

Every day, we communicate with various people, including our friends, family, and colleagues. Why can we understand each other so well and so quickly?

Recent studies suggest that just like language comprehension through a hierarchical process, such as syllable - word – sentence, during communication, we understand each other by forming hierarchical shared representations. For example, when we communicate, we start by understanding and aligning the basic verbal symbols we used. We then move to interpreting each other’s semantic meanings from verbal information and forming a shared sematic space, and finally, we grasp each other's deep intentions and beliefs. During the process of constructing hierarchical shared representations, neural synchronization may occur between the brains of the communicators.

![image](https://github.com/manipulative/CNS2024/assets/26652791/bef2c7c5-7d9b-4d7a-947c-17394e36f563)

With the advancement of globalization, intercultural communication has become one of the main forms of our daily interactions, like the communication we are engaged in right now. However, cultural psychologists have found that people from different cultural backgrounds exhibit differences in many cognitive processes, such as symbolic systems, semantic concepts, and values.  These cultural differences often lead to conflicts during intercultural communication and may exhibit a different hierarchical structure from our ordinary communication.

So our research question is, **what is the unique communicative hierarchical structure in interpersonal cultural conflicts?**

## Method

To do so, we recruited 31 American college students who can speak Mandarin in China. Each of them paired with a Chinese college student to have four rounds of free conversation on culturally relevant topics. All participants had little intercultural experience. Both participants in each dyad were hyperscanned using fNIRS to collect hemodynamic signals.

<img width="644" alt="image" src="https://github.com/manipulative/CNS2024/assets/26652791/55c196c3-51b9-48e9-990b-721c0b8b3a03">

## Results

### The hierarchical structure of interpersonal cultural conflict 

According to previous studies in communication and cross-cultural psychology, we hypothesized that the primary layers of intercultural conflicts occur at the layers of semantic representation and cultural values. 

To identify the hierarchical structure of intercultural conflicts, we constructed shared representation indexes for both layers across three behavioral modalities.

For the real-time modality, we first transcribed their speech in each turn into text. Then, we used the word2vec model to transform text into word embeddings. 
At the semantic layer, we quantified the level of shared semantic representation by calculating the cosine similarity of word embeddings between Chinese and American for each turn. 
At the cultural layer, we employed a method called semantic projection. Initially, we created an "individualism-collectivism" dictionary. Each dimension included five representative words such as 'cooperation', 'obedience', 'autonomy', and 'self-determination'. We used the word vectors from this dictionary to construct a cultural feature space. By computing the dot product of word vectors in each conversational turn with this cultural feature space, we could determine to what extent each statement reflected collectivist or individualist values. For example, the projection value of words like “friend” and “relative” score high on collectivism, while “debate” and “argument” score high on individualism. We then measured the level of shared cultural representation by calculating the difference in projection values for each turn between communicators.

<img width="781" alt="image" src="https://github.com/manipulative/CNS2024/assets/26652791/3d614258-4f7b-4009-8d91-7494fc15e0f5">

For the state modality, after each round of conversation, we asked both participants to rate to what extent they understood each other and the degree of cultural conflicts they experienced, 
then we calculated the average value for the two communicators.

<img width="295" alt="image" src="https://github.com/manipulative/CNS2024/assets/26652791/ddebb94b-36aa-4df1-9e1f-ccaf7c56a270">

For the trait modality, in the cultural layer, we used the self-construal scale to measure each participant’s cultural mindset and calculated their cultural mindset distance. In the semantic layer, participants were asked to rate the semantic relatedness of 20 abstract words and further calculated their semantic structure similarity.

<img width="489" alt="image" src="https://github.com/manipulative/CNS2024/assets/26652791/5197ee6a-3809-44e1-a590-714b9b842da9">

For all three indices in the two layers, the level of shared representation in the across-culture interaction group was lower than that in the within-culture interaction group. Further, we performed a PCA on six variables, resulting in two dimensions that align with our hypotheses.

<img width="495" alt="image" src="https://github.com/manipulative/CNS2024/assets/26652791/c5d13abb-1b72-4d56-9b63-eefd91a4903b">

Therefore, we can conclude that interpersonal cultural conflicts have a hierarchical structure that includes at least two levels: conflicts in cultural value representation and conflicts in semantic representation.

### The interpersonal neural synchronization(INS) basis of hierarchy

Further, we investigated the interpersonal neural synchronization (INS) basis of these two layers. We used the wavelet transform coherence algorithm to calculate the INS between participants in each dyad. This algorithm allowed us to calculate the synchronization between brain regions of two participants at each time point. 

We found that INS in the mPFC of American to the mPFC of Chinese was lower than that within the same-culture dyads. Also, the INS in the lTPJ of American to the rMTG of Chinese was lower in across-culture interaction either. This decreased neural synchronization under conditions of cultural conflict was consistent across both English and Mandarin settings.

<img width="793" alt="image" src="https://github.com/manipulative/CNS2024/assets/26652791/62ed80e9-79de-4b15-8f8d-fcaf4cf3c9a1">

Then, we developed a method called interpersonal-RSA to examine the correspondence between INS and two communication layers. At the behavioral level, we used the real-time modality's turn-by-turn semantic RDM and cultural RDM. At the neural synchronization level, we calculated the INS differences for each conversational turn, creating a turn-by-turn neural synchronization RDM. We then calculated the Spearman correlation between the two behavioral RDMs and the neural RDM. 

We found that INS in mPFC to mPFC is associated with the cultural layer’s real-time RDM, and INS in lTPJ to rMTG is associated with the semantic layer.

<img width="765" alt="image" src="https://github.com/manipulative/CNS2024/assets/26652791/cd5bc37c-4938-4a22-b0c1-e7cd13986baa">

### Information pathway of hierarchy

Finally, we were interested in the relationship between these two layers, which means the information pathway between them. We conducted a Granger causality analysis on the INS time-series of two layers. 

The results indicated that conflicts at the semantic layer accumulate to the cultural layer from a bottom-up pathway.

<img width="441" alt="image" src="https://github.com/manipulative/CNS2024/assets/26652791/c1ef3333-31f8-4337-8e27-6533676c6fc8">

## Conclusion
In summary, we discovered that interpersonal cultural conflicts possess a hierarchical structure comprising at least two layers: conflicts in cultural value representation and semantic representation. 

Such hierarchical structure reflected in decreased interpersonal neural synchronization in mPFC to mPFC and lTPJ to rMTG. 

The hierarchy is characterized by lower-level semantic conflicts accumulating to higher-level cultural conflicts.



