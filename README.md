# Text-to-SQL Survey
Survey about recent advances in text-to-SQL research. This page presents the content in our work [Recent Advances in Text-to-SQL:
A Survey of What We Have and What We Expect](dummy.com)


## Citation

If you would like to cite our work, please cite the following work:

> Naihao Deng, Yulong Chen, and Yue Zhang. 2022. Recent Advances in Text-to-SQL:
A Survey of What We Have and What We Expect

```
dummy
```

## Concept Diagram

|<img src="imgs/text-to-SQL-framework.png" width="50%"/>| 
|:--:| 
| The framework for text-to-SQL systems. Given the database schema and user utterance, the system outputs a corresponding SQL query to query the database system for the result. Appendix B gives more text-to-SQL examples.|



| <img src="imgs/text-to-SQL-topology.png" width="70%"/>| 
|:--:| 
| Topology for text-to-SQL. Format adapted from <a href="https://arxiv.org/abs/2107.13586" target="_blank">Liu et al. (2021a)|


## Datasets



<table>
<thead>
  <tr>
    <th>Datasets</th>
    <th>#Size</th>
    <th>#DB</th>
    <th>#D</th>
    <th>#T/DB</th>
    <th>Issues addressed</th>
    <th>Sources for data</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Spider (Yu et al., 2018c)</td>
    <td align='right'>10,181</td>
    <td align='right'>200</td>
    <td align='right'>138</td>
    <td align='right'>5.1</td>
    <td>Domain generalization</td>
    <td>College courses, DabaseAnswers, WikiSQL</td>
  </tr>
  <tr>
    <td>Spider-DK (Gan et al., 2021b)</td>
    <td align='right'>535</td>
    <td align='right'>10</td>
    <td align='right'>-</td>
    <td align='right'>4.8</td>
    <td>Domain knowledge</td>
    <td>Spider dev set</td>
  </tr>
  <tr>
    <td>Spiderutran (Zeng et al., 2020)</td>
    <td align='right'>15,023</td>
    <td align='right'>200</td>
    <td align='right'>138</td>
    <td align='right'>5.1</td>
    <td>Untranslatable questions</td>
    <td>Spider + 5,330 untranslatable questions</td>
  </tr>
  <tr>
    <td>Spider-L (Lei et al., 2020)</td>
    <td align='right'>8,034</td>
    <td align='right'>160</td>
    <td align='right'>-</td>
    <td align='right'>5.1</td>
    <td>Schema Unking</td>
    <td>Spider train/dev</td>
  </tr>
  <tr>
    <td>SpiderSL (Taniguchi et al., 2021)</td>
    <td align='right'>1,034</td>
    <td align='right'>10</td>
    <td align='right'>-</td>
    <td align='right'>4.8</td>
    <td>Schema linking</td>
    <td>Spider dev set</td>
  </tr>
  <tr>
    <td>Spider-Syn (Gan et al., 2021a)</td>
    <td align='right'>8,034</td>
    <td align='right'>160</td>
    <td align='right'>-</td>
    <td align='right'>5.1</td>
    <td>Robustness</td>
    <td>Spider train/dev</td>
  </tr>
  <tr>
    <td>WikiSQL (Zhong et al., 2017)</td>
    <td align='right'>80,654</td>
    <td align='right'>26,521</td>
    <td align='right'>-</td>
    <td align='right'>1</td>
    <td>Data size</td>
    <td>Wikipedia</td>
  </tr>
  <tr>
    <td>Squall (Shi et al., 2020b)</td>
    <td align='right'>11,468</td>
    <td align='right'>1,679</td>
    <td align='right'>-</td>
    <td align='right'>1</td>
    <td>Lexicon-level supervision</td>
    <td>WikiTableQuestions (Pasupat and Liang, 2015)</td>
  </tr>
  <tr>
    <td>KaggleDBQA (Lee et al., 2021)</td>
    <td align='right'>272</td>
    <td align='right'>8</td>
    <td align='right'>8</td>
    <td align='right'>2.3</td>
    <td>Domain generalization</td>
    <td>Real web daabases</td>
  </tr>
  <tr style="border-bottom: 1px solid #000;">
  <tr>
    <td>ATIS (Price, 1990; Dahl et al., 1994)</td>
    <td align='right'>5,280</td>
    <td align='right'>1</td>
    <td align='right'>1</td>
    <td align='right'>32</td>
    <td>-</td>
    <td>FUght-booking</td>
  </tr>
  <tr>
    <td>GeoQuery (Zelle and Mooney, 1996)</td>
    <td align='right'>877</td>
    <td align='right'>1</td>
    <td align='right'>1</td>
    <td align='right'>6</td>
    <td>-</td>
    <td>US geography</td>
  </tr>
  <tr>
    <td>Scholar (Iyer et al., 2017)</td>
    <td align='right'>817</td>
    <td align='right'>1</td>
    <td align='right'>1</td>
    <td align='right'>7</td>
    <td>-</td>
    <td>Academic publications</td>
  </tr>
  <tr>
    <td>Academic (Li and Jagadish, 2014)</td>
    <td align='right'>196</td>
    <td align='right'>1</td>
    <td align='right'>1</td>
    <td align='right'>15</td>
    <td>-</td>
    <td>Microsoft Academic Search (MAS)</td>
  </tr>
  <tr>
    <td>IMDB (Yaghmazadeh et al., 2017)</td>
    <td align='right'>131</td>
    <td align='right'>1</td>
    <td align='right'>1</td>
    <td align='right'>16</td>
    <td>-</td>
    <td>database Internet Movie Database</td>
  </tr>
  <tr>
    <td>Yelp (Yaghmazadeh et al., 2017)</td>
    <td align='right'>128</td>
    <td align='right'>1</td>
    <td align='right'>1</td>
    <td align='right'>7</td>
    <td>-</td>
    <td>Yelp website</td>
  </tr>
  <tr>
    <td>Advising (Finegan-Dollak et al., 2018)</td>
    <td align='right'>3,898</td>
    <td align='right'>1</td>
    <td align='right'>1</td>
    <td align='right'>10</td>
    <td>-</td>
    <td>University of Michigan course</td>
  </tr>
  <tr>
    <td>Restaurants (Tang and Mooney, 2000) (Popescu et al., 2003)</td>
    <td align='right'>378</td>
    <td align='right'>1</td>
    <td align='right'>1</td>
    <td align='right'>3</td>
    <td>-</td>
    <td>information Restaurants</td>
  </tr>
  <tr>
    <td>MIMICSQL (Wang et al., 2020d)</td>
    <td align='right'>10,000</td>
    <td align='right'>1</td>
    <td align='right'>1</td>
    <td align='right'>5</td>
    <td>-</td>
    <td>Healthcare domain</td>
  </tr>
  <tr>
    <td>SEDE (Hazoom et al., 2021)</td>
    <td align='right'>12,023</td>
    <td align='right'>1</td>
    <td align='right'>1</td>
    <td align='right'>29</td>
    <td>SQL template diversity</td>
    <td>Stack Exchange</td>
  </tr>
  <tr>
    <td colspan=7 align='center'>Summarization for text-to-SQL datasets. #Size, #DB, #D, and #T/DB represent the number of question-SQL
