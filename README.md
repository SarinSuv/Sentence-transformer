---
pipeline_tag: sentence-similarity
tags:
- sentence-transformers
- feature-extraction
- sentence-similarity
- mteb
language: en
license: apache-2.0
datasets:
- s2orc
- flax-sentence-embeddings/stackexchange_xml
- MS Marco
- gooaq
- yahoo_answers_topics
- code_search_net
- search_qa
- eli5
- snli
- multi_nli
- wikihow
- natural_questions
- trivia_qa
- embedding-data/sentence-compression
- embedding-data/flickr30k-captions
- embedding-data/altlex
- embedding-data/simple-wiki
- embedding-data/QQP
- embedding-data/SPECTER
- embedding-data/PAQ_pairs
- embedding-data/WikiAnswers
model-index:
- name: all-MiniLM-L12-v2
  results:
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_counterfactual
      name: MTEB AmazonCounterfactualClassification (en)
      config: en
      split: test
    metrics:
    - type: accuracy
      value: 65.28358208955224
    - type: ap
      value: 28.02247873560022
    - type: f1
      value: 59.09977445939425
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_counterfactual
      name: MTEB AmazonCounterfactualClassification (de)
      config: de
      split: test
    metrics:
    - type: accuracy
      value: 57.09850107066381
    - type: ap
      value: 73.38224986285773
    - type: f1
      value: 55.183322516223434
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_counterfactual
      name: MTEB AmazonCounterfactualClassification (en-ext)
      config: en-ext
      split: test
    metrics:
    - type: accuracy
      value: 67.24137931034483
    - type: ap
      value: 17.93337056203553
    - type: f1
      value: 55.200711090858846
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_counterfactual
      name: MTEB AmazonCounterfactualClassification (ja)
      config: ja
      split: test
    metrics:
    - type: accuracy
      value: 59.91434689507494
    - type: ap
      value: 13.610920446878454
    - type: f1
      value: 48.70464699796398
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_polarity
      name: MTEB AmazonPolarityClassification
      config: default
      split: test
    metrics:
    - type: accuracy
      value: 62.984899999999996
    - type: ap
      value: 58.19701547898307
    - type: f1
      value: 62.704020410756144
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_reviews_multi
      name: MTEB AmazonReviewsClassification (en)
      config: en
      split: test
    metrics:
    - type: accuracy
      value: 30.792
    - type: f1
      value: 30.254565315575437
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_reviews_multi
      name: MTEB AmazonReviewsClassification (de)
      config: de
      split: test
    metrics:
    - type: accuracy
      value: 25.907999999999998
    - type: f1
      value: 25.538149526380543
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_reviews_multi
      name: MTEB AmazonReviewsClassification (es)
      config: es
      split: test
    metrics:
    - type: accuracy
      value: 27.634000000000004
    - type: f1
      value: 27.287076320171728
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_reviews_multi
      name: MTEB AmazonReviewsClassification (fr)
      config: fr
      split: test
    metrics:
    - type: accuracy
      value: 27.540000000000003
    - type: f1
      value: 27.21486019130574
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_reviews_multi
      name: MTEB AmazonReviewsClassification (ja)
      config: ja
      split: test
    metrics:
    - type: accuracy
      value: 23.566000000000003
    - type: f1
      value: 23.3492650771905
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_reviews_multi
      name: MTEB AmazonReviewsClassification (zh)
      config: zh
      split: test
    metrics:
    - type: accuracy
      value: 22.99
    - type: f1
      value: 22.47175043426865
  - task:
      type: Retrieval
    dataset:
      type: arguana
      name: MTEB ArguAna
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 23.257
    - type: map_at_10
      value: 38.083
    - type: map_at_100
      value: 39.263999999999996
    - type: map_at_1000
      value: 39.273
    - type: map_at_3
      value: 32.574999999999996
    - type: map_at_5
      value: 35.669000000000004
    - type: mrr_at_1
      value: 23.613
    - type: mrr_at_10
      value: 38.243
    - type: mrr_at_100
      value: 39.410000000000004
    - type: mrr_at_1000
      value: 39.419
    - type: mrr_at_3
      value: 32.883
    - type: mrr_at_5
      value: 35.766999999999996
    - type: ndcg_at_1
      value: 23.257
    - type: ndcg_at_10
      value: 47.128
    - type: ndcg_at_100
      value: 52.093
    - type: ndcg_at_1000
      value: 52.315999999999995
    - type: ndcg_at_3
      value: 35.794
    - type: ndcg_at_5
      value: 41.364000000000004
    - type: precision_at_1
      value: 23.257
    - type: precision_at_10
      value: 7.632
    - type: precision_at_100
      value: 0.979
    - type: precision_at_1000
      value: 0.1
    - type: precision_at_3
      value: 15.055
    - type: precision_at_5
      value: 11.735
    - type: recall_at_1
      value: 23.257
    - type: recall_at_10
      value: 76.31599999999999
    - type: recall_at_100
      value: 97.866
    - type: recall_at_1000
      value: 99.57300000000001
    - type: recall_at_3
      value: 45.164
    - type: recall_at_5
      value: 58.677
  - task:
      type: Clustering
    dataset:
      type: mteb/arxiv-clustering-p2p
      name: MTEB ArxivClusteringP2P
      config: default
      split: test
    metrics:
    - type: v_measure
      value: 46.06982724111873
  - task:
      type: Clustering
    dataset:
      type: mteb/arxiv-clustering-s2s
      name: MTEB ArxivClusteringS2S
      config: default
      split: test
    metrics:
    - type: v_measure
      value: 37.501829188148264
  - task:
      type: Reranking
    dataset:
      type: mteb/askubuntudupquestions-reranking
      name: MTEB AskUbuntuDupQuestions
      config: default
      split: test
    metrics:
    - type: map
      value: 64.06160552465775
    - type: mrr
      value: 77.40029899309677
  - task:
      type: STS
    dataset:
      type: mteb/biosses-sts
      name: MTEB BIOSSES
      config: default
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 86.73300462416691
    - type: cos_sim_spearman
      value: 83.56756679430214
    - type: euclidean_pearson
      value: 84.35153960397948
    - type: euclidean_spearman
      value: 83.56756679430214
    - type: manhattan_pearson
      value: 84.10087673223914
    - type: manhattan_spearman
      value: 83.58383222516198
  - task:
      type: Classification
    dataset:
      type: mteb/banking77
      name: MTEB Banking77Classification
      config: default
      split: test
    metrics:
    - type: accuracy
      value: 80.40259740259741
    - type: f1
      value: 79.7932665380276
  - task:
      type: Clustering
    dataset:
      type: mteb/biorxiv-clustering-p2p
      name: MTEB BiorxivClusteringP2P
      config: default
      split: test
    metrics:
    - type: v_measure
      value: 36.985834019439366
  - task:
      type: Clustering
    dataset:
      type: mteb/biorxiv-clustering-s2s
      name: MTEB BiorxivClusteringS2S
      config: default
      split: test
    metrics:
    - type: v_measure
      value: 33.207831360185644
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackAndroidRetrieval
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 34.975
    - type: map_at_10
      value: 47.227999999999994
    - type: map_at_100
      value: 48.91
    - type: map_at_1000
      value: 49.016
    - type: map_at_3
      value: 43.334
    - type: map_at_5
      value: 45.353
    - type: mrr_at_1
      value: 43.348
    - type: mrr_at_10
      value: 53.744
    - type: mrr_at_100
      value: 54.432
    - type: mrr_at_1000
      value: 54.458
    - type: mrr_at_3
      value: 51.359
    - type: mrr_at_5
      value: 52.825
    - type: ndcg_at_1
      value: 43.348
    - type: ndcg_at_10
      value: 54.118
    - type: ndcg_at_100
      value: 59.496
    - type: ndcg_at_1000
      value: 60.846999999999994
    - type: ndcg_at_3
      value: 49.001
    - type: ndcg_at_5
      value: 51.245
    - type: precision_at_1
      value: 43.348
    - type: precision_at_10
      value: 10.658
    - type: precision_at_100
      value: 1.701
    - type: precision_at_1000
      value: 0.214
    - type: precision_at_3
      value: 23.701
    - type: precision_at_5
      value: 17.082
    - type: recall_at_1
      value: 34.975
    - type: recall_at_10
      value: 66.291
    - type: recall_at_100
      value: 88.727
    - type: recall_at_1000
      value: 97.26700000000001
    - type: recall_at_3
      value: 51.505
    - type: recall_at_5
      value: 57.833
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackEnglishRetrieval
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 31.509999999999998
    - type: map_at_10
      value: 43.401
    - type: map_at_100
      value: 44.762
    - type: map_at_1000
      value: 44.906
    - type: map_at_3
      value: 39.83
    - type: map_at_5
      value: 41.784
    - type: mrr_at_1
      value: 39.936
    - type: mrr_at_10
      value: 49.534
    - type: mrr_at_100
      value: 50.126000000000005
    - type: mrr_at_1000
      value: 50.163999999999994
    - type: mrr_at_3
      value: 46.996
    - type: mrr_at_5
      value: 48.508
    - type: ndcg_at_1
      value: 39.936
    - type: ndcg_at_10
      value: 49.845
    - type: ndcg_at_100
      value: 54.25600000000001
    - type: ndcg_at_1000
      value: 56.227000000000004
    - type: ndcg_at_3
      value: 44.982
    - type: ndcg_at_5
      value: 47.187
    - type: precision_at_1
      value: 39.936
    - type: precision_at_10
      value: 9.771
    - type: precision_at_100
      value: 1.575
    - type: precision_at_1000
      value: 0.20600000000000002
    - type: precision_at_3
      value: 22.314
    - type: precision_at_5
      value: 15.975
    - type: recall_at_1
      value: 31.509999999999998
    - type: recall_at_10
      value: 61.468
    - type: recall_at_100
      value: 80.023
    - type: recall_at_1000
      value: 92.267
    - type: recall_at_3
      value: 46.698
    - type: recall_at_5
      value: 53.03600000000001
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackGamingRetrieval
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 38.577
    - type: map_at_10
      value: 51.041000000000004
    - type: map_at_100
      value: 52.141000000000005
    - type: map_at_1000
      value: 52.190000000000005
    - type: map_at_3
      value: 47.904
    - type: map_at_5
      value: 49.645
    - type: mrr_at_1
      value: 44.138
    - type: mrr_at_10
      value: 54.36
    - type: mrr_at_100
      value: 55.05799999999999
    - type: mrr_at_1000
      value: 55.084
    - type: mrr_at_3
      value: 52.017
    - type: mrr_at_5
      value: 53.321
    - type: ndcg_at_1
      value: 44.138
    - type: ndcg_at_10
      value: 56.855999999999995
    - type: ndcg_at_100
      value: 61.133
    - type: ndcg_at_1000
      value: 62.17399999999999
    - type: ndcg_at_3
      value: 51.624
    - type: ndcg_at_5
      value: 54.108999999999995
    - type: precision_at_1
      value: 44.138
    - type: precision_at_10
      value: 9.16
    - type: precision_at_100
      value: 1.2309999999999999
    - type: precision_at_1000
      value: 0.135
    - type: precision_at_3
      value: 23.156
    - type: precision_at_5
      value: 15.762
    - type: recall_at_1
      value: 38.577
    - type: recall_at_10
      value: 70.638
    - type: recall_at_100
      value: 89.01
    - type: recall_at_1000
      value: 96.53699999999999
    - type: recall_at_3
      value: 56.635000000000005
    - type: recall_at_5
      value: 62.731
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackGisRetrieval
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 27.038
    - type: map_at_10
      value: 36.108000000000004
    - type: map_at_100
      value: 37.316
    - type: map_at_1000
      value: 37.396
    - type: map_at_3
      value: 33.206
    - type: map_at_5
      value: 34.674
    - type: mrr_at_1
      value: 29.04
    - type: mrr_at_10
      value: 37.979
    - type: mrr_at_100
      value: 39.056000000000004
    - type: mrr_at_1000
      value: 39.11
    - type: mrr_at_3
      value: 35.348
    - type: mrr_at_5
      value: 36.675999999999995
    - type: ndcg_at_1
      value: 29.04
    - type: ndcg_at_10
      value: 41.408
    - type: ndcg_at_100
      value: 46.918
    - type: ndcg_at_1000
      value: 48.827
    - type: ndcg_at_3
      value: 35.699999999999996
    - type: ndcg_at_5
      value: 38.112
    - type: precision_at_1
      value: 29.04
    - type: precision_at_10
      value: 6.463000000000001
    - type: precision_at_100
      value: 0.9570000000000001
    - type: precision_at_1000
      value: 0.116
    - type: precision_at_3
      value: 15.104000000000001
    - type: precision_at_5
      value: 10.508000000000001
    - type: recall_at_1
      value: 27.038
    - type: recall_at_10
      value: 55.989
    - type: recall_at_100
      value: 80.418
    - type: recall_at_1000
      value: 94.506
    - type: recall_at_3
      value: 40.388000000000005
    - type: recall_at_5
      value: 46.085
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackMathematicaRetrieval
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 17.264
    - type: map_at_10
      value: 26.157000000000004
    - type: map_at_100
      value: 27.503
    - type: map_at_1000
      value: 27.617000000000004
    - type: map_at_3
      value: 23.247999999999998
    - type: map_at_5
      value: 24.81
    - type: mrr_at_1
      value: 21.144
    - type: mrr_at_10
      value: 30.516
    - type: mrr_at_100
      value: 31.607000000000003
    - type: mrr_at_1000
      value: 31.673000000000002
    - type: mrr_at_3
      value: 27.716
    - type: mrr_at_5
      value: 29.357
    - type: ndcg_at_1
      value: 21.144
    - type: ndcg_at_10
      value: 31.86
    - type: ndcg_at_100
      value: 38.12
    - type: ndcg_at_1000
      value: 40.699000000000005
    - type: ndcg_at_3
      value: 26.411
    - type: ndcg_at_5
      value: 28.896
    - type: precision_at_1
      value: 21.144
    - type: precision_at_10
      value: 5.995
    - type: precision_at_100
      value: 1.058
    - type: precision_at_1000
      value: 0.14100000000000001
    - type: precision_at_3
      value: 12.894
    - type: precision_at_5
      value: 9.428
    - type: recall_at_1
      value: 17.264
    - type: recall_at_10
      value: 45.074
    - type: recall_at_100
      value: 71.817
    - type: recall_at_1000
      value: 89.846
    - type: recall_at_3
      value: 30.031000000000002
    - type: recall_at_5
      value: 36.233
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackPhysicsRetrieval
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 28.668
    - type: map_at_10
      value: 40.382
    - type: map_at_100
      value: 41.836
    - type: map_at_1000
      value: 41.954
    - type: map_at_3
      value: 37.136
    - type: map_at_5
      value: 38.755
    - type: mrr_at_1
      value: 35.13
    - type: mrr_at_10
      value: 45.928999999999995
    - type: mrr_at_100
      value: 46.814
    - type: mrr_at_1000
      value: 46.854
    - type: mrr_at_3
      value: 43.423
    - type: mrr_at_5
      value: 44.79
    - type: ndcg_at_1
      value: 35.13
    - type: ndcg_at_10
      value: 46.81
    - type: ndcg_at_100
      value: 52.552
    - type: ndcg_at_1000
      value: 54.493
    - type: ndcg_at_3
      value: 41.732
    - type: ndcg_at_5
      value: 43.847
    - type: precision_at_1
      value: 35.13
    - type: precision_at_10
      value: 8.738999999999999
    - type: precision_at_100
      value: 1.373
    - type: precision_at_1000
      value: 0.174
    - type: precision_at_3
      value: 20.372
    - type: precision_at_5
      value: 14.302000000000001
    - type: recall_at_1
      value: 28.668
    - type: recall_at_10
      value: 60.038000000000004
    - type: recall_at_100
      value: 83.736
    - type: recall_at_1000
      value: 96.184
    - type: recall_at_3
      value: 45.647999999999996
    - type: recall_at_5
      value: 51.212
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackProgrammersRetrieval
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 25.287
    - type: map_at_10
      value: 35.351
    - type: map_at_100
      value: 36.867
    - type: map_at_1000
      value: 36.973
    - type: map_at_3
      value: 32.176
    - type: map_at_5
      value: 33.894999999999996
    - type: mrr_at_1
      value: 31.735000000000003
    - type: mrr_at_10
      value: 40.832
    - type: mrr_at_100
      value: 41.812
    - type: mrr_at_1000
      value: 41.864000000000004
    - type: mrr_at_3
      value: 38.489000000000004
    - type: mrr_at_5
      value: 39.654
    - type: ndcg_at_1
      value: 31.735000000000003
    - type: ndcg_at_10
      value: 41.327999999999996
    - type: ndcg_at_100
      value: 47.565000000000005
    - type: ndcg_at_1000
      value: 49.708000000000006
    - type: ndcg_at_3
      value: 36.391
    - type: ndcg_at_5
      value: 38.489000000000004
    - type: precision_at_1
      value: 31.735000000000003
    - type: precision_at_10
      value: 7.7170000000000005
    - type: precision_at_100
      value: 1.2670000000000001
    - type: precision_at_1000
      value: 0.16199999999999998
    - type: precision_at_3
      value: 17.808
    - type: precision_at_5
      value: 12.534
    - type: recall_at_1
      value: 25.287
    - type: recall_at_10
      value: 53.735
    - type: recall_at_100
      value: 80.149
    - type: recall_at_1000
      value: 94.756
    - type: recall_at_3
      value: 39.475
    - type: recall_at_5
      value: 45.532000000000004
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackRetrieval
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 26.613
    - type: map_at_10
      value: 36.747416666666666
    - type: map_at_100
      value: 38.091416666666674
    - type: map_at_1000
      value: 38.2075
    - type: map_at_3
      value: 33.630833333333335
    - type: map_at_5
      value: 35.28225
    - type: mrr_at_1
      value: 31.654
    - type: mrr_at_10
      value: 40.94166666666666
    - type: mrr_at_100
      value: 41.85883333333334
    - type: mrr_at_1000
      value: 41.910666666666664
    - type: mrr_at_3
      value: 38.44458333333334
    - type: mrr_at_5
      value: 39.84525000000001
    - type: ndcg_at_1
      value: 31.654
    - type: ndcg_at_10
      value: 42.533
    - type: ndcg_at_100
      value: 48.09741666666667
    - type: ndcg_at_1000
      value: 50.170166666666674
    - type: ndcg_at_3
      value: 37.37858333333333
    - type: ndcg_at_5
      value: 39.666666666666664
    - type: precision_at_1
      value: 31.654
    - type: precision_at_10
      value: 7.649500000000001
    - type: precision_at_100
      value: 1.2425
    - type: precision_at_1000
      value: 0.16175
    - type: precision_at_3
      value: 17.49625
    - type: precision_at_5
      value: 12.410333333333332
    - type: recall_at_1
      value: 26.613
    - type: recall_at_10
      value: 55.33375
    - type: recall_at_100
      value: 79.52791666666667
    - type: recall_at_1000
      value: 93.73391666666667
    - type: recall_at_3
      value: 40.861333333333334
    - type: recall_at_5
      value: 46.84675
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackStatsRetrieval
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 26.079
    - type: map_at_10
      value: 33.481
    - type: map_at_100
      value: 34.494
    - type: map_at_1000
      value: 34.589999999999996
    - type: map_at_3
      value: 31.165
    - type: map_at_5
      value: 32.482
    - type: mrr_at_1
      value: 29.293999999999997
    - type: mrr_at_10
      value: 36.303000000000004
    - type: mrr_at_100
      value: 37.183
    - type: mrr_at_1000
      value: 37.254
    - type: mrr_at_3
      value: 34.33
    - type: mrr_at_5
      value: 35.519
    - type: ndcg_at_1
      value: 29.293999999999997
    - type: ndcg_at_10
      value: 37.817
    - type: ndcg_at_100
      value: 42.91
    - type: ndcg_at_1000
      value: 45.342
    - type: ndcg_at_3
      value: 33.695
    - type: ndcg_at_5
      value: 35.747
    - type: precision_at_1
      value: 29.293999999999997
    - type: precision_at_10
      value: 5.951
    - type: precision_at_100
      value: 0.9400000000000001
    - type: precision_at_1000
      value: 0.121
    - type: precision_at_3
      value: 14.519000000000002
    - type: precision_at_5
      value: 10.123
    - type: recall_at_1
      value: 26.079
    - type: recall_at_10
      value: 48.27
    - type: recall_at_100
      value: 71.64
    - type: recall_at_1000
      value: 89.775
    - type: recall_at_3
      value: 36.858000000000004
    - type: recall_at_5
      value: 42.013
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackTexRetrieval
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 18.17
    - type: map_at_10
      value: 26.483
    - type: map_at_100
      value: 27.732
    - type: map_at_1000
      value: 27.864
    - type: map_at_3
      value: 23.76
    - type: map_at_5
      value: 25.290000000000003
    - type: mrr_at_1
      value: 22.436
    - type: mrr_at_10
      value: 30.448999999999998
    - type: mrr_at_100
      value: 31.476
    - type: mrr_at_1000
      value: 31.548
    - type: mrr_at_3
      value: 28.051
    - type: mrr_at_5
      value: 29.421999999999997
    - type: ndcg_at_1
      value: 22.436
    - type: ndcg_at_10
      value: 31.662000000000003
    - type: ndcg_at_100
      value: 37.611
    - type: ndcg_at_1000
      value: 40.439
    - type: ndcg_at_3
      value: 26.939999999999998
    - type: ndcg_at_5
      value: 29.177999999999997
    - type: precision_at_1
      value: 22.436
    - type: precision_at_10
      value: 5.908
    - type: precision_at_100
      value: 1.056
    - type: precision_at_1000
      value: 0.149
    - type: precision_at_3
      value: 12.962000000000002
    - type: precision_at_5
      value: 9.476999999999999
    - type: recall_at_1
      value: 18.17
    - type: recall_at_10
      value: 43.219
    - type: recall_at_100
      value: 70.106
    - type: recall_at_1000
      value: 90.04100000000001
    - type: recall_at_3
      value: 30.023
    - type: recall_at_5
      value: 35.845
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackUnixRetrieval
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 28.016999999999996
    - type: map_at_10
      value: 38.123000000000005
    - type: map_at_100
      value: 39.367000000000004
    - type: map_at_1000
      value: 39.467999999999996
    - type: map_at_3
      value: 34.836
    - type: map_at_5
      value: 36.661
    - type: mrr_at_1
      value: 33.116
    - type: mrr_at_10
      value: 42.211
    - type: mrr_at_100
      value: 43.118
    - type: mrr_at_1000
      value: 43.169000000000004
    - type: mrr_at_3
      value: 39.521
    - type: mrr_at_5
      value: 41.154
    - type: ndcg_at_1
      value: 33.116
    - type: ndcg_at_10
      value: 43.86
    - type: ndcg_at_100
      value: 49.486000000000004
    - type: ndcg_at_1000
      value: 51.487
    - type: ndcg_at_3
      value: 38.303
    - type: ndcg_at_5
      value: 40.927
    - type: precision_at_1
      value: 33.116
    - type: precision_at_10
      value: 7.649
    - type: precision_at_100
      value: 1.165
    - type: precision_at_1000
      value: 0.145
    - type: precision_at_3
      value: 17.724
    - type: precision_at_5
      value: 12.668
    - type: recall_at_1
      value: 28.016999999999996
    - type: recall_at_10
      value: 57.032000000000004
    - type: recall_at_100
      value: 81.828
    - type: recall_at_1000
      value: 95.273
    - type: recall_at_3
      value: 41.733
    - type: recall_at_5
      value: 48.496
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackWebmastersRetrieval
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 24.295
    - type: map_at_10
      value: 34.94
    - type: map_at_100
      value: 36.659000000000006
    - type: map_at_1000
      value: 36.902
    - type: map_at_3
      value: 31.562
    - type: map_at_5
      value: 33.28
    - type: mrr_at_1
      value: 29.644
    - type: mrr_at_10
      value: 39.467999999999996
    - type: mrr_at_100
      value: 40.561
    - type: mrr_at_1000
      value: 40.61
    - type: mrr_at_3
      value: 36.759
    - type: mrr_at_5
      value: 38.251000000000005
    - type: ndcg_at_1
      value: 29.644
    - type: ndcg_at_10
      value: 41.376000000000005
    - type: ndcg_at_100
      value: 47.701
    - type: ndcg_at_1000
      value: 49.925999999999995
    - type: ndcg_at_3
      value: 36.009
    - type: ndcg_at_5
      value: 38.23
    - type: precision_at_1
      value: 29.644
    - type: precision_at_10
      value: 8.182
    - type: precision_at_100
      value: 1.672
    - type: precision_at_1000
      value: 0.253
    - type: precision_at_3
      value: 17.325
    - type: precision_at_5
      value: 12.450999999999999
    - type: recall_at_1
      value: 24.295
    - type: recall_at_10
      value: 54.478
    - type: recall_at_100
      value: 81.85
    - type: recall_at_1000
      value: 95.395
    - type: recall_at_3
      value: 39.121
    - type: recall_at_5
      value: 45.465
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackWordpressRetrieval
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 19.476
    - type: map_at_10
      value: 28.274
    - type: map_at_100
      value: 29.509999999999998
    - type: map_at_1000
      value: 29.614
    - type: map_at_3
      value: 25.413000000000004
    - type: map_at_5
      value: 26.758
    - type: mrr_at_1
      value: 20.887
    - type: mrr_at_10
      value: 29.975
    - type: mrr_at_100
      value: 31.063000000000002
    - type: mrr_at_1000
      value: 31.14
    - type: mrr_at_3
      value: 27.326
    - type: mrr_at_5
      value: 28.666000000000004
    - type: ndcg_at_1
      value: 20.887
    - type: ndcg_at_10
      value: 33.456
    - type: ndcg_at_100
      value: 39.421
    - type: ndcg_at_1000
      value: 41.873
    - type: ndcg_at_3
      value: 27.755000000000003
    - type: ndcg_at_5
      value: 30.032999999999998
    - type: precision_at_1
      value: 20.887
    - type: precision_at_10
      value: 5.601
    - type: precision_at_100
      value: 0.915
    - type: precision_at_1000
      value: 0.125
    - type: precision_at_3
      value: 12.076
    - type: precision_at_5
      value: 8.613999999999999
    - type: recall_at_1
      value: 19.476
    - type: recall_at_10
      value: 47.772999999999996
    - type: recall_at_100
      value: 75.031
    - type: recall_at_1000
      value: 92.96
    - type: recall_at_3
      value: 32.221
    - type: recall_at_5
      value: 37.68
  - task:
      type: Retrieval
    dataset:
      type: climate-fever
      name: MTEB ClimateFEVER
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 8.341999999999999
    - type: map_at_10
      value: 14.524000000000001
    - type: map_at_100
      value: 16.114
    - type: map_at_1000
      value: 16.301
    - type: map_at_3
      value: 11.904
    - type: map_at_5
      value: 13.175
    - type: mrr_at_1
      value: 18.892999999999997
    - type: mrr_at_10
      value: 29.185
    - type: mrr_at_100
      value: 30.368000000000002
    - type: mrr_at_1000
      value: 30.418
    - type: mrr_at_3
      value: 25.548
    - type: mrr_at_5
      value: 27.708
    - type: ndcg_at_1
      value: 18.892999999999997
    - type: ndcg_at_10
      value: 21.572
    - type: ndcg_at_100
      value: 28.51
    - type: ndcg_at_1000
      value: 32.204
    - type: ndcg_at_3
      value: 16.753
    - type: ndcg_at_5
      value: 18.5
    - type: precision_at_1
      value: 18.892999999999997
    - type: precision_at_10
      value: 6.997000000000001
    - type: precision_at_100
      value: 1.433
    - type: precision_at_1000
      value: 0.211
    - type: precision_at_3
      value: 12.53
    - type: precision_at_5
      value: 10.098
    - type: recall_at_1
      value: 8.341999999999999
    - type: recall_at_10
      value: 27.215
    - type: recall_at_100
      value: 51.534
    - type: recall_at_1000
      value: 72.655
    - type: recall_at_3
      value: 15.634
    - type: recall_at_5
      value: 20.227
  - task:
      type: Retrieval
    dataset:
      type: dbpedia-entity
      name: MTEB DBPedia
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 7.5920000000000005
    - type: map_at_10
      value: 15.42
    - type: map_at_100
      value: 21.269
    - type: map_at_1000
      value: 22.55
    - type: map_at_3
      value: 11.221
    - type: map_at_5
      value: 13.225999999999999
    - type: mrr_at_1
      value: 58.25
    - type: mrr_at_10
      value: 66.237
    - type: mrr_at_100
      value: 66.74799999999999
    - type: mrr_at_1000
      value: 66.762
    - type: mrr_at_3
      value: 64.167
    - type: mrr_at_5
      value: 65.229
    - type: ndcg_at_1
      value: 45.625
    - type: ndcg_at_10
      value: 33.355000000000004
    - type: ndcg_at_100
      value: 37.484
    - type: ndcg_at_1000
      value: 44.523
    - type: ndcg_at_3
      value: 37.879000000000005
    - type: ndcg_at_5
      value: 35.841
    - type: precision_at_1
      value: 58.25
    - type: precision_at_10
      value: 26.450000000000003
    - type: precision_at_100
      value: 8.290000000000001
    - type: precision_at_1000
      value: 1.744
    - type: precision_at_3
      value: 40.75
    - type: precision_at_5
      value: 35.0
    - type: recall_at_1
      value: 7.5920000000000005
    - type: recall_at_10
      value: 20.064
    - type: recall_at_100
      value: 43.187
    - type: recall_at_1000
      value: 66.154
    - type: recall_at_3
      value: 12.366000000000001
    - type: recall_at_5
      value: 15.631
  - task:
      type: Classification
    dataset:
      type: mteb/emotion
      name: MTEB EmotionClassification
      config: default
      split: test
    metrics:
    - type: accuracy
      value: 41.17
    - type: f1
      value: 36.961926373935974
  - task:
      type: Retrieval
    dataset:
      type: fever
      name: MTEB FEVER
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 37.361
    - type: map_at_10
      value: 49.407000000000004
    - type: map_at_100
      value: 50.11600000000001
    - type: map_at_1000
      value: 50.151999999999994
    - type: map_at_3
      value: 46.608
    - type: map_at_5
      value: 48.286
    - type: mrr_at_1
      value: 40.204
    - type: mrr_at_10
      value: 52.714000000000006
    - type: mrr_at_100
      value: 53.347
    - type: mrr_at_1000
      value: 53.373000000000005
    - type: mrr_at_3
      value: 49.935
    - type: mrr_at_5
      value: 51.626000000000005
    - type: ndcg_at_1
      value: 40.204
    - type: ndcg_at_10
      value: 55.905
    - type: ndcg_at_100
      value: 59.229
    - type: ndcg_at_1000
      value: 60.077000000000005
    - type: ndcg_at_3
      value: 50.367
    - type: ndcg_at_5
      value: 53.291999999999994
    - type: precision_at_1
      value: 40.204
    - type: precision_at_10
      value: 8.0
    - type: precision_at_100
      value: 0.979
    - type: precision_at_1000
      value: 0.106
    - type: precision_at_3
      value: 20.997
    - type: precision_at_5
      value: 14.215
    - type: recall_at_1
      value: 37.361
    - type: recall_at_10
      value: 72.775
    - type: recall_at_100
      value: 87.883
    - type: recall_at_1000
      value: 94.204
    - type: recall_at_3
      value: 57.830000000000005
    - type: recall_at_5
      value: 64.888
  - task:
      type: Retrieval
    dataset:
      type: fiqa
      name: MTEB FiQA2018
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 18.257
    - type: map_at_10
      value: 29.694
    - type: map_at_100
      value: 31.593
    - type: map_at_1000
      value: 31.795
    - type: map_at_3
      value: 25.778000000000002
    - type: map_at_5
      value: 27.901999999999997
    - type: mrr_at_1
      value: 36.574
    - type: mrr_at_10
      value: 45.562000000000005
    - type: mrr_at_100
      value: 46.479
    - type: mrr_at_1000
      value: 46.52
    - type: mrr_at_3
      value: 43.184
    - type: mrr_at_5
      value: 44.558
    - type: ndcg_at_1
      value: 36.574
    - type: ndcg_at_10
      value: 37.274
    - type: ndcg_at_100
      value: 44.379000000000005
    - type: ndcg_at_1000
      value: 47.803000000000004
    - type: ndcg_at_3
      value: 33.999
    - type: ndcg_at_5
      value: 34.927
    - type: precision_at_1
      value: 36.574
    - type: precision_at_10
      value: 10.571
    - type: precision_at_100
      value: 1.779
    - type: precision_at_1000
      value: 0.23700000000000002
    - type: precision_at_3
      value: 22.942
    - type: precision_at_5
      value: 16.944
    - type: recall_at_1
      value: 18.257
    - type: recall_at_10
      value: 43.46
    - type: recall_at_100
      value: 70.017
    - type: recall_at_1000
      value: 90.838
    - type: recall_at_3
      value: 30.520999999999997
    - type: recall_at_5
      value: 35.977
  - task:
      type: Retrieval
    dataset:
      type: hotpotqa
      name: MTEB HotpotQA
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 25.935000000000002
    - type: map_at_10
      value: 35.96
    - type: map_at_100
      value: 36.811
    - type: map_at_1000
      value: 36.894
    - type: map_at_3
      value: 33.479
    - type: map_at_5
      value: 34.93
    - type: mrr_at_1
      value: 51.870000000000005
    - type: mrr_at_10
      value: 59.671
    - type: mrr_at_100
      value: 60.153
    - type: mrr_at_1000
      value: 60.183
    - type: mrr_at_3
      value: 57.815000000000005
    - type: mrr_at_5
      value: 58.965999999999994
    - type: ndcg_at_1
      value: 51.870000000000005
    - type: ndcg_at_10
      value: 44.589
    - type: ndcg_at_100
      value: 48.113
    - type: ndcg_at_1000
      value: 49.962
    - type: ndcg_at_3
      value: 40.304
    - type: ndcg_at_5
      value: 42.543
    - type: precision_at_1
      value: 51.870000000000005
    - type: precision_at_10
      value: 9.454
    - type: precision_at_100
      value: 1.225
    - type: precision_at_1000
      value: 0.147
    - type: precision_at_3
      value: 25.131999999999998
    - type: precision_at_5
      value: 16.851
    - type: recall_at_1
      value: 25.935000000000002
    - type: recall_at_10
      value: 47.272
    - type: recall_at_100
      value: 61.229
    - type: recall_at_1000
      value: 73.55199999999999
    - type: recall_at_3
      value: 37.698
    - type: recall_at_5
      value: 42.126999999999995
  - task:
      type: Classification
    dataset:
      type: mteb/imdb
      name: MTEB ImdbClassification
      config: default
      split: test
    metrics:
    - type: accuracy
      value: 59.76079999999999
    - type: ap
      value: 55.90381572041755
    - type: f1
      value: 58.99832553463791
  - task:
      type: Retrieval
    dataset:
      type: msmarco
      name: MTEB MSMARCO
      config: default
      split: dev
    metrics:
    - type: map_at_1
      value: 20.666999999999998
    - type: map_at_10
      value: 32.425
    - type: map_at_100
      value: 33.586
    - type: map_at_1000
      value: 33.643
    - type: map_at_3
      value: 28.836000000000002
    - type: map_at_5
      value: 30.847
    - type: mrr_at_1
      value: 21.275
    - type: mrr_at_10
      value: 33.062999999999995
    - type: mrr_at_100
      value: 34.168
    - type: mrr_at_1000
      value: 34.217999999999996
    - type: mrr_at_3
      value: 29.491
    - type: mrr_at_5
      value: 31.502999999999997
    - type: ndcg_at_1
      value: 21.246000000000002
    - type: ndcg_at_10
      value: 39.034
    - type: ndcg_at_100
      value: 44.768
    - type: ndcg_at_1000
      value: 46.2
    - type: ndcg_at_3
      value: 31.652
    - type: ndcg_at_5
      value: 35.257
    - type: precision_at_1
      value: 21.246000000000002
    - type: precision_at_10
      value: 6.196
    - type: precision_at_100
      value: 0.909
    - type: precision_at_1000
      value: 0.10300000000000001
    - type: precision_at_3
      value: 13.547999999999998
    - type: precision_at_5
      value: 9.946000000000002
    - type: recall_at_1
      value: 20.666999999999998
    - type: recall_at_10
      value: 59.321999999999996
    - type: recall_at_100
      value: 86.158
    - type: recall_at_1000
      value: 97.154
    - type: recall_at_3
      value: 39.160000000000004
    - type: recall_at_5
      value: 47.82
  - task:
      type: Classification
    dataset:
      type: mteb/mtop_domain
      name: MTEB MTOPDomainClassification (en)
      config: en
      split: test
    metrics:
    - type: accuracy
      value: 91.89922480620154
    - type: f1
      value: 91.66762682851963
  - task:
      type: Classification
    dataset:
      type: mteb/mtop_domain
      name: MTEB MTOPDomainClassification (de)
      config: de
      split: test
    metrics:
    - type: accuracy
      value: 72.03719357565511
    - type: f1
      value: 68.75742308679864
  - task:
      type: Classification
    dataset:
      type: mteb/mtop_domain
      name: MTEB MTOPDomainClassification (es)
      config: es
      split: test
    metrics:
    - type: accuracy
      value: 72.98532354903269
    - type: f1
      value: 71.33173021994274
  - task:
      type: Classification
    dataset:
      type: mteb/mtop_domain
      name: MTEB MTOPDomainClassification (fr)
      config: fr
      split: test
    metrics:
    - type: accuracy
      value: 75.59348575007829
    - type: f1
      value: 73.1511918522243
  - task:
      type: Classification
    dataset:
      type: mteb/mtop_domain
      name: MTEB MTOPDomainClassification (hi)
      config: hi
      split: test
    metrics:
    - type: accuracy
      value: 40.36213696665471
    - type: f1
      value: 37.865703085609475
  - task:
      type: Classification
    dataset:
      type: mteb/mtop_domain
      name: MTEB MTOPDomainClassification (th)
      config: th
      split: test
    metrics:
    - type: accuracy
      value: 17.099457504520796
    - type: f1
      value: 12.86835498185132
  - task:
      type: Classification
    dataset:
      type: mteb/mtop_intent
      name: MTEB MTOPIntentClassification (en)
      config: en
      split: test
    metrics:
    - type: accuracy
      value: 62.83629730962153
    - type: f1
      value: 44.241027031016735
  - task:
      type: Classification
    dataset:
      type: mteb/mtop_intent
      name: MTEB MTOPIntentClassification (de)
      config: de
      split: test
    metrics:
    - type: accuracy
      value: 43.412228796844175
    - type: f1
      value: 25.96122949091921
  - task:
      type: Classification
    dataset:
      type: mteb/mtop_intent
      name: MTEB MTOPIntentClassification (es)
      config: es
      split: test
    metrics:
    - type: accuracy
      value: 41.8812541694463
    - type: f1
      value: 27.93481154758236
  - task:
      type: Classification
    dataset:
      type: mteb/mtop_intent
      name: MTEB MTOPIntentClassification (fr)
      config: fr
      split: test
    metrics:
    - type: accuracy
      value: 38.93830253679925
    - type: f1
      value: 25.820783392796052
  - task:
      type: Classification
    dataset:
      type: mteb/mtop_intent
      name: MTEB MTOPIntentClassification (hi)
      config: hi
      split: test
    metrics:
    - type: accuracy
      value: 17.7518823951237
    - type: f1
      value: 11.681226129204576
  - task:
      type: Classification
    dataset:
      type: mteb/mtop_intent
      name: MTEB MTOPIntentClassification (th)
      config: th
      split: test
    metrics:
    - type: accuracy
      value: 5.631103074141048
    - type: f1
      value: 2.046543337618445
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (af)
      config: af
      split: test
    metrics:
    - type: accuracy
      value: 38.94082044384667
    - type: f1
      value: 36.222023448848596
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (am)
      config: am
      split: test
    metrics:
    - type: accuracy
      value: 2.451244115669133
    - type: f1
      value: 1.1859369824825732
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (ar)
      config: ar
      split: test
    metrics:
    - type: accuracy
      value: 20.938130464021523
    - type: f1
      value: 17.984223607695032
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (az)
      config: az
      split: test
    metrics:
    - type: accuracy
      value: 34.25016812373907
    - type: f1
      value: 33.954933856088616
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (bn)
      config: bn
      split: test
    metrics:
    - type: accuracy
      value: 13.665097511768659
    - type: f1
      value: 12.091606412618153
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (cy)
      config: cy
      split: test
    metrics:
    - type: accuracy
      value: 35.7128446536651
    - type: f1
      value: 33.62071051640523
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (da)
      config: da
      split: test
    metrics:
    - type: accuracy
      value: 44.425016812373904
    - type: f1
      value: 41.20770166767181
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (de)
      config: de
      split: test
    metrics:
    - type: accuracy
      value: 44.1661062542031
    - type: f1
      value: 40.374580049860995
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (el)
      config: el
      split: test
    metrics:
    - type: accuracy
      value: 28.698722259583054
    - type: f1
      value: 24.131330009557754
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (en)
      config: en
      split: test
    metrics:
    - type: accuracy
      value: 67.14862138533961
    - type: f1
      value: 65.29267177342918
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (es)
      config: es
      split: test
    metrics:
    - type: accuracy
      value: 40.907868190988566
    - type: f1
      value: 39.705805513162154
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (fa)
      config: fa
      split: test
    metrics:
    - type: accuracy
      value: 23.517148621385342
    - type: f1
      value: 20.450403227141454
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (fi)
      config: fi
      split: test
    metrics:
    - type: accuracy
      value: 39.27370544720915
    - type: f1
      value: 36.44557663703388
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (fr)
      config: fr
      split: test
    metrics:
    - type: accuracy
      value: 44.81506388702085
    - type: f1
      value: 42.61335088326293
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (he)
      config: he
      split: test
    metrics:
    - type: accuracy
      value: 23.648285137861468
    - type: f1
      value: 19.948568467541378
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (hi)
      config: hi
      split: test
    metrics:
    - type: accuracy
      value: 17.97579018157364
    - type: f1
      value: 16.06739661356912
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (hu)
      config: hu
      split: test
    metrics:
    - type: accuracy
      value: 37.995965030262276
    - type: f1
      value: 35.26841971527663
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (hy)
      config: hy
      split: test
    metrics:
    - type: accuracy
      value: 8.691997310020176
    - type: f1
      value: 7.237344584036491
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (id)
      config: id
      split: test
    metrics:
    - type: accuracy
      value: 39.66039004707465
    - type: f1
      value: 38.775085127634476
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (is)
      config: is
      split: test
    metrics:
    - type: accuracy
      value: 35.141223940820446
    - type: f1
      value: 33.61281534585094
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (it)
      config: it
      split: test
    metrics:
    - type: accuracy
      value: 43.17081371889711
    - type: f1
      value: 41.80158989235553
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (ja)
      config: ja
      split: test
    metrics:
    - type: accuracy
      value: 30.944855413584392
    - type: f1
      value: 27.785702058036733
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (jv)
      config: jv
      split: test
    metrics:
    - type: accuracy
      value: 36.69468728984533
    - type: f1
      value: 34.21258336813279
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (ka)
      config: ka
      split: test
    metrics:
    - type: accuracy
      value: 9.169468728984533
    - type: f1
      value: 6.904570655222885
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (km)
      config: km
      split: test
    metrics:
    - type: accuracy
      value: 4.986550100874243
    - type: f1
      value: 1.7161855654054863
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (kn)
      config: kn
      split: test
    metrics:
    - type: accuracy
      value: 3.0766644250168125
    - type: f1
      value: 1.9577724201468871
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (ko)
      config: ko
      split: test
    metrics:
    - type: accuracy
      value: 19.966375252185607
    - type: f1
      value: 16.545470254940454
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (lv)
      config: lv
      split: test
    metrics:
    - type: accuracy
      value: 38.61129791526564
    - type: f1
      value: 37.447802930149614
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (ml)
      config: ml
      split: test
    metrics:
    - type: accuracy
      value: 2.85137861466039
    - type: f1
      value: 0.8642500845287098
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (mn)
      config: mn
      split: test
    metrics:
    - type: accuracy
      value: 23.24815063887021
    - type: f1
      value: 22.162182623622098
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (ms)
      config: ms
      split: test
    metrics:
    - type: accuracy
      value: 36.21385339609952
    - type: f1
      value: 33.62879988681565
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (my)
      config: my
      split: test
    metrics:
    - type: accuracy
      value: 4.381304640215198
    - type: f1
      value: 1.4197071894925672
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (nb)
      config: nb
      split: test
    metrics:
    - type: accuracy
      value: 41.91324815063887
    - type: f1
      value: 38.890562616282196
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (nl)
      config: nl
      split: test
    metrics:
    - type: accuracy
      value: 41.85272360457296
    - type: f1
      value: 38.79874724974811
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (pl)
      config: pl
      split: test
    metrics:
    - type: accuracy
      value: 37.632817753866846
    - type: f1
      value: 34.5071421221765
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (pt)
      config: pt
      split: test
    metrics:
    - type: accuracy
      value: 45.12104909213182
    - type: f1
      value: 43.32946794837761
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (ro)
      config: ro
      split: test
    metrics:
    - type: accuracy
      value: 41.71486213853396
    - type: f1
      value: 39.500043810450016
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (ru)
      config: ru
      split: test
    metrics:
    - type: accuracy
      value: 26.3315400134499
    - type: f1
      value: 24.213252556865477
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (sl)
      config: sl
      split: test
    metrics:
    - type: accuracy
      value: 38.52051109616678
    - type: f1
      value: 37.07900132022834
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (sq)
      config: sq
      split: test
    metrics:
    - type: accuracy
      value: 41.62071284465367
    - type: f1
      value: 39.89522566274897
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (sv)
      config: sv
      split: test
    metrics:
    - type: accuracy
      value: 40.416946872898464
    - type: f1
      value: 38.43895125974106
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (sw)
      config: sw
      split: test
    metrics:
    - type: accuracy
      value: 35.27908540685945
    - type: f1
      value: 33.8079098469717
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (ta)
      config: ta
      split: test
    metrics:
    - type: accuracy
      value: 13.096839273705447
    - type: f1
      value: 10.24267220963294
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (te)
      config: te
      split: test
    metrics:
    - type: accuracy
      value: 2.5622057834566236
    - type: f1
      value: 1.0615210594147622
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (th)
      config: th
      split: test
    metrics:
    - type: accuracy
      value: 10.537995965030262
    - type: f1
      value: 6.1708791409070995
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (tl)
      config: tl
      split: test
    metrics:
    - type: accuracy
      value: 38.56086079354405
    - type: f1
      value: 35.015690080151465
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (tr)
      config: tr
      split: test
    metrics:
    - type: accuracy
      value: 35.897780766644246
    - type: f1
      value: 33.90602650751521
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (ur)
      config: ur
      split: test
    metrics:
    - type: accuracy
      value: 16.1768661735037
    - type: f1
      value: 15.713925259255651
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (vi)
      config: vi
      split: test
    metrics:
    - type: accuracy
      value: 37.37726967047747
    - type: f1
      value: 35.652051460172906
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (zh-CN)
      config: zh-CN
      split: test
    metrics:
    - type: accuracy
      value: 23.74243443174176
    - type: f1
      value: 19.255371431159425
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (zh-TW)
      config: zh-TW
      split: test
    metrics:
    - type: accuracy
      value: 22.387357094821787
    - type: f1
      value: 19.094067620374382
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (af)
      config: af
      split: test
    metrics:
    - type: accuracy
      value: 45.709482178883654
    - type: f1
      value: 43.61228850391169
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (am)
      config: am
      split: test
    metrics:
    - type: accuracy
      value: 7.407531943510423
    - type: f1
      value: 3.8875366763112984
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (ar)
      config: ar
      split: test
    metrics:
    - type: accuracy
      value: 27.61936785474109
    - type: f1
      value: 25.329931057423753
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (az)
      config: az
      split: test
    metrics:
    - type: accuracy
      value: 39.57969065232011
    - type: f1
      value: 37.39258432617311
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (bn)
      config: bn
      split: test
    metrics:
    - type: accuracy
      value: 18.9778076664425
    - type: f1
      value: 17.620144033142864
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (cy)
      config: cy
      split: test
    metrics:
    - type: accuracy
      value: 41.40215198386012
    - type: f1
      value: 38.06372767307641
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (da)
      config: da
      split: test
    metrics:
    - type: accuracy
      value: 49.46872898453262
    - type: f1
      value: 46.90610579296604
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (de)
      config: de
      split: test
    metrics:
    - type: accuracy
      value: 52.07128446536652
    - type: f1
      value: 49.46913533778989
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (el)
      config: el
      split: test
    metrics:
    - type: accuracy
      value: 35.50773369199731
    - type: f1
      value: 31.66524248503607
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (en)
      config: en
      split: test
    metrics:
    - type: accuracy
      value: 74.57632817753867
    - type: f1
      value: 73.95638454943459
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (es)
      config: es
      split: test
    metrics:
    - type: accuracy
      value: 50.743106926698054
    - type: f1
      value: 48.200939058933415
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (fa)
      config: fa
      split: test
    metrics:
    - type: accuracy
      value: 29.004707464694015
    - type: f1
      value: 25.784529950699753
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (fi)
      config: fi
      split: test
    metrics:
    - type: accuracy
      value: 45.80026899798252
    - type: f1
      value: 41.79459465764992
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (fr)
      config: fr
      split: test
    metrics:
    - type: accuracy
      value: 53.7626092804304
    - type: f1
      value: 51.70423088264189
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (he)
      config: he
      split: test
    metrics:
    - type: accuracy
      value: 25.682582380632148
    - type: f1
      value: 23.16790314457902
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (hi)
      config: hi
      split: test
    metrics:
    - type: accuracy
      value: 23.022864828513782
    - type: f1
      value: 21.459384490296486
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (hu)
      config: hu
      split: test
    metrics:
    - type: accuracy
      value: 44.08540685944856
    - type: f1
      value: 40.99340260145573
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (hy)
      config: hy
      split: test
    metrics:
    - type: accuracy
      value: 14.83187626092804
    - type: f1
      value: 12.970096153546534
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (id)
      config: id
      split: test
    metrics:
    - type: accuracy
      value: 44.34767989240081
    - type: f1
      value: 42.21539278376439
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (is)
      config: is
      split: test
    metrics:
    - type: accuracy
      value: 43.08002689979825
    - type: f1
      value: 40.01184510787284
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (it)
      config: it
      split: test
    metrics:
    - type: accuracy
      value: 51.71486213853396
    - type: f1
      value: 48.49232807960585
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (ja)
      config: ja
      split: test
    metrics:
    - type: accuracy
      value: 36.748486886348346
    - type: f1
      value: 35.46615048175051
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (jv)
      config: jv
      split: test
    metrics:
    - type: accuracy
      value: 44.56624075319435
    - type: f1
      value: 40.90741041356553
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (ka)
      config: ka
      split: test
    metrics:
    - type: accuracy
      value: 14.83523873570948
    - type: f1
      value: 12.296442463483718
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (km)
      config: km
      split: test
    metrics:
    - type: accuracy
      value: 9.754539340954944
    - type: f1
      value: 4.250353307219123
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (kn)
      config: kn
      split: test
    metrics:
    - type: accuracy
      value: 8.315400134498994
    - type: f1
      value: 5.388118548783403
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (ko)
      config: ko
      split: test
    metrics:
    - type: accuracy
      value: 25.719569603227978
    - type: f1
      value: 23.20523005165416
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (lv)
      config: lv
      split: test
    metrics:
    - type: accuracy
      value: 42.74714189643578
    - type: f1
      value: 40.61202626722604
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (ml)
      config: ml
      split: test
    metrics:
    - type: accuracy
      value: 7.252858103564222
    - type: f1
      value: 3.448646759763805
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (mn)
      config: mn
      split: test
    metrics:
    - type: accuracy
      value: 29.034969737726968
    - type: f1
      value: 26.63495414552696
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (ms)
      config: ms
      split: test
    metrics:
    - type: accuracy
      value: 44.64694014794889
    - type: f1
      value: 40.192107405242155
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (my)
      config: my
      split: test
    metrics:
    - type: accuracy
      value: 10.067249495628783
    - type: f1
      value: 5.764723442216905
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (nb)
      config: nb
      split: test
    metrics:
    - type: accuracy
      value: 47.357094821788834
    - type: f1
      value: 44.596914417443266
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (nl)
      config: nl
      split: test
    metrics:
    - type: accuracy
      value: 49.15265635507734
    - type: f1
      value: 46.15820727175712
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (pl)
      config: pl
      split: test
    metrics:
    - type: accuracy
      value: 44.72091459314056
    - type: f1
      value: 42.88213581673335
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (pt)
      config: pt
      split: test
    metrics:
    - type: accuracy
      value: 52.99932750504372
    - type: f1
      value: 51.01176637403334
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (ro)
      config: ro
      split: test
    metrics:
    - type: accuracy
      value: 49.97310020174849
    - type: f1
      value: 47.22673671303613
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (ru)
      config: ru
      split: test
    metrics:
    - type: accuracy
      value: 28.74915938130464
    - type: f1
      value: 27.25888866616121
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (sl)
      config: sl
      split: test
    metrics:
    - type: accuracy
      value: 42.2595830531271
    - type: f1
      value: 41.261927156734785
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (sq)
      config: sq
      split: test
    metrics:
    - type: accuracy
      value: 49.13584398117014
    - type: f1
      value: 47.08320600523055
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (sv)
      config: sv
      split: test
    metrics:
    - type: accuracy
      value: 46.82582380632145
    - type: f1
      value: 43.40423470084757
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (sw)
      config: sw
      split: test
    metrics:
    - type: accuracy
      value: 43.18426361802287
    - type: f1
      value: 39.815480841992084
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (ta)
      config: ta
      split: test
    metrics:
    - type: accuracy
      value: 19.3813046402152
    - type: f1
      value: 16.699966519668614
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (te)
      config: te
      split: test
    metrics:
    - type: accuracy
      value: 7.737054472091459
    - type: f1
      value: 3.8594459698077364
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (th)
      config: th
      split: test
    metrics:
    - type: accuracy
      value: 18.31540013449899
    - type: f1
      value: 13.491482848005418
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (tl)
      config: tl
      split: test
    metrics:
    - type: accuracy
      value: 48.305312710154666
    - type: f1
      value: 45.48790821413181
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (tr)
      config: tr
      split: test
    metrics:
    - type: accuracy
      value: 41.792199058507066
    - type: f1
      value: 41.24552662271258
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (ur)
      config: ur
      split: test
    metrics:
    - type: accuracy
      value: 24.462004034969738
    - type: f1
      value: 22.270575649981797
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (vi)
      config: vi
      split: test
    metrics:
    - type: accuracy
      value: 40.94149293880296
    - type: f1
      value: 39.08540872012287
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (zh-CN)
      config: zh-CN
      split: test
    metrics:
    - type: accuracy
      value: 33.17753866845998
    - type: f1
      value: 31.64001182395128
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (zh-TW)
      config: zh-TW
      split: test
    metrics:
    - type: accuracy
      value: 31.15669132481506
    - type: f1
      value: 30.89137619124565
  - task:
      type: Clustering
    dataset:
      type: mteb/medrxiv-clustering-p2p
      name: MTEB MedrxivClusteringP2P
      config: default
      split: test
    metrics:
    - type: v_measure
      value: 34.24621118290122
  - task:
      type: Clustering
    dataset:
      type: mteb/medrxiv-clustering-s2s
      name: MTEB MedrxivClusteringS2S
      config: default
      split: test
    metrics:
    - type: v_measure
      value: 32.24202424478886
  - task:
      type: Reranking
    dataset:
      type: mteb/mind_small
      name: MTEB MindSmallReranking
      config: default
      split: test
    metrics:
    - type: map
      value: 31.024522945679166
    - type: mrr
      value: 32.018722362966635
  - task:
      type: Retrieval
    dataset:
      type: nfcorpus
      name: MTEB NFCorpus
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 5.156000000000001
    - type: map_at_10
      value: 11.551
    - type: map_at_100
      value: 14.938
    - type: map_at_1000
      value: 16.366
    - type: map_at_3
      value: 8.118
    - type: map_at_5
      value: 9.918000000000001
    - type: mrr_at_1
      value: 42.415000000000006
    - type: mrr_at_10
      value: 51.571999999999996
    - type: mrr_at_100
      value: 52.126
    - type: mrr_at_1000
      value: 52.171
    - type: mrr_at_3
      value: 49.02
    - type: mrr_at_5
      value: 50.50599999999999
    - type: ndcg_at_1
      value: 39.783
    - type: ndcg_at_10
      value: 32.25
    - type: ndcg_at_100
      value: 30.089
    - type: ndcg_at_1000
      value: 38.86
    - type: ndcg_at_3
      value: 36.962
    - type: ndcg_at_5
      value: 35.292
    - type: precision_at_1
      value: 41.796
    - type: precision_at_10
      value: 24.272
    - type: precision_at_100
      value: 7.963000000000001
    - type: precision_at_1000
      value: 2.07
    - type: precision_at_3
      value: 35.397
    - type: precision_at_5
      value: 31.022
    - type: recall_at_1
      value: 5.156000000000001
    - type: recall_at_10
      value: 15.468000000000002
    - type: recall_at_100
      value: 31.049
    - type: recall_at_1000
      value: 63.148
    - type: recall_at_3
      value: 9.078999999999999
    - type: recall_at_5
      value: 12.275
  - task:
      type: Retrieval
    dataset:
      type: nq
      name: MTEB NQ
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 23.672
    - type: map_at_10
      value: 38.452
    - type: map_at_100
      value: 39.705
    - type: map_at_1000
      value: 39.742
    - type: map_at_3
      value: 33.806999999999995
    - type: map_at_5
      value: 36.576
    - type: mrr_at_1
      value: 26.854
    - type: mrr_at_10
      value: 40.822
    - type: mrr_at_100
      value: 41.801
    - type: mrr_at_1000
      value: 41.827999999999996
    - type: mrr_at_3
      value: 36.824
    - type: mrr_at_5
      value: 39.312000000000005
    - type: ndcg_at_1
      value: 26.854
    - type: ndcg_at_10
      value: 46.469
    - type: ndcg_at_100
      value: 51.756
    - type: ndcg_at_1000
      value: 52.601
    - type: ndcg_at_3
      value: 37.623
    - type: ndcg_at_5
      value: 42.324
    - type: precision_at_1
      value: 26.854
    - type: precision_at_10
      value: 8.189
    - type: precision_at_100
      value: 1.11
    - type: precision_at_1000
      value: 0.11900000000000001
    - type: precision_at_3
      value: 17.718999999999998
    - type: precision_at_5
      value: 13.291
    - type: recall_at_1
      value: 23.672
    - type: recall_at_10
      value: 68.639
    - type: recall_at_100
      value: 91.546
    - type: recall_at_1000
      value: 97.794
    - type: recall_at_3
      value: 45.643
    - type: recall_at_5
      value: 56.523
  - task:
      type: Retrieval
    dataset:
      type: quora
      name: MTEB QuoraRetrieval
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 69.667
    - type: map_at_10
      value: 83.83500000000001
    - type: map_at_100
      value: 84.479
    - type: map_at_1000
      value: 84.494
    - type: map_at_3
      value: 80.759
    - type: map_at_5
      value: 82.657
    - type: mrr_at_1
      value: 80.46
    - type: mrr_at_10
      value: 86.83800000000001
    - type: mrr_at_100
      value: 86.944
    - type: mrr_at_1000
      value: 86.945
    - type: mrr_at_3
      value: 85.815
    - type: mrr_at_5
      value: 86.508
    - type: ndcg_at_1
      value: 80.46
    - type: ndcg_at_10
      value: 87.752
    - type: ndcg_at_100
      value: 88.973
    - type: ndcg_at_1000
      value: 89.072
    - type: ndcg_at_3
      value: 84.735
    - type: ndcg_at_5
      value: 86.371
    - type: precision_at_1
      value: 80.46
    - type: precision_at_10
      value: 13.452
    - type: precision_at_100
      value: 1.532
    - type: precision_at_1000
      value: 0.157
    - type: precision_at_3
      value: 37.187
    - type: precision_at_5
      value: 24.5
    - type: recall_at_1
      value: 69.667
    - type: recall_at_10
      value: 95.329
    - type: recall_at_100
      value: 99.52
    - type: recall_at_1000
      value: 99.991
    - type: recall_at_3
      value: 86.696
    - type: recall_at_5
      value: 91.346
  - task:
      type: Clustering
    dataset:
      type: mteb/reddit-clustering
      name: MTEB RedditClustering
      config: default
      split: test
    metrics:
    - type: v_measure
      value: 51.177545122684634
  - task:
      type: Clustering
    dataset:
      type: mteb/reddit-clustering-p2p
      name: MTEB RedditClusteringP2P
      config: default
      split: test
    metrics:
    - type: v_measure
      value: 54.804652123126985
  - task:
      type: Retrieval
    dataset:
      type: scidocs
      name: MTEB SCIDOCS
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 5.162
    - type: map_at_10
      value: 13.168
    - type: map_at_100
      value: 15.766
    - type: map_at_1000
      value: 16.136
    - type: map_at_3
      value: 9.180000000000001
    - type: map_at_5
      value: 11.205
    - type: mrr_at_1
      value: 25.5
    - type: mrr_at_10
      value: 36.617
    - type: mrr_at_100
      value: 37.814
    - type: mrr_at_1000
      value: 37.86
    - type: mrr_at_3
      value: 33.15
    - type: mrr_at_5
      value: 35.29
    - type: ndcg_at_1
      value: 25.5
    - type: ndcg_at_10
      value: 21.818
    - type: ndcg_at_100
      value: 31.302999999999997
    - type: ndcg_at_1000
      value: 37.175000000000004
    - type: ndcg_at_3
      value: 20.358999999999998
    - type: ndcg_at_5
      value: 18.169
    - type: precision_at_1
      value: 25.5
    - type: precision_at_10
      value: 11.32
    - type: precision_at_100
      value: 2.495
    - type: precision_at_1000
      value: 0.38899999999999996
    - type: precision_at_3
      value: 18.833
    - type: precision_at_5
      value: 16.06
    - type: recall_at_1
      value: 5.162
    - type: recall_at_10
      value: 22.932
    - type: recall_at_100
      value: 50.598
    - type: recall_at_1000
      value: 79.053
    - type: recall_at_3
      value: 11.442
    - type: recall_at_5
      value: 16.272000000000002
  - task:
      type: STS
    dataset:
      type: mteb/sickr-sts
      name: MTEB SICK-R
      config: default
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 84.73414727754201
    - type: cos_sim_spearman
      value: 79.3180820145488
    - type: euclidean_pearson
      value: 81.33251162244008
    - type: euclidean_spearman
      value: 79.31808410123591
    - type: manhattan_pearson
      value: 81.24535628962194
    - type: manhattan_spearman
      value: 79.18643136990889
  - task:
      type: STS
    dataset:
      type: mteb/sts12-sts
      name: MTEB STS12
      config: default
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 82.89241604274538
    - type: cos_sim_spearman
      value: 73.08329002776462
    - type: euclidean_pearson
      value: 78.75856902522398
    - type: euclidean_spearman
      value: 73.0808569122323
    - type: manhattan_pearson
      value: 78.81165127939924
    - type: manhattan_spearman
      value: 73.13358160467396
  - task:
      type: STS
    dataset:
      type: mteb/sts13-sts
      name: MTEB STS13
      config: default
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 81.65439991719452
    - type: cos_sim_spearman
      value: 82.13398891011764
    - type: euclidean_pearson
      value: 81.63807492339613
    - type: euclidean_spearman
      value: 82.13398891011764
    - type: manhattan_pearson
      value: 81.5983078333819
    - type: manhattan_spearman
      value: 82.11893098949203
  - task:
      type: STS
    dataset:
      type: mteb/sts14-sts
      name: MTEB STS14
      config: default
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 81.66945263546415
    - type: cos_sim_spearman
      value: 76.7342099954029
    - type: euclidean_pearson
      value: 79.98454905286438
    - type: euclidean_spearman
      value: 76.73420731947648
    - type: manhattan_pearson
      value: 79.98121513026915
    - type: manhattan_spearman
      value: 76.74818574618494
  - task:
      type: STS
    dataset:
      type: mteb/sts15-sts
      name: MTEB STS15
      config: default
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 84.80085528616004
    - type: cos_sim_spearman
      value: 85.57752600637704
    - type: euclidean_pearson
      value: 84.88803602633503
    - type: euclidean_spearman
      value: 85.57753174543699
    - type: manhattan_pearson
      value: 84.77107707460819
    - type: manhattan_spearman
      value: 85.4531691739887
  - task:
      type: STS
    dataset:
      type: mteb/sts16-sts
      name: MTEB STS16
      config: default
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 79.32666585707851
    - type: cos_sim_spearman
      value: 80.22692417222228
    - type: euclidean_pearson
      value: 79.847799005588
    - type: euclidean_spearman
      value: 80.22692417222228
    - type: manhattan_pearson
      value: 79.86640649752613
    - type: manhattan_spearman
      value: 80.25939898948658
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (ko-ko)
      config: ko-ko
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 36.97351108396674
    - type: cos_sim_spearman
      value: 43.373159642451846
    - type: euclidean_pearson
      value: 42.343251342924724
    - type: euclidean_spearman
      value: 43.37383732365708
    - type: manhattan_pearson
      value: 42.21420013714062
    - type: manhattan_spearman
      value: 43.27093471564943
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (ar-ar)
      config: ar-ar
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 54.25766812232355
    - type: cos_sim_spearman
      value: 58.70907752953121
    - type: euclidean_pearson
      value: 57.74925638384565
    - type: euclidean_spearman
      value: 58.70907752953121
    - type: manhattan_pearson
      value: 57.53107164585081
    - type: manhattan_spearman
      value: 58.18399071690873
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (en-ar)
      config: en-ar
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 2.000902150291317
    - type: cos_sim_spearman
      value: 0.5442319876381565
    - type: euclidean_pearson
      value: 2.0061692624223886
    - type: euclidean_spearman
      value: 0.5442319876381565
    - type: manhattan_pearson
      value: 1.6005243901065973
    - type: manhattan_spearman
      value: 0.8261501538578374
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (en-de)
      config: en-de
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 31.103076250241756
    - type: cos_sim_spearman
      value: 27.538399556865983
    - type: euclidean_pearson
      value: 31.299966953719917
    - type: euclidean_spearman
      value: 27.538399556865983
    - type: manhattan_pearson
      value: 29.252983940152795
    - type: manhattan_spearman
      value: 24.545142053308506
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (en-en)
      config: en-en
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 88.92662843843466
    - type: cos_sim_spearman
      value: 88.6282754793921
    - type: euclidean_pearson
      value: 88.9663425476392
    - type: euclidean_spearman
      value: 88.6282754793921
    - type: manhattan_pearson
      value: 89.04213757202741
    - type: manhattan_spearman
      value: 88.8029452722001
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (en-tr)
      config: en-tr
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 6.699439791440673
    - type: cos_sim_spearman
      value: 0.42741621491041054
    - type: euclidean_pearson
      value: 7.0939749740816485
    - type: euclidean_spearman
      value: 0.42741621491041054
    - type: manhattan_pearson
      value: 3.7604205840813005
    - type: manhattan_spearman
      value: -1.7995925853478083
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (es-en)
      config: es-en
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 22.332768127048812
    - type: cos_sim_spearman
      value: 22.011862055263386
    - type: euclidean_pearson
      value: 22.275743114886957
    - type: euclidean_spearman
      value: 22.011862055263386
    - type: manhattan_pearson
      value: 21.382471306976754
    - type: manhattan_spearman
      value: 20.5220742340821
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (es-es)
      config: es-es
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 78.59529102081041
    - type: cos_sim_spearman
      value: 78.36515013988296
    - type: euclidean_pearson
      value: 79.6578967101581
    - type: euclidean_spearman
      value: 78.36388790924713
    - type: manhattan_pearson
      value: 79.54080618487365
    - type: manhattan_spearman
      value: 78.03366107978795
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (fr-en)
      config: fr-en
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 34.19498070710533
    - type: cos_sim_spearman
      value: 30.702559767030923
    - type: euclidean_pearson
      value: 34.28061977250095
    - type: euclidean_spearman
      value: 30.702559767030923
    - type: manhattan_pearson
      value: 34.8122111793038
    - type: manhattan_spearman
      value: 31.40796587790667
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (it-en)
      config: it-en
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 25.84186641167081
    - type: cos_sim_spearman
      value: 24.28452119168039
    - type: euclidean_pearson
      value: 25.866557000478302
    - type: euclidean_spearman
      value: 24.28452119168039
    - type: manhattan_pearson
      value: 24.273876016721925
    - type: manhattan_spearman
      value: 23.66844883927423
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (nl-en)
      config: nl-en
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 31.68262883322153
    - type: cos_sim_spearman
      value: 24.508086225784982
    - type: euclidean_pearson
      value: 32.07775246994894
    - type: euclidean_spearman
      value: 24.508086225784982
    - type: manhattan_pearson
      value: 33.20196765495327
    - type: manhattan_spearman
      value: 27.383641505403627
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (en)
      config: en
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 66.82398288868168
    - type: cos_sim_spearman
      value: 65.6697261994716
    - type: euclidean_pearson
      value: 66.84746542331361
    - type: euclidean_spearman
      value: 65.6697261994716
    - type: manhattan_pearson
      value: 66.89947196080837
    - type: manhattan_spearman
      value: 65.61734245758937
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (de)
      config: de
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 18.956935297479266
    - type: cos_sim_spearman
      value: 22.525438836468805
    - type: euclidean_pearson
      value: 13.676185827963197
    - type: euclidean_spearman
      value: 22.525438836468805
    - type: manhattan_pearson
      value: 13.749488574260106
    - type: manhattan_spearman
      value: 22.49725541226794
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (es)
      config: es
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 43.159634114474954
    - type: cos_sim_spearman
      value: 43.97530387822291
    - type: euclidean_pearson
      value: 42.45018759035119
    - type: euclidean_spearman
      value: 43.97530387822291
    - type: manhattan_pearson
      value: 43.88212906018782
    - type: manhattan_spearman
      value: 44.2344991447187
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (pl)
      config: pl
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 2.9506287366804567
    - type: cos_sim_spearman
      value: 19.21860340477442
    - type: euclidean_pearson
      value: 6.306031200912426
    - type: euclidean_spearman
      value: 19.21860340477442
    - type: manhattan_pearson
      value: 5.968058806485322
    - type: manhattan_spearman
      value: 18.496966556101356
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (tr)
      config: tr
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 17.494702940326327
    - type: cos_sim_spearman
      value: 21.600665598855933
    - type: euclidean_pearson
      value: 19.949878763475876
    - type: euclidean_spearman
      value: 21.600665598855933
    - type: manhattan_pearson
      value: 20.562737979747386
    - type: manhattan_spearman
      value: 21.548415116687096
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (ar)
      config: ar
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 21.455304899947475
    - type: cos_sim_spearman
      value: 17.54247841644246
    - type: euclidean_pearson
      value: 19.954769470444862
    - type: euclidean_spearman
      value: 17.54247841644246
    - type: manhattan_pearson
      value: 20.491628523649304
    - type: manhattan_spearman
      value: 17.984509706975498
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (ru)
      config: ru
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 5.725870260172754
    - type: cos_sim_spearman
      value: 11.187514830423046
    - type: euclidean_pearson
      value: 5.917124931676964
    - type: euclidean_spearman
      value: 11.187514830423046
    - type: manhattan_pearson
      value: 6.374841892742465
    - type: manhattan_spearman
      value: 10.769670996439327
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (zh)
      config: zh
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 23.644675903928903
    - type: cos_sim_spearman
      value: 33.1476054705555
    - type: euclidean_pearson
      value: 27.486723401317015
    - type: euclidean_spearman
      value: 33.14559867176513
    - type: manhattan_pearson
      value: 28.905530853992335
    - type: manhattan_spearman
      value: 32.97179552695711
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (fr)
      config: fr
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 68.19096417445061
    - type: cos_sim_spearman
      value: 69.51402658537921
    - type: euclidean_pearson
      value: 65.89836450895854
    - type: euclidean_spearman
      value: 69.51402658537921
    - type: manhattan_pearson
      value: 65.95918282706997
    - type: manhattan_spearman
      value: 69.66631782067878
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (de-en)
      config: de-en
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 47.02727261965111
    - type: cos_sim_spearman
      value: 42.85739641224728
    - type: euclidean_pearson
      value: 47.55857919944314
    - type: euclidean_spearman
      value: 42.85739641224728
    - type: manhattan_pearson
      value: 50.24947623020984
    - type: manhattan_spearman
      value: 44.34581665268886
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (es-en)
      config: es-en
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 52.54253509229287
    - type: cos_sim_spearman
      value: 53.98864875959218
    - type: euclidean_pearson
      value: 52.771474843725464
    - type: euclidean_spearman
      value: 53.98864875959218
    - type: manhattan_pearson
      value: 53.39728391060008
    - type: manhattan_spearman
      value: 54.65413858996554
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (it)
      config: it
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 48.017241684543656
    - type: cos_sim_spearman
      value: 47.47536430344332
    - type: euclidean_pearson
      value: 46.94098755337956
    - type: euclidean_spearman
      value: 47.47536430344332
    - type: manhattan_pearson
      value: 47.27489495136295
    - type: manhattan_spearman
      value: 47.75408075281176
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (pl-en)
      config: pl-en
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 43.16723254329198
    - type: cos_sim_spearman
      value: 42.6695846628273
    - type: euclidean_pearson
      value: 43.37634781317223
    - type: euclidean_spearman
      value: 42.6695846628273
    - type: manhattan_pearson
      value: 46.43632735525556
    - type: manhattan_spearman
      value: 44.399080708250175
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (zh-en)
      config: zh-en
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 42.614472380988
    - type: cos_sim_spearman
      value: 44.386615916921755
    - type: euclidean_pearson
      value: 42.602921485579536
    - type: euclidean_spearman
      value: 44.386615916921755
    - type: manhattan_pearson
      value: 39.57742966805997
    - type: manhattan_spearman
      value: 41.12937281700849
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (es-it)
      config: es-it
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 41.19025498086497
    - type: cos_sim_spearman
      value: 40.70511339346037
    - type: euclidean_pearson
      value: 41.757361379987536
    - type: euclidean_spearman
      value: 40.70511339346037
    - type: manhattan_pearson
      value: 42.12654868854391
    - type: manhattan_spearman
      value: 40.16977290096036
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (de-fr)
      config: de-fr
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 42.58930629526249
    - type: cos_sim_spearman
      value: 43.51970789091437
    - type: euclidean_pearson
      value: 42.79780567751299
    - type: euclidean_spearman
      value: 43.51970789091437
    - type: manhattan_pearson
      value: 43.11190678703615
    - type: manhattan_spearman
      value: 43.921331076552214
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (de-pl)
      config: de-pl
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 9.14354524166508
    - type: cos_sim_spearman
      value: 1.632087485480262
    - type: euclidean_pearson
      value: 9.808059926397586
    - type: euclidean_spearman
      value: 1.632087485480262
    - type: manhattan_pearson
      value: 15.655877492684972
    - type: manhattan_spearman
      value: 9.084260532390138
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (fr-pl)
      config: fr-pl
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 16.116974803470246
    - type: cos_sim_spearman
      value: 16.903085094570333
    - type: euclidean_pearson
      value: 16.277560475636694
    - type: euclidean_spearman
      value: 16.903085094570333
    - type: manhattan_pearson
      value: 20.321632312194925
    - type: manhattan_spearman
      value: 28.17180849095055
  - task:
      type: STS
    dataset:
      type: mteb/stsbenchmark-sts
      name: MTEB STSBenchmark
      config: default
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 83.75945741541354
    - type: cos_sim_spearman
      value: 83.08944658809418
    - type: euclidean_pearson
      value: 83.5587988852494
    - type: euclidean_spearman
      value: 83.08938533093635
    - type: manhattan_pearson
      value: 83.56896467262781
    - type: manhattan_spearman
      value: 83.11516183577004
  - task:
      type: Reranking
    dataset:
      type: mteb/scidocs-reranking
      name: MTEB SciDocsRR
      config: default
      split: test
    metrics:
    - type: map
      value: 87.20127714147824
    - type: mrr
      value: 96.44415315983943
  - task:
      type: Retrieval
    dataset:
      type: scifact
      name: MTEB SciFact
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 47.483
    - type: map_at_10
      value: 57.18600000000001
    - type: map_at_100
      value: 57.863
    - type: map_at_1000
      value: 57.901
    - type: map_at_3
      value: 53.909
    - type: map_at_5
      value: 55.57299999999999
    - type: mrr_at_1
      value: 50.0
    - type: mrr_at_10
      value: 58.607
    - type: mrr_at_100
      value: 59.169000000000004
    - type: mrr_at_1000
      value: 59.207
    - type: mrr_at_3
      value: 56.056
    - type: mrr_at_5
      value: 57.422
    - type: ndcg_at_1
      value: 50.0
    - type: ndcg_at_10
      value: 62.639
    - type: ndcg_at_100
      value: 65.549
    - type: ndcg_at_1000
      value: 66.497
    - type: ndcg_at_3
      value: 56.602
    - type: ndcg_at_5
      value: 59.270999999999994
    - type: precision_at_1
      value: 50.0
    - type: precision_at_10
      value: 8.833
    - type: precision_at_100
      value: 1.0370000000000001
    - type: precision_at_1000
      value: 0.11100000000000002
    - type: precision_at_3
      value: 22.222
    - type: precision_at_5
      value: 15.0
    - type: recall_at_1
      value: 47.483
    - type: recall_at_10
      value: 78.233
    - type: recall_at_100
      value: 91.167
    - type: recall_at_1000
      value: 98.333
    - type: recall_at_3
      value: 61.956
    - type: recall_at_5
      value: 68.43900000000001
  - task:
      type: PairClassification
    dataset:
      type: mteb/sprintduplicatequestions-pairclassification
      name: MTEB SprintDuplicateQuestions
      config: default
      split: test
    metrics:
    - type: cos_sim_accuracy
      value: 99.72871287128713
    - type: cos_sim_ap
      value: 92.44554820122362
    - type: cos_sim_f1
      value: 85.89083419155509
    - type: cos_sim_precision
      value: 88.53503184713377
    - type: cos_sim_recall
      value: 83.39999999999999
    - type: dot_accuracy
      value: 99.72871287128713
    - type: dot_ap
      value: 92.44554820122363
    - type: dot_f1
      value: 85.89083419155509
    - type: dot_precision
      value: 88.53503184713377
    - type: dot_recall
      value: 83.39999999999999
    - type: euclidean_accuracy
      value: 99.72871287128713
    - type: euclidean_ap
      value: 92.44554820122362
    - type: euclidean_f1
      value: 85.89083419155509
    - type: euclidean_precision
      value: 88.53503184713377
    - type: euclidean_recall
      value: 83.39999999999999
    - type: manhattan_accuracy
      value: 99.73267326732673
    - type: manhattan_ap
      value: 92.57860510428624
    - type: manhattan_f1
      value: 86.20170597089813
    - type: manhattan_precision
      value: 86.5055387713998
    - type: manhattan_recall
      value: 85.9
    - type: max_accuracy
      value: 99.73267326732673
    - type: max_ap
      value: 92.57860510428624
    - type: max_f1
      value: 86.20170597089813
  - task:
      type: Clustering
    dataset:
      type: mteb/stackexchange-clustering
      name: MTEB StackExchangeClustering
      config: default
      split: test
    metrics:
    - type: v_measure
      value: 53.04887987709521
  - task:
      type: Clustering
    dataset:
      type: mteb/stackexchange-clustering-p2p
      name: MTEB StackExchangeClusteringP2P
      config: default
      split: test
    metrics:
    - type: v_measure
      value: 33.133116286225686
  - task:
      type: Reranking
    dataset:
      type: mteb/stackoverflowdupquestions-reranking
      name: MTEB StackOverflowDupQuestions
      config: default
      split: test
    metrics:
    - type: map
      value: 51.4732035634667
    - type: mrr
      value: 52.263880931160344
  - task:
      type: Summarization
    dataset:
      type: mteb/summeval
      name: MTEB SummEval
      config: default
      split: test
    metrics:
    - type: cos_sim_pearson
      value: 29.365093191497525
    - type: cos_sim_spearman
      value: 27.90160600683062
    - type: dot_pearson
      value: 29.36509564650472
    - type: dot_spearman
      value: 27.90160600683062
  - task:
      type: Retrieval
    dataset:
      type: trec-covid
      name: MTEB TRECCOVID
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 0.17600000000000002
    - type: map_at_10
      value: 1.164
    - type: map_at_100
      value: 6.048
    - type: map_at_1000
      value: 14.913000000000002
    - type: map_at_3
      value: 0.44799999999999995
    - type: map_at_5
      value: 0.658
    - type: mrr_at_1
      value: 64.0
    - type: mrr_at_10
      value: 73.538
    - type: mrr_at_100
      value: 73.752
    - type: mrr_at_1000
      value: 73.752
    - type: mrr_at_3
      value: 70.667
    - type: mrr_at_5
      value: 72.467
    - type: ndcg_at_1
      value: 59.0
    - type: ndcg_at_10
      value: 50.815999999999995
    - type: ndcg_at_100
      value: 37.662
    - type: ndcg_at_1000
      value: 35.907
    - type: ndcg_at_3
      value: 54.112
    - type: ndcg_at_5
      value: 51.19200000000001
    - type: precision_at_1
      value: 64.0
    - type: precision_at_10
      value: 55.400000000000006
    - type: precision_at_100
      value: 38.48
    - type: precision_at_1000
      value: 16.012
    - type: precision_at_3
      value: 57.99999999999999
    - type: precision_at_5
      value: 54.800000000000004
    - type: recall_at_1
      value: 0.17600000000000002
    - type: recall_at_10
      value: 1.435
    - type: recall_at_100
      value: 9.122
    - type: recall_at_1000
      value: 34.378
    - type: recall_at_3
      value: 0.47400000000000003
    - type: recall_at_5
      value: 0.736
  - task:
      type: Retrieval
    dataset:
      type: webis-touche2020
      name: MTEB Touche2020
      config: default
      split: test
    metrics:
    - type: map_at_1
      value: 1.813
    - type: map_at_10
      value: 6.632000000000001
    - type: map_at_100
      value: 11.485
    - type: map_at_1000
      value: 13.031
    - type: map_at_3
      value: 3.5069999999999997
    - type: map_at_5
      value: 5.183
    - type: mrr_at_1
      value: 18.367
    - type: mrr_at_10
      value: 33.035
    - type: mrr_at_100
      value: 34.117
    - type: mrr_at_1000
      value: 34.168
    - type: mrr_at_3
      value: 27.551
    - type: mrr_at_5
      value: 31.326999999999998
    - type: ndcg_at_1
      value: 15.306000000000001
    - type: ndcg_at_10
      value: 17.224
    - type: ndcg_at_100
      value: 29.287999999999997
    - type: ndcg_at_1000
      value: 41.613
    - type: ndcg_at_3
      value: 15.786
    - type: ndcg_at_5
      value: 16.985
    - type: precision_at_1
      value: 18.367
    - type: precision_at_10
      value: 15.714
    - type: precision_at_100
      value: 6.4079999999999995
    - type: precision_at_1000
      value: 1.451
    - type: precision_at_3
      value: 17.687
    - type: precision_at_5
      value: 18.776
    - type: recall_at_1
      value: 1.813
    - type: recall_at_10
      value: 12.006
    - type: recall_at_100
      value: 41.016999999999996
    - type: recall_at_1000
      value: 78.632
    - type: recall_at_3
      value: 4.476999999999999
    - type: recall_at_5
      value: 7.904999999999999
  - task:
      type: Classification
    dataset:
      type: mteb/toxic_conversations_50k
      name: MTEB ToxicConversationsClassification
      config: default
      split: test
    metrics:
    - type: accuracy
      value: 67.4694
    - type: ap
      value: 12.602604676283388
    - type: f1
      value: 51.82471949507483
  - task:
      type: Classification
    dataset:
      type: mteb/tweet_sentiment_extraction
      name: MTEB TweetSentimentExtractionClassification
      config: default
      split: test
    metrics:
    - type: accuracy
      value: 54.25297113752122
    - type: f1
      value: 54.50148311546008
  - task:
      type: Clustering
    dataset:
      type: mteb/twentynewsgroups-clustering
      name: MTEB TwentyNewsgroupsClustering
      config: default
      split: test
    metrics:
    - type: v_measure
      value: 47.467044776612376
  - task:
      type: PairClassification
    dataset:
      type: mteb/twittersemeval2015-pairclassification
      name: MTEB TwitterSemEval2015
      config: default
      split: test
    metrics:
    - type: cos_sim_accuracy
      value: 84.78869881385229
    - type: cos_sim_ap
      value: 70.01722500181003
    - type: cos_sim_f1
      value: 65.943384461903
    - type: cos_sim_precision
      value: 62.52069047056041
    - type: cos_sim_recall
      value: 69.76253298153034
    - type: dot_accuracy
      value: 84.78869881385229
    - type: dot_ap
      value: 70.01721947474665
    - type: dot_f1
      value: 65.943384461903
    - type: dot_precision
      value: 62.52069047056041
    - type: dot_recall
      value: 69.76253298153034
    - type: euclidean_accuracy
      value: 84.78869881385229
    - type: euclidean_ap
      value: 70.01721811552584
    - type: euclidean_f1
      value: 65.943384461903
    - type: euclidean_precision
      value: 62.52069047056041
    - type: euclidean_recall
      value: 69.76253298153034
    - type: manhattan_accuracy
      value: 84.68140907194373
    - type: manhattan_ap
      value: 69.90669388421887
    - type: manhattan_f1
      value: 66.00842865743527
    - type: manhattan_precision
      value: 60.70874861572536
    - type: manhattan_recall
      value: 72.32189973614776
    - type: max_accuracy
      value: 84.78869881385229
    - type: max_ap
      value: 70.01722500181003
    - type: max_f1
      value: 66.00842865743527
  - task:
      type: PairClassification
    dataset:
      type: mteb/twitterurlcorpus-pairclassification
      name: MTEB TwitterURLCorpus
      config: default
      split: test
    metrics:
    - type: cos_sim_accuracy
      value: 88.4367601971514
    - type: cos_sim_ap
      value: 84.77318195783158
    - type: cos_sim_f1
      value: 77.13502703503444
    - type: cos_sim_precision
      value: 74.31140288283146
    - type: cos_sim_recall
      value: 80.18170619032954
    - type: dot_accuracy
      value: 88.4367601971514
    - type: dot_ap
      value: 84.77317449778201
    - type: dot_f1
      value: 77.13502703503444
    - type: dot_precision
      value: 74.31140288283146
    - type: dot_recall
      value: 80.18170619032954
    - type: euclidean_accuracy
      value: 88.4367601971514
    - type: euclidean_ap
      value: 84.77314948093711
    - type: euclidean_f1
      value: 77.13502703503444
    - type: euclidean_precision
      value: 74.31140288283146
    - type: euclidean_recall
      value: 80.18170619032954
    - type: manhattan_accuracy
      value: 88.43287926417511
    - type: manhattan_ap
      value: 84.71097141640011
    - type: manhattan_f1
      value: 77.08356453223837
    - type: manhattan_precision
      value: 74.18298326806692
    - type: manhattan_recall
      value: 80.2202032645519
    - type: max_accuracy
      value: 88.4367601971514
    - type: max_ap
      value: 84.77318195783158
    - type: max_f1
      value: 77.13502703503444
