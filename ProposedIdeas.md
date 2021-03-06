# Project: 
https://competitions.codalab.org/competitions/20022 (just as a reminder ;-) )

# Approaches for Subtask A (fact vs. non-fact, opinion vs. socializing)
- Simple logistic regression or SVM as a basis
- Separate facts from non-facts, then classify opinions vs. socializing comments
- Use of patterns to improve precision of fact vs non-fact estimation as suggested by Oraby et. al

# Approaches for Subtask B (truth estimation)
- Simple features: number of users with the same answer, answers containing links, answer length
- Link checking: does the linked resource contain the answer given?
- Online (or stored) search queries: presence of terms in answer in top results for question keyword search
- Pre-search domain-specific data (e.g. Qatar regulation docs) before widening net to online search
- Persistent user modelling: does a user often give false answers?

# General improvement ideas related to both Tasks:
- Parsing input (question / answers)
- In some ways use output of Subtask A for Subtask B?

# References
Oraby et al. "And That's A Fact: Distinguishing Factual and Emotional Argumentation in Online Dialogue." In Proceedings of the 2nd Workshop on Argumentation Mining at NAACL. 2017. https://arxiv.org/pdf/1709.05295.pdf

Marilyn A. Walker, Pranav Anand, Jean E. Fox Tree, Rob Abbott, Joseph King. "A Corpus for Research on Deliberation and Debate." In Proceedings of the 8th International Conference on Language Resources and Evaluation (LREC), Istanbul, Turkey, 2012. https://nlds.soe.ucsc.edu/iac
