Update README.md
# Does coupling information give insight to how E/I balance is maintained?

## Abstract 
 
 
## Introduction

The prefrontal cortical circuit plays host to a multitude of brain functions and complex behaviors such as controlling attention, social interaction and emotional regulation. A general understanding is that it learns a model for the statistics of actions and their expected outcomes to guide or monitor behavior. Previous work has shown that inactivating mPFC impairs the learning of new rules (Ragozzino et al., 1999a,b; Rich and Shapiro, 2007; Floresco et al., 2008), and single pyramidal neurons change their firing times relative to ongoing theta-band oscillations only with successful rule learning (Benchenane et al., 2010).  Additionally, previous methodological limitations made it difficult to parse out the contribution of certain neuronal subpopulations in refining cortical representations. Previous research has demonstrated the importance of the optimal balance of excitation and inhibition (E/I) in cortical circuits in maintaining the efficiency of cortical information processing. Although we are still unraveling the mechanisms of information representation in the PFC, the E/I balance seems to be crucial, as pharmacological, chemogenetic and optogenetic approaches for disrupting E/I balance induce impairments in a range of PFC-dependent behaviors. 
We know little about how this pyramidal neuron activity is regulated to drive appropriate behavioral responses. The 
To address these questions, here we analyze the continuity and form of population plasticity in the PFC of rats learning rules on a Y-maze. 

 
## Materials and Methods