pairs, databases, domains, and tables per domain, respectively. We put “-” in the #D column because we do not
know how many domains are in the Spider dev set and “-” in the Issues Addressed column because there is no
specific issue addressed for the dataset. Datasets above and below the line are cross-domain and single-domain,
respectively.</td>
  </tr>
</tbody>
</table>

### Other relevant datasets

* Chinest text-to-SQL: 
  * CSpider (Min et al., 2019a)
  * TableQA (Sun et al., 2020)
  * DuSQL (Wang et al., 2020c)
  * ESQL (Chen et al., 2021a)
* Vietnamese text-to-SQL: ViText2SQL (Tuan Nguyen et al., 2020)
* Portuguese text-to-SQL: (José and Cozman, 2021)
* Multi-turn context-dependent text-to-SQL:
  * ATIS (Price, 1990) (Dahl et al., 1994)
  * Sparc (Yu et al., 2019b)
  * CoSQL (Yu et al., 2019a)
* Unanswerable questions: TriageSQL (Zhang et al., 2020)


### Resources

* [This Github Repo](https://github.com/jkkummerfeld/text2sql-data) holds data for many of the single domain datasets including Academic, Advising, ATIS, Geography, IMDB, Restaurants, Scholar, Yelp; as well as cross-domain datasets including Spider and WikiSQL. The Github Repo is the official repo for [This paper](https://aclanthology.org/P18-1033/), and their methods of processding the data is described in the paper as well.

* [The official Spider leaderboard](https://yale-lily.github.io/spider) shows the performance of models on Spider dev and the hidden test set.

* [The official WikiSQL Github Repo](https://github.com/salesforce/WikiSQL) holds leaderboard for models on WikiSQL dataset.


<!-- Note of jonanthan's data; note of wikisql and spider leaderboard -->


## Methods

### Data Augmentation

* Typical effects:
  * Handle complex or unseen questions (Zhong et al., 2020b; Wang et al., 2021b)
  * Achieve state-of-the-art with less supervised data (Guo et al., 2018)
  * Attain robustness towards different types of questions (Radhakrishnan et al., 2020)

* Data generation methods:
  * (Iyer et al., 2017)
  * (Li et al., 2020a)

* Quality control of the generated data:
  * (Zhong et al., 2020b)
  * (Wu et al., 2021)

* Diversify the generated data:
  * (Guo et al., 2018)
  * (Radhakrishnan et al., 2020)
  * (Wang et al. 2021b)


### Encoding

<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">Methods</th>
    <th class="tg-0pky">Adopted by</th>
    <th class="tg-dvpl">Applied datasets</th>
    <th class="tg-0pky">Addressed challenges</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">Encode token type</td>
    <td class="tg-0pky">TypeSQL (Yu et al., 2018a)</td>
    <td class="tg-dvpl">WikiSQL</td>
    <td class="tg-0pky">Representing question meaning</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan=8>Graph-based</td>
    <td class="tg-0pky">GNN (Bogin et al., 2019a)</td>
    <td class="tg-dvpl">Spider</td>
    <td class="tg-0pky" rowspan=13>(1)    Representing question and DB schemas in a structured way (2)    Schema linking</td>
  </tr>
  <tr>
    <td class="tg-0pky">Global-GCN (Bogin et al., 2019b)</td>
    <td class="tg-dvpl">Spider</td>
  </tr>
  <tr>
    <td class="tg-0pky">IGSQL (Cai and Wan, 2020)</td>
    <td class="tg-dvpl">Sparc, CoSQL</td>
  </tr>
  <tr>
    <td class="tg-0pky">RAT-SQL (Wang et al., 2020a)</td>
    <td class="tg-dvpl">Spider</td>
  </tr>
  <tr>
    <td class="tg-0pky">LEGSQL (Cao et al., 2021)</td>
    <td class="tg-dvpl">Spider</td>
  </tr>
  <tr>
    <td class="tg-0pky">SADGA (Cai et al., 2021)</td>
    <td class="tg-dvpl">Spider</td>
  </tr>
  <tr>
    <td class="tg-0pky">ShawdowGNN (Chen et al., 2021b)</td>
    <td class="tg-dvpl">Spider</td>
  </tr>
  <tr>
    <td class="tg-0pky">S2SQL (Hui et al., 2022)</td>
    <td class="tg-dvpl">Spider, Spider-Syn</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan=5>Self-attention</td>
    <td class="tg-0pky">X-SQL (He et al., 2019)</td>
    <td class="tg-dvpl">WikiSQL</td>
  </tr>
  <tr>
    <td class="tg-0pky">SQLova (Hwang et al., 2019)</td>
    <td class="tg-dvpl">WikiSQL</td>
  </tr>
  <tr>
    <td class="tg-0pky">RAT-SQL (Wang et al., 2020a)</td>
    <td class="tg-dvpl">Spider</td>
  </tr>
  <tr>
    <td class="tg-0pky">DuoRAT (Scholak et al., 2021a)</td>
    <td class="tg-dvpl">Spider</td>
  </tr>
  <tr>
    <td class="tg-0pky">UnifiedSKG (Xie et al., 2022)</td>
    <td class="tg-dvpl">WikiSQL, Spider</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan=5>Adapt PLM</td>
    <td class="tg-0pky">X-SQL (He et al., 2019)</td>
    <td class="tg-dvpl">WikiSQL</td>
    <td class="tg-0pky" rowspan=8>Leveraging external data to represent question and DB schemas</td>
  </tr>
  <tr>
    <td class="tg-0pky">SQLova (Hwang et al., 2019)</td>
    <td class="tg-dvpl">WikiSQL</td>
  </tr>
  <tr>
    <td class="tg-0pky">Guo and Gao (2019)</td>
    <td class="tg-dvpl">WikiSQL</td>
  </tr>
  <tr>
    <td class="tg-0pky">HydraNet (Lyu et al., 2020)</td>
    <td class="tg-dvpl">WikiSQL</td>
  </tr>
  <tr>
    <td class="tg-0pky">Liu et al. (2021b), etc</td>
    <td class="tg-dvpl">Spider-L, SQUALL</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan=3>Pre-training</td>
    <td class="tg-0pky">TaBERT (Yin et al., 2020)</td>
    <td class="tg-dvpl">Spider</td>
  </tr>
  <tr>
    <td class="tg-0pky">GraPPA (Yu et al., 2021)</td>
    <td class="tg-dvpl">Spider</td>
  </tr>
  <tr>
    <td class="tg-0pky">GAP (Shi et al., 2020a)</td>
    <td class="tg-dvpl">Spider</td>
  </tr>
  <tr>
    <td colspan=4 align='center'>Methods used for encoding in text-to-SQL.</td>
  </tr>
</tbody>
</table>

## Decoding


<table>
<thead>
  <tr>
    <th>Methods</th>
    <th></th>
    <th>Adopted by</th>
    <th>Applied datasets</th>
    <th>Addressed challenges</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td rowspan=3>Tree-based</td>
    <td></td>
    <td>Seq2Tree (Dong and Lapata, 2016)</td>
    <td>-</td>
    <td rowspan=8>Hierarchical decoding</td>
  </tr>
  <tr>
    <td></td>
    <td>Seq2AST (Yin and Neubig, 2017)</td>
    <td>-</td>
  </tr>
  <tr>
    <td></td>
    <td>SyntaxSQLNet (Yu et al., 2018b)</td>
    <td>Spider</td>
  </tr>
  <tr>
    <td rowspan=4>Sketch-based</td>
    <td></td>
    <td>SQLNet (Xu et al., 2017)</td>
    <td>WikiSQL</td>
  </tr>
  <tr>
    <td></td>
    <td>(Dong and Lapata, 2018)</td>
    <td>WikiSQL</td>
  </tr>
  <tr>
    <td></td>
    <td>IRNet (Guo et al., 2019)</td>
    <td>Spider</td>
  </tr>
  <tr>
    <td></td>
    <td>RYANSQL (Choi et al., 2021)</td>
    <td>Spider</td>
  </tr>
  <tr>
    <td>Bottom-up</td>
    <td></td>
    <td>SmBop (Rubin and Berant, 2021)</td>
    <td>Spider</td>
  </tr>
  <tr>
    <td rowspan=5>Attention Mechanism</td>
    <td rowspan="2">Attention</td>
    <td>Seq2Tree (Dong and Lapata, 2016)</td>
    <td>-</td>
    <td rowspan=9>Synthesizing information for decoding</td>
  </tr>
  <tr>
    <td>Seq2SQL (Zhong et al., 2017)</td>
    <td>WikiSQL</td>
  </tr>
  <tr>
    <td>Bi-attention</td>
    <td>Guo and Gao (2018)</td>
    <td>WikiSQL</td>
  </tr>
  <tr>
    <td>Structured attention</td>
    <td>Wang et al. (2019)</td>
    <td>WikiSQL</td>
  </tr>
  <tr>
    <td>Relation-aware Self-attention</td>
    <td>DuoRAT (Scholak et al., 2021a)</td>
    <td>Spider</td>
  </tr>
  <tr>
    <td rowspan=4>Copy Mechanism</td>
    <td></td>
    <td>Seq2AST (Yin and Neubig, 2017)</td>
    <td>-</td>
  </tr>
  <tr>
    <td></td>
    <td>Seq2SQL (Zhong et al., 2017)</td>
    <td>WikiSQL</td>
  </tr>
  <tr>
    <td></td>
    <td>Wang et al. (2018a)</td>
    <td>WikiSQL</td>
  </tr>
  <tr>
    <td></td>
    <td>SeqGenSQL (Li et al., 2020a)</td>
    <td>WikiSQL</td>
  </tr>
  <tr>
    <td rowspan=6>Intermediate Representation</td>
    <td></td>
    <td>IncSQL (Shi et al., 2018)</td>
    <td>WikiSQL</td>
    <td rowspan=6>Brdiging the gap between natural language and SQL query</td>
  </tr>
  <tr>
    <td></td>
    <td>IRNet (Guo et al., 2019)</td>
    <td>Spider</td>
  </tr>
  <tr>
    <td></td>
    <td>Suhr et al. (2020)</td>
    <td>Spider and others♠</td>
  </tr>
  <tr>
    <td></td>
    <td>Herzig et al. (2021)</td>
    <td>GeoQuery, ATIS, Scholar</td>
  </tr>
  <tr>
    <td></td>
    <td>Gan et al. (2021c)</td>
    <td>Spider</td>
  </tr>
  <tr>
    <td></td>
    <td>Brunner and Stockinger (2021)</td>
    <td>Spider</td>
  </tr>
  <tr>
    <td rowspan=11>Others</td>
    <td rowspan=2>Constrained decoding</td>
    <td>UniSAr (Dou et al., 2022)</td>
    <td>WikiSQL, Spide and others♡</td>
    <td rowspan=4>Fine-grained decoding</td>
  </tr>
  <tr>
    <td>PICARD (Scholak et al., 2021b)</td>
    <td>Spider, CoSQL</td>
  </tr>
  <tr>
    <td rowspan=2>Execution-guided</td>
    <td>SQLova (Hwang et al., 2019)</td>
    <td>WikiSQL</td>
  </tr>
  <tr>
    <td>Wang et al. (2018b)</td>
    <td>WikiSQL</td>
  </tr>
  <tr>
    <td rowspan=2>Discriminative re-ranking</td>
    <td>Global-GCN Bogin et al. (2019b)</td>
    <td>Spider</td>
    <td rowspan="2">SQL Ranking</td>
  </tr>
  <tr>
    <td>Kelkar et al. (2020)</td>
    <td>Spider</td>
  </tr>
  <tr>
    <td rowspan=3>Separate submodule</td>
    <td>SQLNet (Xu et al., 2017)</td>
    <td>WikiSQL</td>
    <td rowspan=4>Easier decoding</td>
  </tr>
  <tr>
    <td>Guo and Gao (2018)</td>
    <td>WikiSQL</td>
  </tr>
  <tr>
    <td>Lee (2019)</td>
    <td>Spider</td>
  </tr>
  <tr>
    <td>BPE</td>
    <td>Muller and Vlachos (2019)</td>
    <td>Advising, ATIS, GeoQuery</td>
  </tr>
  <tr>
    <td>Link gating</td>
    <td>Chen et al. (2020b)</td>
    <td>Spider</td>
    <td>Synthesizing information for decoding</td>
  </tr>
  <tr><td colspan=5 align='center'>Methods used for decoding in text-to-SQL. ♠: Academic, Advising, ATIS, GeoQuery, Yelp, IMDB, Scholar, Restaurants; ♡: TableQA DuSQL, CoSQL, Sparc, Chase.</td></tr>
</tbody>
</table>

### Learning Techniques

* Fully supervised
  * Active learning (Ni et al., 2020)
  * Interactive/Imitation learning (Yao et al., 2019) (Yao et al., 2020)
  * Meta-learning (Huang et al., 2018) (Wang et al., 2021a) (Chen et al., 2021a)
  * Multi-task learning (Chang et al., 2020) (Xuan et al., 2021) (Hui et al., 2021b) (Shi et al., 2021) (McCann et al., 2018) (Xie et al., 2022)

* Weakly supervised
  * Reinforcement learning (Zhong et al., 2017) (Liang et al., 2018)
  * Meta-learning and Bayesian optimization (Agarwal et al., 2019)
  * (Min et al., 2019b)


### Miscellaneous

* DB linking:
  * (Lin et al., 2020)
  * (Ma et al., 2020)
* Model-wise:
  * (Finegan-Dollak et al., 2018)
  * (Shaw et al., 2021)
  * (Yan et al., 2020)
  * (Xu et al., 2021)
* SQL generation:
  * (Shi et al., 2018)
  * (Brunner and Stockinger, 2021)

For context-dependent text-to-SQL:
* Turn-level encoder and copy mechanism (Suhr et al., 2018) (Zhang et al., 2019) (Wang et al., 2020b)
* Constrained decoding (Wang et al., 2020b)
* Dynamic memory decay mechanism (Hui et al., 2021a)
* (Zheng et al., 2022)


## Evaluation

### Metrics

<table>
<thead>
  <tr>
    <th>Metrics</th>
    <th>Datasets</th>
    <th>Errors</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Naiive Execution Accuracy</td>
    <td>GeoQuery, IMDB, Yelp, WikiSQL, etc</td>
    <td>False positive</td>
  </tr>
  <tr>
    <td>Exact String Match</td>
    <td>Advising, WikiSQL, etc</td>
    <td>False negative</td>
  </tr>
  <tr>
    <td>Exact Set Match</td>
    <td>Spider</td>
    <td>False negative</td>
  </tr>
  <tr>
    <td>Test Suite Accuracy (execution accuracy with generated databases)</td>
    <td>Spider, GeoQuery, etc</td>
    <td>False positive</td>
  </tr>
  <tr>
    <td colspan=3 align='center'>The summary of metrics, datasets that use these metrics, and their potential error cases.</td>
  </tr>
</tbody>
</table>

### Evaluation Setup
* Question split: split the question-SQL pairs randomly (Iyer et al., 2017).
* SQL query split: no SQL query is allowed to appear in more than one set among the train, dev, and test sets (Finegan-Dollak et al., 2018)
* Database split: databases in the test set do not appear in the training time (Yu et al., 2018c)
* Others (Shaw et al., 2021) (Chang et al., 2020)

## Discussion and Future Directions

* Cross-domain text-to-SQL: incorporate domain knowledge to models trained on the existing datasets, and deploy such models efficiently on different domains.

* Real-world use cases:
  * Handle corrupted tables or scenarios where no table is provided.
  * Handle user inputs different from the existing datasets.
  * Facilitate DB administrator to manage DB schemas, updating DB content.
  * Multi-lingual text-to-SQL.
  * DB interface for the disabled.

* Integrated into a larger scope of research:
  * QA system for DB.
  * Dialogue system with knowledge from DB.
  * Explore the inter-relation between SQL and other logical forms.
  * Generalized semantic parsing.

* Others:
  * Apply prompt learning to text-to-SQL: how to make the system robust.
  * Evalulation of the existing text-to-SQL systems.


## Text-to-SQL examples

### Example of the table in the database

The domain for Restaurant dataset is restaurant information, where questions are typically about food type, restaurant location, etc.

There is a big difference in terms of how many tables a database has. For restaurants, there are 3
tables in the database, while there are 32 tables in ATIS (Suhr et al., 2020).

<table>
<thead>
  <tr>
    <th>CITY.NAME*</th>
    <th>COUNTY</th>
    <th>REGION</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>VARCHAR(255)</td>
    <td>VARCHAR(255)</td>
    <td>VARCHAR(255)</td>
  </tr>
  <tr>
    <td>Alameda</td>
    <td>Alameda County</td>
    <td>Bay Area</td>
  </tr>
  <tr>
    <td>Alamo</td>
    <td>Contra Costa County</td>
    <td>Bay Area</td>
  </tr>
  <tr>
    <td>Albany</td>
    <td>Alameda County</td>
    <td>Bay Area</td>
  </tr>
  <tr>
    <td>...</td>
    <td>...</td>
    <td>...</td>
  </tr>
  <tr>
    <td colspan=3>Geography, one of the 3 tables in Restaurants database. * denotes the primary key of this table. We only include 3 rows for demonstration purpose.</td>
  </tr>
</tbody>
</table>

### Domain Knowledge

*Question*: 
```
Will undergrads be okay to take 581 ?
```

*SQL query*:
```sql
SELECT DISTINCT T1.ADVISORY_REQUIREMENT , T1.ENFORCED_REQUIREMENT , T1.NAME FROM COURSE AS T1 WHERE T1.DEPARTMENT = "EECS" AND T1.NUMBER = 581 ;
```

In Advising dataset, Department “EECS” is considered as domain knowledge where “581” in the
utterance means a course in “EECS” department with course number “581”.

### Dataset Convention

*Question*: 
```
Give me some restaurants in alameda ?
```

*SQL query*:
```sql
SELECT T1.HOUSE_NUMBER , T2.NAME FROM LOCATION AS T1 , RESTAURANT AS T2 WHERE T1.CITY_NAME = "alameda" AND T2.ID = T1.RESTAURANT_ID ;
```

In Restaurants dataset, when the user queries “restaurants”, by dataset convention, the corresponding SQL query returns the column “HOUSE_NUMBER” and “NAME”.


### Text-to-SQL Templates

An example of the template for text-to-SQL pair used by (Iyer et al., 2017) is as follows:

*Question template*: 
```
Get all <ENT1>.<NAME> having <ENT2>.<COL1>.<NAME> as <ENT2>.<COL1>.<TYPE>
```

*SQL query template*:

```sql
SELECT <ENT1>.<DEF> FROM JOIN_FROM(<ENT1>, <ENT2>) WHERE JOIN_WHERE(<ENT1>, <ENT2>) AND <ENT2>.<COL1> = <ENT2>.<COL1>.<TYPE> ;
```

*Generated question*: 
```
Get all author having dataset as DATASET_TYPE
```

*Generated SQL query*:
```sql
SELECT author.authorId FROM author , writes , paper , paperDataset , dataset WHERE author. authorId = writes.authorId AND writes.paperId = paper.paperId AND paper.paperId = paperDataset.paperId AND paperDataset.datasetId = dataset. datasetId AND dataset.datasetName = DATASET_TYPE
``` 
, where they populate the slots in the templates with table and column names from the database schema, as well as join the corresponding tables accordingly.

(Iyer et al., 2017) also uses PPDB (Ganitkevitch et al., 2013) to paraphrase the NL. An example of PPDB paraphrasing is `thrown into jail` and `imprisoned`.

[This Github Repo](https://github.com/jkkummerfeld/text2sql-data) also holds NL-SQL templates for Academic, Advising, ATIS, Geography, IMDB, Restaurants, Scholar, Yelp, where they mask the corresponding entities in the NL-SQL pairs.

### Complexity of NL-SQL pairs

(Yu et al., 2018c) defines the SQL hardness as the number of SQL components. The SQL query is harder when it contains more SQL keywords such as `GROUP BY` and nested subqueries. Here are some examples from the original paper:

*Easy*:
```sql
SELECT COUNT(*) FROM cars_data WHERE cylinders > 4
```

*Medium*:
```sql
SELECT T2.name, COUNT(*) FROM concert AS T1 JOIN stadium AS T2 ON T1.stadium_id = T2.stadium_id GROUP BY T1.stadium_id
```

*Hard*:
```sql
SELECT T1.country_name FROM countries AS T1 JOIN continents AS T2 ON T1.continent = T2.cont_id JOIN car_makers AS T3 ON T1.country_id = T3. country WHERE T2.continent = ’Europe’ GROUP BY T1.country_name HAVING COUNT(*) >= 3
```

*Extra Hard*:
```sql
SELECT AVG(life_expectancy) FROM country WHERE name NOT IN (SELECT T1.name FROM country AS T1 JOIN country_language AS T2 ON T1.code = T2.country_code WHERE T2.language = "English" AND T2.is_official = "T")
```

There is no qualitative measure of how hard the NL is. Intuitively, models’ performance can decrease when faced with longer questions from users. However, the information conveyed in longer sentences can be more complete, while there can be ambiguity in shorter sentences. Besides, there can be domain-specific phrases that confuse the model in both short and long utterances (Suhr et al., 2020). Thus, researchers need to consider various perspectives to determine the complexity of natural utterance.


