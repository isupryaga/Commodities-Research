Hypothesis: On days when the CFTC COT commercial index for corn (ZC) 
is above 0.8 (52-week rolling window), the intraday open-to-close 
return is positive and the pullback from the session open is shallower 
than on non-signal days. 

Entry: Buy at first pullback during hours 14-16 UTC on COT signal days
Exit: Close of session
Filter: cot_idx > 0.8, calculated with 9-day publication lag

Null hypothesis: No difference in OC return between signal and non-signal days

If the 5 year data shows: 

OC return on signal days < 0.05% → no edge, abandon
Pullback depth identical on signal vs non-signal → COT adds nothing intraday
Edge only exists in one sub-period → regime artifact, abandon

Then its false.