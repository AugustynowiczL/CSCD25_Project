## Deplatforming Dilemma: Unraveling the Shift in Online Polarization After Reddit’s Intervention

### Report
The report file is in the located at `Report.md`

### Abstract
Social media forums and discussion boards allow for users to share and discuss a variety of events ranging from politics to entertainment. However, there has been a rising concern over the possibility of echo chambers within these platforms which polarize their audiences. Many have opinions on how polarization should be handled, and one popular opinion, deplatforming, is one which Reddit went ahead with in 2017. In this work, I investigate the effects of the event and its usefulness in reducing polarization, especially in politically right-leaning spaces. Although polarization seemed to have decreased post-2017, I argue that it is due to a platform shift of these communities rather than a decrease in polarized activity from users.    

### Research Questions 
1. How successful was Reddit’s deplatforming intervention in curbing polarization, especially in right-leaning spaces?
- Have other highly polarized subreddits emerged in recent years? 
2. Is the decrease in polarization due to platform hopping or a successful decrease in polarization?
- Did the users exhibiting polarized activity integrate into other subreddits, or did they leave the platform?

### Hypothesis
The decrease in polarized activity on reddit is a result of users leaving the platform and joining other communication forums and not users becoming more central.

### Methods
- Collect `text_submissions.csv` and `text_comments.csv` datasets
- Cleaning data and converting columns such as UTC time stamps to actual dates.
- Aggregating right and left news source (+2, -2, +1, -1) activity over both `text_comments` and `text_submissions`
- Extract top 10 subreddits activity for each category of Allsides rated news source
- Track activity of these subreddits over the entire dataset by aggregating submissions to these communities.
- Normalize activity to be number of post per day. 
- Collect data for 2020 deplatformed community, r/The_Donald, `thedonald_comments.csv` and `thedonald_submissions.csv`
- Aggregate the activity of submissions and compare with activity of current (+2) subreddits. 
- Perform NLP sentiment analysis of all the (+2 and -2) subreddits and aggregate both.
- Perform NLP sentinment analysis of `thedonald_comments.csv` and check to see if after deplatforming, the sentiment changed to behave more like r/The_Donald.
- Perform temporal analysis on `thedonald_comments.csv` on a word bank of migrational words to determine of users mentioned moving platforms. 

### Conclusions
Overall we found standard results in terms of which subreddits shared the most polarzing new sources, with some being shared with both sides of the spectrum. The analysis suggested that the deplatforming was succesful in the sense that there did not seem to be deep polarized subreddits as existed before such as r/The_Donald, and suggested that the users from these polarized communitity did not integrate themselves into new subreddits, but this is not conclusive. The NLP sentiment analysis and activity suggest that a large portion of the users were discussing moving platforms though the Named Entity Recognition method did not back up this claim. The analysis suggest that the users did not continue to use reddit in a similar manor that was used in the r/The_Donald community. This hints at users leaving the platform, but is possible, even though unlikely, that those users decided to post less polarized material. 


