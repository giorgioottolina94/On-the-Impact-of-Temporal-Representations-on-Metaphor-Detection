# On the Impact of Temporal Representations on Metaphor Detection [LREC 2022]

Our explorative analysis highlighted interesting recurring patterns, such as the interactions between literal meanings and domains of discourse (for example, in sentences containing correctly identified metaphors, the topics related to economics, politics, and emotions are the most recurring ones); verbs with a literal meaning characterized by physical connotations, often getting figurative meanings when used in sentences related to the aforementioned contexts (economics, politics, emotions, etc).

Some patterns concern indeed the interaction between time and language. Studying the predictions obtained with the embeddings of one specific time period, we noticed that none of the sentences belonging to the "news" domain of the VUA dataset were correctly predicted. This could indicate that for that specific time period (1990 decade), words' representations of that domain are biased towards their metaphorical meaning, and this would prevent the neural networks from correctly identifying the metaphors.
Furthermore, if temporal word embeddings provided words' representations that are more inclined towards their literal core meaning (and not the metaphorical one), models exploiting them would correctly identify metaphors more easily.
One way to investigate these hypotheses further is to explore the nearest neighbors of a word in the word embeddings used in a figurative way inside a sentence, both in a static (atemporal) word embedding space, e.g., obtained with GloVe, and in a decade-specific temporal space, e.g., obtained from the CoHa corpus with Procrustes alignment.
