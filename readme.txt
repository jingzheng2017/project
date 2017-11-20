
A PRACTICAL SPAM CLASSIFIER BASED ON SUPPORT VECTOR MACHINE AND NAÏVE BAYES MODEL:


1.Preprocessed email such as switching into lower case, striping html, punctuation, normalizing numbers, URLs, email address sign.Made a vocabulary list contains 1899 common words and matched words to a word index.Thus features of 1899 dimensions 0-1 vectors were constructed.
2.Used 100 emails(from SpamAssassin Public Corpus) to train SVM model, in which linear, Gaussian, polynomial kernels were selected to fit different types of boundaries. Used 100 emails to test. The accuracy of linear and Gaussian was 95.8% and 94.6%, but the polynomial is only 81.2%.
3.Trained Naive Bayes model, in which we used multinomial model to prevent calculating accuracy problem and Laplace smoothing to prevent zero probability. The average accuracy is lower than the average accuracy of SVM, near to 93%.
4.Meanwhile, we also use our own emails for testing: Sample1.txt(non-spam), Sample2.txt(spam), the result is that both SVM and Naive Bayes could correctly distinguish whether the emails is spam or not.