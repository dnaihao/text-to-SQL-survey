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
    <td>10,181</td>
    <td>200</td>
    <td>138</td>
    <td>5.1</td>
    <td>Domain generalization</td>
    <td>College courses, DabaseAnswers, WikiSQL</td>
  </tr>
  <tr>
    <td>Spider-DK (Gan et al., 2021b)</td>
    <td>535</td>
    <td>10</td>
    <td>-</td>
    <td>4.8</td>
    <td>Domain knowledge</td>
    <td>Spider dev set</td>
  </tr>
  <tr>
    <td>Spiderutran (Zeng et al., 2020)</td>
    <td>15,023</td>
    <td>200</td>
    <td>138</td>
    <td>5.1</td>
    <td>Untranslatable questions</td>
    <td>Spider + 5,330 untranslatable questions</td>
  </tr>
  <tr>
    <td>Spider-L (Lei et al., 2020)</td>
    <td>8,034</td>
    <td>160</td>
    <td>-</td>
    <td>5.1</td>
    <td>Schema Unking</td>
    <td>Spider train/dev</td>
  </tr>
  <tr>
    <td>SpiderSL (Taniguchi et al., 2021)</td>
    <td>1,034</td>
    <td>10</td>
    <td>-</td>
    <td>4.8</td>
    <td>Schema linking</td>
    <td>Spider dev set</td>
  </tr>
  <tr>
    <td>Spider-Syn (Gan et al., 2021a)</td>
    <td>8,034</td>
    <td>160</td>
    <td>-</td>
    <td>5.1</td>
    <td>Robustness</td>
    <td>Spider train/dev</td>
  </tr>
  <tr>
    <td>WikiSQL (Zhong et al., 2017)</td>
    <td>80,654</td>
    <td>26,521</td>
    <td>-</td>
    <td>1</td>
    <td>Data size</td>
    <td>Wikipedia</td>
  </tr>
  <tr>
    <td>Squall (Shi et al., 2020b)</td>
    <td>11,468</td>
    <td>1,679</td>
    <td>-</td>
    <td>1</td>
    <td>Lexicon-level supervision</td>
    <td>WikiTableQuestions (Pasupat and Liang, 2015)</td>
  </tr>
  <tr>
    <td>KaggleDBQA (Lee et al., 2021)</td>
    <td>272</td>
    <td>8</td>
    <td>8</td>
    <td>2.3</td>
    <td>Domain generalization</td>
    <td>Real web daabases</td>
  </tr>
  <tr style="border-bottom: 1px solid #000;">
  <tr>
    <td>ATIS (Price, 1990; Dahl et al., 1994)</td>
    <td>5,280</td>
    <td>1</td>
    <td>1</td>
    <td>32</td>
    <td>-</td>
    <td>FUght-booking</td>
  </tr>
  <tr>
    <td>GeoQuery (Zelle and Mooney, 1996)</td>
    <td>877</td>
    <td>1</td>
    <td>1</td>
    <td>6</td>
    <td>-</td>
    <td>US geography</td>
  </tr>
  <tr>
    <td>Scholar (Iyer et al., 2017)</td>
    <td>817</td>
    <td>1</td>
    <td>1</td>
    <td>7</td>
    <td>-</td>
    <td>Academic publications</td>
  </tr>
  <tr>
    <td>Academic (Li and Jagadish, 2014)</td>
    <td>196</td>
    <td>1</td>
    <td>1</td>
    <td>15</td>
    <td>-</td>
    <td>Microsoft Academic Search (MAS)</td>
  </tr>
  <tr>
    <td>IMDB (Yaghmazadeh et al., 2017)</td>
    <td>131</td>
    <td>1</td>
    <td>1</td>
    <td>16</td>
    <td>-</td>
    <td>database Internet Movie Database</td>
  </tr>
  <tr>
    <td>Yelp (Yaghmazadeh et al., 2017)</td>
    <td>128</td>
    <td>1</td>
    <td>1</td>
    <td>7</td>
    <td>-</td>
    <td>Yelp website</td>
  </tr>
  <tr>
    <td>Advising (Finegan-Dollak et al., 2018)</td>
    <td>3,898</td>
    <td>1</td>
    <td>1</td>
    <td>10</td>
    <td>-</td>
    <td>University of Michigan course</td>
  </tr>
  <tr>
    <td>Restaurants (Tang and Mooney, 2000) (Popescu et al., 2003)</td>
    <td>378</td>
    <td>1</td>
    <td>1</td>
    <td>3</td>
    <td>-</td>
    <td>information Restaurants</td>
  </tr>
  <tr>
    <td>MIMICSQL (Wang et al., 2020d)</td>
    <td>10,000</td>
    <td>1</td>
    <td>1</td>
    <td>5</td>
    <td>-</td>
    <td>Healthcare domain</td>
  </tr>
  <tr>
    <td>SEDE (Hazoom et al., 2021)</td>
    <td>12,023</td>
    <td>1</td>
    <td>1</td>
    <td>29</td>
    <td>SQL template diversity</td>
    <td>Stack Exchange</td>
  </tr>
  <tr>
    <td colspan=7>Summarization for text-to-SQL datasets. #Size, #DB, #D, and #T/DB represent the number of question-SQL
pairs, databases, domains, and tables per domain, respectively. We put “-” in the #D column because we do not
know how many domains are in the Spider dev set and “-” in the Issues Addressed column because there is no
specific issue addressed for the dataset. Datasets above and below the line are cross-domain and single-domain,
respectively.</td>
  </tr>
</tbody>
</table>


## Methods

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
    <td colspan=4>Methods used for encoding in text-to-SQL.</td>
  </tr>
</tbody>
</table>
<div align='center'></div>

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
  <tr><td colspan=5>Methods used for decoding in text-to-SQL. ♠: Academic, Advising, ATIS, GeoQuery, Yelp, IMDB, Scholar, Restaurants; ♡: TableQA DuSQL, CoSQL, Sparc, Chase.</td></tr>
</tbody>
</table>
<!-- <div align='center'></div> -->