---


# all-MiniLM-L12-v2
This is a [sentence-transformers](https://www.SBERT.net) model: It maps sentences & paragraphs to a 384 dimensional dense vector space and can be used for tasks like clustering or semantic search.

## Usage (Sentence-Transformers)
Using this model becomes easy when you have [sentence-transformers](https://www.SBERT.net) installed:

```
pip install -U sentence-transformers
```

Then you can use the model like this:
```python
from sentence_transformers import SentenceTransformer
sentences = ["This is an example sentence", "Each sentence is converted"]

model = SentenceTransformer('sentence-transformers/all-MiniLM-L12-v2')
embeddings = model.encode(sentences)
print(embeddings)
```

## Usage (HuggingFace Transformers)
Without [sentence-transformers](https://www.SBERT.net), you can use the model like this: First, you pass your input through the transformer model, then you have to apply the right pooling-operation on-top of the contextualized word embeddings.

```python
from transformers import AutoTokenizer, AutoModel
import torch
import torch.nn.functional as F

#Mean Pooling - Take attention mask into account for correct averaging
def mean_pooling(model_output, attention_mask):
    token_embeddings = model_output[0] #First element of model_output contains all token embeddings
    input_mask_expanded = attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
    return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(input_mask_expanded.sum(1), min=1e-9)


# Sentences we want sentence embeddings for
sentences = ['This is an example sentence', 'Each sentence is converted']

# Load model from HuggingFace Hub
tokenizer = AutoTokenizer.from_pretrained('sentence-transformers/all-MiniLM-L12-v2')
model = AutoModel.from_pretrained('sentence-transformers/all-MiniLM-L12-v2')

# Tokenize sentences
encoded_input = tokenizer(sentences, padding=True, truncation=True, return_tensors='pt')

# Compute token embeddings
with torch.no_grad():
    model_output = model(**encoded_input)

# Perform pooling
sentence_embeddings = mean_pooling(model_output, encoded_input['attention_mask'])

# Normalize embeddings
sentence_embeddings = F.normalize(sentence_embeddings, p=2, dim=1)

print("Sentence embeddings:")
print(sentence_embeddings)
```

## Evaluation Results

For an automated evaluation of this model, see the *Sentence Embeddings Benchmark*: [https://seb.sbert.net](https://seb.sbert.net?model_name=sentence-transformers/all-MiniLM-L12-v2)

------

## Background

The project aims to train sentence embedding models on very large sentence level datasets using a self-supervised 
contrastive learning objective. We used the pretrained [`microsoft/MiniLM-L12-H384-uncased`](https://huggingface.co/microsoft/MiniLM-L12-H384-uncased) model and fine-tuned in on a 
1B sentence pairs dataset. We use a contrastive learning objective: given a sentence from the pair, the model should predict which out of a set of randomly sampled other sentences, was actually paired with it in our dataset.

We developped this model during the 
[Community week using JAX/Flax for NLP & CV](https://discuss.huggingface.co/t/open-to-the-community-community-week-using-jax-flax-for-nlp-cv/7104), 
organized by Hugging Face. We developped this model as part of the project:
[Train the Best Sentence Embedding Model Ever with 1B Training Pairs](https://discuss.huggingface.co/t/train-the-best-sentence-embedding-model-ever-with-1b-training-pairs/7354). We benefited from efficient hardware infrastructure to run the project: 7 TPUs v3-8, as well as intervention from Googles Flax, JAX, and Cloud team member about efficient deep learning frameworks.

## Intended uses

Our model is intented to be used as a sentence and short paragraph encoder. Given an input text, it ouptuts a vector which captures 
the semantic information. The sentence vector may be used for information retrieval, clustering or sentence similarity tasks.

By default, input text longer than 256 word pieces is truncated.


## Training procedure

### Pre-training 

We use the pretrained [`microsoft/MiniLM-L12-H384-uncased`](https://huggingface.co/microsoft/MiniLM-L12-H384-uncased) model. Please refer to the model card for more detailed information about the pre-training procedure.

### Fine-tuning 

We fine-tune the model using a contrastive objective. Formally, we compute the cosine similarity from each possible sentence pairs from the batch.
We then apply the cross entropy loss by comparing with true pairs.

#### Hyper parameters

We trained ou model on a TPU v3-8. We train the model during 100k steps using a batch size of 1024 (128 per TPU core).
We use a learning rate warm up of 500. The sequence length was limited to 128 tokens. We used the AdamW optimizer with
a 2e-5 learning rate. The full training script is accessible in this current repository: `train_script.py`.

#### Training data

We use the concatenation from multiple datasets to fine-tune our model. The total number of sentence pairs is above 1 billion sentences.
We sampled each dataset given a weighted probability which configuration is detailed in the `data_config.json` file.


| Dataset                                                  | Paper                                    | Number of training tuples  |
|--------------------------------------------------------|:----------------------------------------:|:--------------------------:|
| [Reddit comments (2015-2018)](https://github.com/PolyAI-LDN/conversational-datasets/tree/master/reddit) | [paper](https://arxiv.org/abs/1904.06472) | 726,484,430 |
| [S2ORC](https://github.com/allenai/s2orc) Citation pairs (Abstracts) | [paper](https://aclanthology.org/2020.acl-main.447/) | 116,288,806 |
| [WikiAnswers](https://github.com/afader/oqa#wikianswers-corpus) Duplicate question pairs | [paper](https://doi.org/10.1145/2623330.2623677) | 77,427,422 |
| [PAQ](https://github.com/facebookresearch/PAQ) (Question, Answer) pairs | [paper](https://arxiv.org/abs/2102.07033) | 64,371,441 |
| [S2ORC](https://github.com/allenai/s2orc) Citation pairs (Titles) | [paper](https://aclanthology.org/2020.acl-main.447/) | 52,603,982 |
| [S2ORC](https://github.com/allenai/s2orc) (Title, Abstract) | [paper](https://aclanthology.org/2020.acl-main.447/) | 41,769,185 |
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) (Title, Body) pairs  | - | 25,316,456 |
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) (Title+Body, Answer) pairs  | - | 21,396,559 |
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) (Title, Answer) pairs  | - | 21,396,559 |
| [MS MARCO](https://microsoft.github.io/msmarco/) triplets | [paper](https://doi.org/10.1145/3404835.3462804) | 9,144,553 |
| [GOOAQ: Open Question Answering with Diverse Answer Types](https://github.com/allenai/gooaq) | [paper](https://arxiv.org/pdf/2104.08727.pdf) | 3,012,496 |
| [Yahoo Answers](https://www.kaggle.com/soumikrakshit/yahoo-answers-dataset) (Title, Answer) | [paper](https://proceedings.neurips.cc/paper/2015/hash/250cf8b51c773f3f8dc8b4be867a9a02-Abstract.html) | 1,198,260 |
| [Code Search](https://huggingface.co/datasets/code_search_net) | - | 1,151,414 |
| [COCO](https://cocodataset.org/#home) Image captions | [paper](https://link.springer.com/chapter/10.1007%2F978-3-319-10602-1_48) | 828,395|
| [SPECTER](https://github.com/allenai/specter) citation triplets | [paper](https://doi.org/10.18653/v1/2020.acl-main.207) | 684,100 |
| [Yahoo Answers](https://www.kaggle.com/soumikrakshit/yahoo-answers-dataset) (Question, Answer) | [paper](https://proceedings.neurips.cc/paper/2015/hash/250cf8b51c773f3f8dc8b4be867a9a02-Abstract.html) | 681,164 |
| [Yahoo Answers](https://www.kaggle.com/soumikrakshit/yahoo-answers-dataset) (Title, Question) | [paper](https://proceedings.neurips.cc/paper/2015/hash/250cf8b51c773f3f8dc8b4be867a9a02-Abstract.html) | 659,896 |
| [SearchQA](https://huggingface.co/datasets/search_qa) | [paper](https://arxiv.org/abs/1704.05179) | 582,261 |
| [Eli5](https://huggingface.co/datasets/eli5) | [paper](https://doi.org/10.18653/v1/p19-1346) | 325,475 |
| [Flickr 30k](https://shannon.cs.illinois.edu/DenotationGraph/) | [paper](https://transacl.org/ojs/index.php/tacl/article/view/229/33) | 317,695 |
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) Duplicate questions (titles) | | 304,525 |
| AllNLI ([SNLI](https://nlp.stanford.edu/projects/snli/) and [MultiNLI](https://cims.nyu.edu/~sbowman/multinli/) | [paper SNLI](https://doi.org/10.18653/v1/d15-1075), [paper MultiNLI](https://doi.org/10.18653/v1/n18-1101) | 277,230 | 
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) Duplicate questions (bodies) | | 250,519 |
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) Duplicate questions (titles+bodies) | | 250,460 |
| [Sentence Compression](https://github.com/google-research-datasets/sentence-compression) | [paper](https://www.aclweb.org/anthology/D13-1155/) | 180,000 |
| [Wikihow](https://github.com/pvl/wikihow_pairs_dataset) | [paper](https://arxiv.org/abs/1810.09305) | 128,542 |
| [Altlex](https://github.com/chridey/altlex/) | [paper](https://aclanthology.org/P16-1135.pdf) | 112,696 |
| [Quora Question Triplets](https://quoradata.quora.com/First-Quora-Dataset-Release-Question-Pairs) | - | 103,663 |
| [Simple Wikipedia](https://cs.pomona.edu/~dkauchak/simplification/) | [paper](https://www.aclweb.org/anthology/P11-2117/) | 102,225 |
| [Natural Questions (NQ)](https://ai.google.com/research/NaturalQuestions) | [paper](https://transacl.org/ojs/index.php/tacl/article/view/1455) | 100,231 |
| [SQuAD2.0](https://rajpurkar.github.io/SQuAD-explorer/) | [paper](https://aclanthology.org/P18-2124.pdf) | 87,599 |
| [TriviaQA](https://huggingface.co/datasets/trivia_qa) | - | 73,346 |
| **Total** | | **1,170,060,424** |