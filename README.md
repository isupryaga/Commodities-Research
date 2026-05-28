# Commodity Futures Positioning Signal Research Using CFTC COT Data


This project investigates whether extreme commercial positioning in CFTC Commitment of Traders (COT) data contains predictive information about directional price movement in commodity futures.


Using historical COT positioning data across multiple agriculture markets, signal rules were developed based on tail positioning extremes and were then evaluated on their predictive and portfolio performance through backtesting. The project explores:
* positioning normalization
* signal construction
* conditional return behavior
* holding-period performance
* portfolio allocation framework


Key observations from preliminary analysis:
* evidence of conditional return asymmetry following extreme commercial positioning
* varying heavy-tailed return behavior across certain agricultural futures markets
* limited robustness improvements from additional speculative/open-interest conditioning filters


Preliminary backtesting produced risk-adjusted performance metrics consistent with moderate signal persistence across the analyzed sample period (2008-2026). However, results should be interpreted with caution, as there was no strictly out-of-sample validation, and potential for in-sample bias during iterative signal development.


## Repository Structure


* /data
    * Contains cleaned COT dataset.
* 01_cot_data_cleaning.ipynb
    * Cleans and preprocesses raw cumulative COT reports, filtering relevant markets and positioning variables.
* 02_signal_analysis_and_portfolio.ipynb
    * Develops positioning-based trading signals, analyzes conditional return behavior, and constructs portfolio backtests and performance metrics.
* reqs.txt
    * Contains all required libraries.
* writeup.pdf
    * Contains detailed discussion of methodology, findings, and limitations. 

