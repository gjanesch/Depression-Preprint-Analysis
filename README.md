This code is intended for a casual analysis of preprints on the topic of depression.  It goes from data collection via webscraping to analysis of the preprints with Latent Dirichlet Allocation.  A writeup of the analysis can be found [here].

The three notebooks' purposes are as follows:
* "01 OSF Scraper" consists of scraping the [Open Science Foundation website](https://osf.io/) for information on preprints in general, as an initial survey of sorts for the topic.
* "02 PsyArXiv Scraper" is a more targeted scraper, covering only [PsyArXiv](https://psyarxiv.com/).  It is similar to the preceding notebook, but with less analysis and the addition of downloading the preprints.
* "03 Extract Paper Texts" is the analysis of the preprints themselves.  It performs analysis using both Latent Dirichlet Allocation and non-negative matrix factorization, though only the former was used in the writeup.  Much of the code is based on [an example in the `scikit-learn` documentation](https://scikit-learn.org/stable/auto_examples/applications/plot_topics_extraction_with_nmf_lda.html).

The two CSV files include information on the preprints' pages that were scraped.  Including the preprints themselves was not practical due to size (a few hundred megabytes).