### Description of neurons in PFC
Within the cortex, there are two primary types of neurons: glutamatergic excitatory pyramidal neurons and GABAergic inhibitory interneurons. While a network of purely excitatory connections offers little computational complexity, GABAergic interneurons confer a circuit with tremendous flexibility, dynamically modulating the gain of pyramidal neuron responses from simple all-or-none responsiveness (Klausberger et al., 2003; Isaacson and Scanziani, 2011). Through inhibition of neighboring pyramidal neurons, GABAergic interneurons act as an important brake on excitatory signaling, control spike generation and timing (Pouille and Scanziani, 2001), and prevent incoming excitation from afferent structures from causing runaway feed-forward excitation (Dichter and Ayala, 1987).
GABAergic interneurons are a diverse family that can be classified by their morphology, electrophysiological properties, or histological markers (Markram et al., 2004, 2015). The most common nomenclature segregates interneurons into three broad types, parvalbumin (PV), somatostatin (SST) and ionotropic serotonin receptor 5HT3a (5HT3aR) expressing interneurons (Rudy et al., 2011). Although not entirely distinct, this population minimizes overlap between the groups and accounts for nearly the entirety of known interneuronal subtypes.
The most common subtype, PV interneurons, are known for their fast-spiking phenotype, low input resistance, and high-amplitude rapid after-hyperpolarization (AHP; Kawaguchi et al., 1987; Kawaguchi and Kubota, 1997). This combination of properties confers an ability to fire a rapid train of action potentials unlike any other neuron in the cortex. PV interneurons can be further divided into two subtypes: basket cells that innervate the soma and proximal dendrites, and chandelier cells that synapse onto the axon initial segment (Kawaguchi and Kubota, 1997; Petilla Interneuron Nomenclature Group et al., 2008). Relatively less is known about the properties and function of chandelier cells, and data demonstrate their action may not be purely inhibitory at the axon initial segment (Szabadics et al., 2006). PV basket cells are more common, and by virtue of being easier to identify and study, their properties and role in circuit integration in the normal brain have been characterized in greater detail. Data from paired recordings indicate that a single PV interneuron contacts nearly every local pyramidal neuron providing PV basket cells with an unparalleled ability to regulate the activity of nearby pyramidal neurons (Packer and Yuste, 2011). This allows for a tremendous level of feedforward and feedback inhibition that serves several important functions (Hu et al., 2014). 
An ability of PV interneurons that appears to be universal across cortical regions is controlling spike timing in neighboring excitatory neurons (Pouille and Scanziani, 2001; Wehr and Zador, 2003). Pyramidal neurons receive constant barrages of excitatory synaptic input or excitatory post-synaptic potentials (EPSPs), and are tasked with deciding whether or not to fire an action potential. Given the density of excitatory connections both from afferent structures and within the local circuit, along with the high level of synaptic divergence, excitation of a sufficient magnitude to generate an action potential will likely recruit a large portion of the cortical network, making it challenging to represent information with any specificity. This creates two computational dilemmas, creating a network state such that all excitatory neurons are not firing constantly, as well as allowing for distinct neurons or groups of neurons to have differential responsiveness to EPSPs. One issue is addressed by feedforward inhibition (FFI), a principle illustrated canonically in thalamocortical circuits. A major source of excitatory cortical input is the thalamus, whose neurons branch and synapse onto both excitatory and inhibitory neurons. Seminal physiological studies demonstrated that when thalamic fibers are electrically stimulated, this causes a direct excitatory response in cortical pyramidal neurons, followed shortly by a strong hyperpolarization due to the activation of neighboring PV basket cells (Agmon and Connors, 1991; Castro-Alamancos and Connors, 1997). This enhances the temporal fidelity of pyramidal neuron responsiveness by limiting the window in which incoming excitation can generate an action potential, and has also been observed in the mPFC (Cruikshank et al., 2012; Delevich et al., 2015). The second issue is mitigated through another property of PV interneuron activity, gain control, or ‘‘the rate at which the firing of a neuron increases in response to increasing excitatory input’’ (Isaacson and Scanziani, 2011). This transforms pyramidal neuron responsiveness from a simple go or no-go pattern of activity to having the capacity to represent a broad range of input levels in their firing patterns, a feature that is likely to be crucial in the mPFC, which processes complex multimodal information.
By innervating pyramidal neurons at the soma, PV basket cells are strategically positioned to exert both FFI and gain control. Additionally, PV basket cells have been implicated in the generation of gamma oscillations (30–80 Hz, Buzsáki and Draguhn, 2004), an oscillation range linked to cognition and information processing across species (Howard et al., 2003; Gaetz et al., 2011; Lundqvist et al., 2016). PV basket cells have the ability to fire at frequencies corresponding to gamma oscillations (Gulyás et al., 2010). These interneurons also synapse primarily onto alpha1-gamma-Aminobutyric acid receptors (α1-GABAARs) that are present at high levels on the soma (Fritschy and Mohler, 1995; Nusser et al., 1996), and have a decay constant corresponding to the rising phase of gamma waves (Gonzalez-Burgos and Lewis, 2008). Demonstrating a definitive link, a pair of studies utilized a battery of optogenetic tools to silence or activate cortical PV interneurons, and found them necessary and sufficient in the generation and maintenance of gamma oscillations (Cardin et al., 2009; Sohal et al., 2009). Increasing their activity not only amplified cortical gamma oscillations, but also enhanced information processing by increasing the gain of incoming information and improving behaviors dependent on the manipulated brain regions. Data also indicate the presence of significant gamma alterations in diseases with cognitive impairment, such as schizophrenia and autism spectrum disorders (ASD; Rojas and Wilson, 2014; McNally and McCarley, 2016).
In order for these processes to occur efficiently, levels of inhibition and excitation must remain in the appropriate balance, which in the mPFC has been measured as approximately 20/80% (excitation/inhibition; Le Roux et al., 2008; den Boon et al., 2015). This balance is not static and requires that inhibition be responsive to fluctuations in cortical state and levels of excitatory input (Galarreta and Hestrin, 1998; Shu et al., 2003; Atallah and Scanziani, 2009; Xue et al., 2014). PV interneurons are well suited for helping maintain the proper balance, as their activity is associated with ‘‘divisive’’ rather than subtractive inhibition, which would allow PV interneurons to respond proportionally to dynamic excitation within cortical circuits (El-Boustani and Sur, 2014). Within this balance, however, there must be the capacity for change or plasticity. Data suggests that E/I balance helps facilitate the induction of long-term potentiation, which could be critical in allowing the PFC to remain flexible and adapt to new stimulus-response contingencies (Staff and Spruston, 2003; Marder and Buonomano, 2004).

