Update README.md

# Abstract 
 
 
# Introduction

Elucidating the prefrontal cortical microcircuit has been challenging, given its role in multiple complex behaviors, including working memory, cognitive flexibility, attention, social interaction and emotional regulation. Additionally, previous methodological limitations made it difficult to parse out the contribution of certain neuronal subpopulations in refining cortical representations. However, growing evidence supports a fundamental role of fast-spiking parvalbumin (PV) GABAergic interneurons in regulating pyramidal neuron activity to drive appropriate behavioral responses. Further, their function is heavily diminished in the prefrontal cortex (PFC) in numerous psychiatric diseases, including schizophrenia and autism. Previous research has demonstrated the importance of the optimal balance of excitation and inhibition (E/I) in cortical circuits in maintaining the efficiency of cortical information processing. Although we are still unraveling the mechanisms of information representation in the PFC, the E/I balance seems to be crucial, as pharmacological, chemogenetic and optogenetic approaches for disrupting E/I balance induce impairments in a range of PFC-dependent behaviors. To address these questions, here we analyze the continuity and form of population plasticity in the PFC of rats learning rules on a Y-maze. 

 
# Materials and Methods

### GABAergic signaling

### E/I Balance


### Task and electrophysiological recordings. 
Four Long–Evans male rats with implanted tetrodes in prelimbic cortex were trained on a Y-maze task (see Fig. 1A). Each recording session consisted of a 20 –30 min sleep or rest epoch (pretraining epoch), in which the rat remained undisturbed in a padded flowerpot placed on the central platform of the maze, followed by a training epoch, in which the rat performed for 20 – 40 min, and then by a second 20 –30 min sleep or rest epoch (post-training epoch). Figure 1B shows the structure of these three epochs in the 10 identified learning sessions. Every trial in the training epoch started when the rat left the beginning of the departure arm and finished when the rat reached the end of one of the choice arms. Correct choice was rewarded with drops of flavored milk. Each rat had to learn the current rule by trial-and-error: go to the right arm, go to the cued arm, go to the left arm, or go to the uncued arm. To maintain consistent context across all sessions, the extra-maze light cues were lit in a pseudo-random sequence across trials, whether they were relevant to the rule or not.
The data analyzed here were from a total set of 50 experimental ses- sions taken from the study of Peyrache et al. (2009), representing training sessions starting from naive until either the final training session, or until choice became habitual across multiple consecutive sessions (consistent selection of one arm that was not the correct arm). The 4 rats, respec- tively, had 13, 13, 10, and 14 sessions. From these, we have used here 10 learning sessions and up to 17 “stable” sessions (see below). Tetrode recordings were spike-sorted only within each recording ses- sion for conservative identification of stable single units. In the sessions we analyze here, the populations ranged in size from 15 to 55 units. Spikes were recorded with a resolution of 0.1 ms. For full details on training, spike-sorting, sleep identification, and histology see Peyrache et al. (2009).

### Session selection and strategy analysis. 
We primarily analyze here data from the 10 learning sessions in which the previously defined learning criteria (Peyrache et al., 2009) were met: the first trial of a block of at least three consecutively rewarded trials after which the performance until the end of the session was 􏰀80%. In later sessions, the rats reached the criterion for changing the rule: 10 consecutive correct trials or one error in 12 trials. By these criteria, each rat learned at least two rules.
We also sought sessions in which the rats made stable choices of strat- egy. For each session, we computed P(rule) as the proportion of trials in which the rat’s choice of arm corresponded to each of the three rules (left, right, cued-arm). Whereas P(left) and P(right) are mutually exclusive, P(cued-arm) is not, and has an expected value of 0.5 when it is not being explicitly chosen because of the random switching of the light cue. A session was deemed to be “stable” if P(rule) was greater than some thresh- old 􏰍 for one of the rules, and the session contained at least 10 trials (this removed only two sessions from consideration). Here we tested both 􏰍 􏰁 0.9 and 􏰍 􏰁 0.85, giving 13 and 17 sessions, respectively. These also, respectively, included 2 and 4 of the rule-change sessions. For the time- series in Figure 1C, E, F, we estimated P(rule) in windows of 7 trials, starting from the first trial, and sliding by one trial.

### Characterizing population activity as a dictionary. 
For a population of size N, we characterized the instantaneous population activity from time t to t 􏰂 􏰎 as an N-length binary vector or word. The ith element of the vector was a 1 if at least one spike was fired by the ith neuron in that time bin, and 0 otherwise. Throughout, we test bin sizes covering two orders of magnitude, with 􏰎 ranging from 1 to 100 ms. For a given bin size, the set of unique words that occurred in an epoch defined the dictionary of that epoch. The probability distribution for the dictionary was compiled by counting the frequency of each word’s occurrence in the epoch and nor- malizing by the total number of time bins in that epoch.
For each session, we constructed three dictionaries per bin size, and their corresponding probability distributions P(Epoch): pretraining sleep P(Pre), post-training sleep P(Post), and trials during training P(Trials). To unambiguously identify sleep periods, and for comparisons with pre- vious reports of replay in PFC (Euston et al., 2007; Peyrache et al., 2009), we used slow-wave sleep bouts for the pretraining and post-training sleep dictionaries.
We built dictionaries using the number of recorded neurons N, up to a maximum of 35 for computational tractability. The number of neurons used in each analysis is listed in Tables 1 and 2; where we needed to use less than the total number of recorded neurons, we ranked them accord- ing to the coefficient of variation of their firing rate between the three epochs, and choose the N least variable- in practice this sampled neurons from across the full range of firing rates. Only two learning sessions and six stable sessions were capped in this way.

