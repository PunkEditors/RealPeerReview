# PunkReview

> Value judgments without gatekeeping

## How a Real Punk Peer Review should work? 

1. Any scientists should be able to express her/his opinion. This is easy if we use e.g. a plug-in to allow user ratings of any paper with a proper DOI from your preferred browser.  
2. To prevent non-scientists (i.e. evil bots) to use it, an authentication via ORCID should work.  
3. It has to be simple. Hence, the simplest question you need to answer is, *Do you trust this paper?*. A second question related to trust is *"Is it reproducible?"*. Those are Yes/No questions. A *Why* 150 words-max will complement those questions. Finally, ranking (e.g. one to five stars) its main assets is useful: Data, Ideas, Controversial (this three axes can be refined). This is fast to perform for reviewers if you have read the paper.    
4. All information should be traceable and transparent.   
5. With this information, you can simply add a badge to the paper with the summary. e.g. "13/16 scientists trust this paper and its main asset is the data quality with an average of 4.8 stars". More complex *ad hoc* metrics can be calculated like who is endorsing you paper, etc...     

## Is something like that already there?

Maybe. Plaudit (https://plaudit.pub/) already developed the plug-in with ORCID validation. It only allow users to select if it's "robust" "clear" and "exciting", which is a good start, but lacks the "why" short thread. It seems easy to integrate in journals (https://plaudit.pub/integration/), but you do need a token and to tag doi's so the plug-in can track them (https://www.npmjs.com/package/get-dois#user-content-supported-meta-tags). Reading the data should be also possible using CrossRef events (https://www.crossref.org/services/event-data/), but this needs some work (https://www.crossref.org/documentation/event-data/use/) because is an experimental source (https://www.eventdata.crossref.org/guide/sources/experimental/#experimental-source-plaudit), and I can't see how the API can be queried for that using (https://github.com/ropensci/rcrossref). Plaudit does it here (https://plaudit.pub/endorsements/doi:10.1101/2021.11.18.469079), and web scrapping is also possible, but inelegant.  

## How can Journals use it?

Brave journals can completely skip classic peer review and move on to real peer review. Papers are no longer accepted / rejected, but after an editorial screening (which can be as though as you want) you can track how much support they receive. Editors can further sumarize the *why?* free text box. Of course, uptake is key here, so creating a supporting community is the first step to make this work, and encourage people to rate papers from their peers.

I would love to integrate this workflow in the Punk-Editors journal. 

