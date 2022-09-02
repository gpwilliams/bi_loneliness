# Metadata

This repository contains 4 files at the root directory:

- LICENSE.txt: A text copy of the creative commons license used for this work.
- metadata.md: This file.
- README.md: A readme for navigating this project and the associated OSF repository.
- requirements.txt: A file created by Python to allow for loading the relevant packages (and versions) used in the analysis for computational reproducibility.

The repository is mainly structured around 5 main folders, with the following files:

# /data/:

- cleaned-results.csv: Contains the cleaned data set used for analyses. Has the following columns:
    - PID: Anonymous Participant ID number.
    - DJG: Participants' scores on the De Jong Gierveld 6-item loneliness scale (De Jong Gierveld & Van Tilburg, 2010).
    - single_item: Participants' scores on the single-item loneliness scale. 
    - UCLA: Participants' scores on the UCLA loneliness scale.
    - BRS: Participants' scores on the 6-item Brief Resilience Scale (Smith et al., 2008).
    - WEMWBS: Participants' scores on the 14-item Warwick Edinburgh Mental Well-being Scale (WEMWBS; Tennant et al., 2007).
    - Gender: Participants' gender; M = male, F = female.
    - Age: Participants' age in years.
    - Region: Region to which participants live. If countries are not specified it is implied that this region is England (e.g. North East = North-East England).
    - Martial Status, Living Arrangements, Primary Carer, and Employment are self-explanatory free-text entry responses. Note that for employment FT = full time and PT = part time.
    - BI Severity: Rating of brain injury severity: ordinal from mild, moderate, severe, and very severe.
    - Single/Multiple Impairment: Whether injury is associated with single impairment or multiple impairment. Specific impairments are listed in the remaining columns ranging from Vision to Pain. 

    All scales used short versions to minimise fatigue. Please see the corresponding scales for information on scoring.
    
- compiled-transcripts.pdf: anonymised transcripts for each interview. Coding is explained at the start of the document.

# /docs/:

- analysis.html: contains the html output of the Jupyter notebook explaining the software used and each step of the analysis (including analytical choices) to produce the output for the paper. Note that additional analyses are included here which are not listed in the main body of the paper. Notably, posterior predictive checks and model diagnostics are included here.

- consent.pdf: the consent form given to participants.
- how-to-join-the-interview.pdf: instructions given to participants prior to taking part in the study explaining how to join the interview over Microsoft Teams.
- information.pdf: participant information sheet.
- interview-structure.pdf: an outline of how interviews were conducted with participants.
- standards-for-reporting-qualitative-research.pdf: the guide used to report the qualitative analyses, taken from O'Brien et al. (2014).

# /img/:

Contains several .png images of plots used during the analysis. These are explained in the file /docs/analysis.html, but summaries are as follows:

- plot_impairments.png: Counts of each impairment experienced by participants.
- plot_loo.png: A visual model comparison of the best performing model via PSIS-LOO, the full model (with DJG as a continuous predictor), in comparison to all other models.
- plot_pp_check_BRS.png: Posterior predictive check for the expectation of scores from the full model (with DJG as a continuous predictor) plotted against raw scores and draws from the posterior.
- plot_pp_check_DJG.png: Posterior predictive check for the expectation of scores from the full model (with DJG as a continuous predictor) plotted against raw scores and draws from the posterior.
- plot_pp_check.png: posterior predictive check for the full model (with DJG as a continuous predictor).
- plot_severity.png: Counts of the severity of impairment experienced by participants.
- plot_trace.png: Trace plot with marginal posterior estimates for each parameter from the full model (with DJG as a continuous predictor).
- themes.jpg: an outline of the themes highlighted in the qualitative analysis.

# /python/:

- analysis.ipynb: Jupyter notebook containing Python code and markdown used to produce all analyses and the /docs/analysis.html file.