### Defining E/I balance
At the single neuron level, the numbers of excitatory and inhibitory synapses on individual cortical pyramidal neurons are highly-regulated by a process that reproducibly generates a relative invariant ratio of E/I synapses across dendritic segments [15].
Similarly, at the level of large scale cortical circuits, the ratio of excitatory to inhibitory cortical neurons is precisely controlled by multiple development process [16]. Thus, there appear to be homeostatic and developmental processes that maintain E-I balance at the level of single cells and cortical regions over long timescales. However, this does not exclude the possibility that the E/I ratio may vary between neurons and/or on more dynamic timescales.
From a global perspective, i.e., viewing excitation and inhibition as singular entities, if the level of excitation exceeds that of inhibition, then activity will increase, either until the ability of the circuit to generate activity is maximized, or until marginal increases in activity begin to recruit more inhibition than excitation, producing a state of “balance”. Conversely, if inhibition exceeds excitation, activity will decrease, either until the circuit is quiescent or until marginal decreases in activity cause larger drops in inhibition than excitation (also leading to overall balance). This is the simplest conceptualization of “excitation-inhibition (E-I) balance”. Of course, this is vastly oversimplified because circuit activity is not a singular (unidimensional) entity and both excitation and inhibition have dynamics on multiple timescales. However, before delving into these complications, we should note some useful aspects of the concept of E-I balance. First, the idea that activity will grow until a balanced state is achieved, does nicely describe what happens in isolated cortical circuits upon the optogenetic induction of activity. Stimulating some population of neurons causes activity to spread to other neurons and other layers until sufficient inhibition is recruited to produce balance [17, 18]. There is evidence that E-I balance in cortical layers 2/3 is important for optimal tuning of these circuits to respond to salient inputs and the generation of responses called neuronal avalanches [19].
Spontaneous UP states in brain slices and in vivo similarly begin in a small number of neurons, then spread to other neurons and layers where they recruit inhibition, producing an overall state of balance [20, 21]. Importantly, although circuits should be balanced, in a global sense, lest they succumb to runaway excitation or fall silent, transient imbalances, i.e., fluctuations in the level of activity, occur on fast timescales [22]. Furthermore, even balanced activity can be distributed across many configurations of neurons, and the particular population that is active at a given moment may be stable or change continuously over time. In particular, differences in local circuit connectivity, e.g., differential innervation of pyramidal neurons with different projection targets by GABAergic interneurons [23, 24], can thus lead to differences in levels of inhibition in different pathways, helping to shape the flow of activity through microcircuits. Thus, “E-I balance” usually refers a stable global level of activity within a particular circuit, even though individual groups of neurons may exhibit transient imbalances, and these groups of neurons can be dynamic over time.
In other words, even when a circuit is in E-I balance, the set of active neurons will likely evolve over time, giving rise to many possible configurations that all represent different forms of E-I balance. Changes in external input or short term synaptic plasticity may induce transitions between these configurations. The overall level of excitation and inhibition, as well as the detailed dynamics of excitatory and inhibitory synaptic conductances, will determine how much circuit activity changes in response to incoming input [25], and thus shape the signal-to-noise ratio as originally suggested by Rubenstein and Merzenich [1]. Fig. 1 illustrates a simple instantiation of this concept, although it goes without saying that changes in signal-to-noise ratio will depend on more than just the overall level of excitation and inhibition.
In this context, what does it mean for the E-I balance to be disturbed? This refers to a change in some form of excitation or inhibition such that the state or set of states for which E-I balance is achieved, is altered. In the simplified framework laid out above, this is often thought of as a change in the gain of either excitation or inhibition, causing a change in the overall level of activity at which balance is achieved. However, it is important to remember that excitation and inhibition are not unidimensional entities. Both excitation and inhibition originate from multiple sources and impinge onto different targets. For example, many studies have shown that various subtypes of inhibitory interneurons (e.g., PV vs. SOM expressing interneurons) differentially innervate different subtypes of pyramidal neurons (e.g., deep layer pyramidal neurons projecting callosally vs. projecting to subcortical targets) [23, 24, 26]. On the other hand, VIP-expressing inter-neurons innervate and inhibit other interneurons, such that activity in VIP+ interneurons can increase cortical excitation [27–29].
Thus, while the term “E-I balance” (or E/I ratio) suggests that excitation and inhibition are singular entities, in fact, both are multidimensional, and changes in E-I balance may comprise changes in the relative activity of different sub-types of excitatory or inhibitory neurons, rather than changes in the overall level of excitation or inhibition (Fig. 1, bottom). In summary, while we initially introduced a relatively simple concept of E-I balance, and provided evidence that this balance is maintained at both the single cell and global circuit levels, we then pointed out that E-I imbalance can occur on faster timescales, and that E-I balance is in fact highly multidimensional and complex. Having noted these complexities, let us now look at mechanisms which alter E-I balance, in order to show how the E-I balance concept can nonetheless aid in understanding how these mechanisms contribute to the pathophysiology of autism and related neuropsychiatric disorders.


