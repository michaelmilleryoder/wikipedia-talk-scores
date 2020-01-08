# wikipedia-talk-scores
Wikipedia talk page dataset for [Keith Maki, Michael Miller Yoder, Yohan Jo, Carolyn Penstein Rose (2017), Roles and Success in Wikipedia Talk Pages: Identifying Latent Patterns of Behavior, ICWSM.](https://www.aclweb.org/anthology/I17-1103.pdf).

To download data, select `wikipedia_talk_editor_scores.tar.gz` and run `tar xvzf wikipedia_talk_editor_scores.tar.gz` or otherwise uncompress the archive. The only content is a CSV file called `wikipedia_talk_editor_scores.csv`.

Email yoder@cs.cmu.edu with any questions.

## Data columns
Columns in `wikipedia_talk_editor_scores.csv` are explained here:

* `article`: the name of the Wikipedia article from which the talk page conversations are drawn and from which editor scores are calculated.
* `thread`: the name of the talk page discussion thread
* `editor_anonymized`: an anonymized ID that corresponds to which editor made the talk contribution
* `editor_talk`: that editor's contributions to the discussion thread, concatenated
* `other_talk`: other editors' contributions to the discussion thread, concatenated
* `#editor_turns`: the number of discussion turns contributed by that editor
* `#other_turns`: the number of discussion turns contributed by other editors
* `editor_score`: a measure of that editor's success in editing the article page. This is the proportion of modifications the editor made that are still present 24 hours after the last contribution in the discussion thread. Details can be found in the accompanying [paper](https://www.aclweb.org/anthology/I17-1103.pdf), where this measure is the outcome to be predicted from features in the talk.
