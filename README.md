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

<div align="center">
<img src="imgs/text-to-SQL-framework.png" width="50%"/>
<div align="left" style="width: 50%;">The framework for text-to-SQL systems. Given the database schema and user utterance, the system outputs a corresponding SQL query to query the database system for the result. Appendix B gives more text-to-SQL examples.</div>
</div>


<div align="center">
<img src="imgs/text-to-SQL-topology.png" width="70%"/>
<div align="left" style="width: 50%;">Topology for text-to-SQL. Format adapted from 
<a href="https://arxiv.org/abs/2107.13586" target="_blank">Liu et al. (2021a)</a>
</div>
</div>


## Datasets


| Datasets                                                   |  #Size | #DB #D     | #T/DB | Issues addressed                  | Sources for data                            |
|------------------------------------------------------------|-------:|------------|------:|-----------------------------------|-----------------------------------------    |
| Spider (Yu et al., 2018c)                                  | 10,181 | 200,138    |   5.1 | Domain generalization             | College courses, DabaseAnswers, WikiSQL     |
| Spider-DK (Gan et al., 2021b)                              |    535 |     10     |   4.8 |          Domain knowledge         | Spider dev set                              |
| Spiderutran (Zeng et al., 2020)                            | 15,023 | 200    138 |   5.1 |      Untranslatable questions     | Spider + 5,330 untranslatable questions     |
| Spider-L (Lei et al., 2020)                                |  8,034 | 160        |   5.1 | Schema Unking                     | Spider train/dev                            |
| SpiderSL (Taniguchi et al., 2021)                          |  1,034 |     10     |   4.8 | Schema linking                    | Spider dev set                              |
| Spider-Syn (Gan et al., 2021a)                             |  8,034 | 160        |   5.1 |             Robustness            | Spider train/dev                            |
| WikiSQL (Zhong et al., 2017)                               | 80,654 | 26,521     |     1 |             Data size             | Wikipedia                                   |
| Squall (Shi et al., 2020b)                                 | 11,468 | 1,679      |     1 | Lexicon-level supervision         | WikiTableQuestions (Pasupat and Liang, 2015)|
| KaggleDBQA (Lee et al., 2021)                              |    272 |         88 |   2.3 | Domain generalization             | Real web daabases                           |
| ATIS (Price, 1990; Dahl et al., 1994)                      |  5,280 |         11 |    32 |                 -                 | FUght-booking                               |
| GeoQuery (Zelle and Mooney, 1996)                          |    877 |         11 |     6 |                 -                 | US geography                                |
| Scholar (Iyer et al., 2017)                                |    817 |         11 |     7 |                 -                 | Academic publications                       |
| Academic (Li and Jagadish, 2014)                           |    196 |         11 |    15 |                 -                 | Microsoft Academic Search (MAS)             |
| IMDB (Yaghmazadeh et al., 2017)                            |    131 |         11 |    16 |                 -                 | database Internet Movie Database            |
| Yelp (Yaghmazadeh et al., 2017)                            |    128 |         11 |     7 |                 -                 | Yelp website                                |
| Advising (Finegan-Dollak et al., 2018)                     |  3,898 |         11 |    10 |                 -                 | University of Michigan course               |
| Restaurants (Tang and Mooney, 2000) (Popescu et al., 2003) |    378 |         11 |     3 |                 -                 | information Restaurants                     |
| MIMICSQL (Wang et al., 2020d)                              | 10,000 |         11 |     5 |                 -                 | Healthcare domain                           |
| SEDE (Hazoom et al., 2021)                                 | 12,023 |         11 |    29 |       SQL template diversity      | Stack Exchange                              |


## Encoding

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-dvpl{border-color:inherit;text-align:right;vertical-align:top}
</style>
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
    <td class="tg-0pky" rowspan=8>Leverage external data to represent question and DB schemas</td>
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
</tbody>
</table>

## Decoding