### Comparing dictionaries between epochs. 
We quantified the distance D􏰃P 􏰓 Q􏰄 between two dictionarys’ probability distributions P and Q 􏰈 􏰕qi􏰄2.Toafirstapproximation,thismeasuresforeachpairofprob- abilities (pi, qi) the distance between their square-roots. In this form, DH(P 􏰓 Q) 􏰁 0 means the distributions are identical, and DH(P 􏰓 Q) 􏰁 1 means the distributions are mutually singular: all positive proba- bilities in P are 0 in Q, and vice versa.
To understand whether a pair of pretraining and post-training sleep dictionaries meaningfully differed in their structure, we compared the distance between them, D􏰃Pre 􏰓 Post􏰄, with the predicted distance if they had an identical underlying probability distribution (in which case D􏰃Pre 􏰓 Post􏰄 􏰀 0 would be solely due to finite sampling effects). We used a resampling test to estimate the predicted distance. We first created a single probability distribution P(sleep) for a session by calculating the probability of each word’s appearance in all sleep bouts across both pre- training and post-training sleep epochs. We then sampled P(sleep) to create new time-series of pretraining and post-training sleep words, matching the number of emitted words in each epoch in the original data. By then reconstructing the dictionaries in each epoch from the resampled data, we obtained a prediction for the distance D􏰃Pre􏰗 􏰓 Post􏰗􏰄, where the asterisk indicates the estimate from the resampled data. Repeating the resampling 20 times gave us a distribution of expected distances assum- ing an identical underlying probability distribution for words. The sam- pling distribution’s mean and its 99% CI are plotted for each session in Figure 3D, E: the intervals are too small to see on this scale.
We quantified the relative convergence of the training dictionary X with the dictionaries in sleep by 􏰅D􏰃Pre 􏰓 X􏰄 􏰈 D􏰃Post 􏰓 X􏰄􏰆/􏰅D􏰃Pre 􏰓 X􏰄 􏰂 D􏰃Post 􏰓 X􏰄􏰆. Convergence 􏰀 0 indicates that the distance between the training epoch 􏰅P􏰃X􏰄􏰆 and post-training sleep [P(Post)] distributions was smaller than that between the training and pretraining sleep [P(Pre)] distributions.

### Testing hypotheses for changes in dictionary structure. 
To understand what drove the observed changes in the structure of population activity, we tested three hypotheses: (1) independent changes in the excitability of neurons; (2) changes in firing rate covariations between neuron; and (3) shifts in precise co-spiking between neurons. We tested these hypotheses in two steps:
1. We tested whether dictionaries constructed from independently firing neurons could account for the observed changes in the structure of population activity, with two possible outcomes:
• Yes: Then we could conclude that changes in the data were due to independent changes to the excitability of the recorded neurons.
• No: This implied that the correlations between neurons were also changed.
2. To then identify the types of those correlations, we turned to dic- tionaries constructed from spikes jittered a little in time, and asked whether they could account for the observed changes:
• No: Then we would have evidence that precise co-spiking between neurons contributed to the changes in population activity structure.
• Yes: Then changes to population activity did not depend on precise co-spiking and could be accounted for by changes to covariations in rate between neurons.

For the independent neuron dictionaries, we shuffled interspike inter- vals for each neuron independently, and then constructed words at the same range of bin sizes. As both the training and sleep epochs were broken up into chunks (of trials and slow-wave sleep bouts, respectively), we only shuffled interspike intervals within each chunk. This procedure kept the same interspike interval distribution for each neuron but dis- rupted any correlation between neurons during a trial or during a sleep bout, thus testing for dictionary changes that could be accounted for solely by changes to independent neurons. We repeated the shuffling 20 times.
For any given data statistic sdata for a single session, we compute the same statistic sshuffle for each shuffled dataset, and plot the difference 􏰎 􏰁 Sdata 􏰈 E􏰃Sshuffle) using the mean E() over the shuffled data’s statistics. CIs at 99% for all 􏰎 were smaller than the size of the plotted symbol for 􏰎, so are omitted for clarity.
For the jittered dictionaries, each spike was jittered in time by a ran- dom amount drawn from a Gaussian of mean 0 and SD 􏰏. We tested 􏰏 from 2 to 50 ms. For each 􏰏, we constructed 20 jittered datasets. Words were constructed from each using 5 ms bins here, both as this time-scale would capture millisecond-precise spike timing between neurons and because the biggest effects in the data were most consistently seen at this bin size.
We illustrated changes in the rate covariation between neurons using the coupling between single-neuron and ongoing population activity (Okun et al., 2015). Each neuron’s firing rate was the spike density function fi obtained by convolving each spike with a Gaussian of 100 ms SD. Population coupling for the ith neuron is the Pearson’s correlation coefficient: ci􏰁 corr􏰃 fi, P􏰇i􏰄, where P􏰇i is the population rate obtained by summing all firing rate func- tions, except that belonging to the ith neuron.


# Results




















# Discussion

