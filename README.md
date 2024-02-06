# SPAM-Classification

The Project is based  Machine & Deep Learning models at the interface of NLP and Network Security areas through the use of SMS Spam Collection dataset with helping frameworks & libraries.

# Agenda

*   Theory and Methods
*   General part
    *   Import required libraries and dataset
    *   Some additional & preparing actions & add functions
    *   Reading the Dataset
    *   Dataset manipulations & simple EDA
    *   Dataset size & feature names
    *   Dataset primary statistics
    *   Part A. Advanced Machine Learning for SPAM classification task
    *   Part B. Advanced Deep Learning for SPAM classification task
*   Author

  # Theory and Methods

  The basics of natural language processing (NLP)

The data that we are going to use for this is a subset of an open source default of `SMS Spam Collection dataset`, which contains SMS text examples and its corresponding labels (or tags: `Spam` and `Ham`). The file contains one message per line. Each line consists of two columns: v1 contains the label (`ham` or `spam`) and v2 contains the raw text.

This corpus has been collected from free or free for research sources on the Internet:

*   A collection of 425 SMS spam messages was manually extracted from the Grumbletext website. This is a UK forum where cell phone users make public claims about SMS spam messages, most of them without reporting the very spam message received. The identification of spam messages texts in the claims is a very hard and time-consuming task, and it involved carefully scanning hundreds of web pages. The Grumbletext website is: [Web Link](http://www.grumbletext.co.uk/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkQuickLabsAdvanced_ML_DL_spam_classification_L427910497-2022-01-01).
*   A subset of 3,375 SMS randomly chosen ham messages of the NUS SMS Corpus (NSC), which is a dataset of about 10,000 legitimate messages collected for research at the Department of Computer Science at the National University of Singapore. The messages largely originate from Singaporeans and mostly from students attending the University. These messages were collected from volunteers who were made aware that their contributions were going to be made publicly available. The NUS SMS Corpus is avalaible at: [Web Link](http://www.comp.nus.edu.sg/\~rpnlpir/downloads/corpora/smsCorpus/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkQuickLabsAdvanced_ML_DL_spam_classification_L427910497-2022-01-01).
*   A list of 450 SMS ham messages collected from Caroline Tag's PhD Thesis is available at [Web Link](http://etheses.bham.ac.uk/253/1/Tagg09PhD.pdf?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkQuickLabsAdvanced_ML_DL_spam_classification_L427910497-2022-01-01).
*   Finally, we have incorporated the SMS Spam Corpus v.0.1 Big. It has 1,002 SMS ham messages and 322 spam messages and it is public available at: [Web Link](http://www.esp.uem.es/jmgomez/smsspamcorpus/?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkQuickLabsAdvanced_ML_DL_spam_classification_L427910497-2022-01-01).

The original dataset can be found [here](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-Channel-SkillsNetworkQuickLabsAdvanced_ML_DL_spam_classification_L427910497-2022-01-01). The creators would like to note that in case you find the dataset useful, please, make a reference to the previous paper and the [web page](http://www.dt.fee.unicamp.br/\~tiago/smsspamcollection/) in your papers, research, etc.

This work presents a number of statistics, studies and baseline results for a few machine learning methods.

***

Almeida, T.A., GÃ³mez Hidalgo, J.M., Yamakami, A. Contributions to the Study  of SMS Spam Filtering: New Collection and Results. Proceedings of the 2011 ACM Symposium on Document Engineering (DOCENG'11), Mountain View, CA, USA, 2011.

***

In addition, we will build a visualization of our results, specifically the obtained metrics (accuracy and loss), to choose the best model for further saving and forecasting based on this saved model.