### Population Coupling


### Data Description
Four Long–Evans male rats with implanted tetrodes in prelimbic cortex were trained on a Y-maze task (see Fig. 1A). Each recording session consisted of a 20 –30 min sleep or rest epoch (pretraining epoch), in which the rat remained undisturbed in a padded flowerpot placed on the central platform of the maze, followed by a training epoch, in which the rat performed for 20 – 40 min, and then by a second 20 –30 min sleep or rest epoch (post-training epoch). Figure 1B shows the structure of these three epochs in the 10 identified learning sessions. Every trial in the training epoch started when the rat left the beginning of the departure arm and finished when the rat reached the end of one of the choice arms. Correct choice was rewarded with drops of flavored milk. Each rat had to learn the current rule by trial-and-error: go to the right arm, go to the cued arm, go to the left arm, or go to the uncued arm. To maintain consistent context across all sessions, the extra-maze light cues were lit in a pseudo-random sequence across trials, whether they were relevant to the rule or not.
The data analyzed here were from a total set of 50 experimental ses- sions taken from the study of Peyrache et al. (2009), representing training sessions starting from naive until either the final training session, or until choice became habitual across multiple consecutive sessions (consistent selection of one arm that was not the correct arm). The 4 rats, respec- tively, had 13, 13, 10, and 14 sessions. From these, we have used here 10 learning sessions and up to 17 “stable” sessions (see below). Tetrode recordings were spike-sorted only within each recording ses- sion for conservative identification of stable single units. In the sessions we analyze here, the populations ranged in size from 15 to 55 units. Spikes were recorded with a resolution of 0.1 ms. For full details on training, spike-sorting, sleep identification, and histology see Peyrache et al. (2009).

### Data analysis. 
We primarily analyze here data from the 10 learning sessions in which the previously defined learning criteria (Peyrache et al., 2009) were met: the first trial of a block of at least three consecutively rewarded trials after which the performance until the end of the session was 􏰀80%. In later sessions, the rats reached the criterion for changing the rule: 10 consecutive correct trials or one error in 12 trials. By these criteria, each rat learned at least two rules.
We also sought sessions in which the rats made stable choices of strat- egy. For each session, we computed P(rule) as the proportion of trials in which the rat’s choice of arm corresponded to each of the three rules (left, right, cued-arm). Whereas P(left) and P(right) are mutually exclusive, P(cued-arm) is not, and has an expected value of 0.5 when it is not being explicitly chosen because of the random switching of the light cue. A session was deemed to be “stable” if P(rule) was greater than some thresh- old 􏰍 for one of the rules, and the session contained at least 10 trials (this removed only two sessions from consideration). Here we tested both 􏰍 􏰁 0.9 and 􏰍 􏰁 0.85, giving 13 and 17 sessions, respectively. These also, respectively, included 2 and 4 of the rule-change sessions. For the time- series in Figure 1C, E, F, we estimated P(rule) in windows of 7 trials, starting from the first trial, and sliding by one trial.


## Results


## Discussion

