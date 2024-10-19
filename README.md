# Analysis Methods for a CSCL survey dataset
This repository contains three NLP methods to identify clusters of common themes among replies within the open dataset (add link). 
The dataset contains four open-ended questions about definitions of Computer Supported Collaborative Learning (CSCL), Collaborative Learning, the difference participants make between collaborative and cooperative learning and the future of the field. The dataset contains 50 replies by members of the CSCL research community.
- How do you define Computer Supported Collaborative Learning (CSCL) ?
- How do you define Collaborative Learning (CL) in CSCL ?
- Do you distinguish Collaborative Learning and Cooperative Learning ?
    - If yes, how so ?
    - If no, why not ?
- Where do you see CSCL heading towards in the future ?

All methods are documented in the following OSF preregistration (add link)

## Topic-Modeling
Latent Dirichlet Allocation (LDA) models each document (or answer) as a probability distribution over latent topics (concepts), and each topic as a distribution over words. By extracting these topic distributions from each answer, we can identify common concepts and uncover shared ground among different answers. 

## Text-Embedding-Kmeans
Cluster all open-ended survey responses related to definitions relevant to CSCL by response type using OpenAI's text-embedding-3-small model. Interpret clusters by analyzing typical responses via cosine similarity and highlight high-signal words using TF-IDF analysis.

## Dual-Sonnet-Model-Calls
Emulate a thematic analysis workflow with a Claude 3.5 Sonnet LLM