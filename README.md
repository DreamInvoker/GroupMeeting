# GroupMeeting

* [Tasks or Methods](#tasks-or-methods)
    * [Relation Extraction](#1-relation-extraction)
    * [Semantic Role Labeling](#2-semantic-role-labeling)
    * [Dependency Parsing](#3-dependency-parsing)
    * [Math Problem Generation](#4-math-problem-generation)
    * [Medical Text Processing](#5-medical-text-processing)
    * [Named Entity Recognition](#6-named-entity-recognition)
    * [Law Judgement Prediction](#7-law-judgement-prediction)
    * [Discourse Parsing](#8-discourse-parsing)
    * [Knowledge Distilling](#9-knowledge-distilling)
    * [Data Augmentation](#10-data-augmentation)
    * [Transformer](#11-transformer)
    * [Numerical Embedding](#12-numerical-embedding)
    * [Question Answering](#13-question-answering)
    * [Chinese Word Segmentation](#14-chinese-word-segmentation-and-semi-supervised-learning)
    * [Machine Translation](#15-machine-translation)
    * [Question Generation](#16-question-generation)
    * [Language Model](#17-language-model)
    * [Abstractive Summarization](#18-abstractive-summarization)
    * [Sequence Labeling](#19-sequence-labeling)

## Tasks or Methods
### 1. Relation Extraction
2020/02/23
reporter: Shuang Zeng
* paper: Fenia Christopoulou, Makoto Miwa, Sophia Ananiadou. 2019. [Connecting the Dots: Document-level Neural Relation Extraction with Edge-oriented Graphs](https://arxiv.org/abs/1909.00228). In *EMNLP-IJCNLP 2019*.
* ppt:  [20200223_zs](ppts/20200223_zs.pdf)
* method: BiLSTM + Edge-oriented Graph + Iterative Inference Mechanism

2020/03/08
reporter: Yuan Zong
* paper: Daojian Zeng, Haoran Zhang, Qianying Liu. 2020. [CopyMTL:Copy Mechanism for Joint Extraction of Entities and Relations with Multi-Task Learning](https://arxiv.org/abs/1911.10438). In *AAAI 2020*.
* ppt:  [20200308_zy](ppts/20200308_zy.pdf)
* method: Pointer-generator + mulit-task

2020/03/15
reporter: Runxin Xu
* paper: Zhepei Wei, Jianlin Su, Yue Wang, Yuan Tian, Yi Chang. 2019. [A Novel Hierarchical Binary Tagging Framework for Joint Extraction of Entities and Relations](https://arxiv.org/abs/1909.03227). In *arxiv preprint*.
* ppt:  [20200315_xrx](ppts/20200315_xrx.pdf)
* method: BERT + subject tagger + relation-specific object tagger

2020/03/22
reporter: Shuang Zeng
* paper: Bowen Yu, Zhenyu Zhang, Tingwen Liu, Bin Wang, Sujian Li, Quangang Li. 2019. [Beyond Word Attention: Using Segment Attention in Neural Relation Extraction](https://www.ijcai.org/Proceedings/2019/750). In *IJCAI 2019*.
* ppt:  [20200322_zs](ppts/20200322_zs.pdf)
* method: Segment Attention Layer with linear-chain CRF + two regularizers

2020/04/05
reporter: Yuan Zong
* paper: Christoph Alt, Marc Hübner, Leonhard Hennig. 2019. [Fine-tuning Pre-Trained Transformer Language Models to Distantly Supervised Relation Extraction](https://arxiv.org/abs/1906.08646). In *ACL 2019*.
* ppt:  [20200405_zy](ppts/20200405_zy.pdf)
* method: Pretrain_model + bag_level

2020/04/12
reporter: Shuang Zeng
* paper1: Xiaocheng Feng, Jiang Guo, Bing Qin, Ting Liu, Yongjie Liu. 2017. [Effective Deep Memory Networks for Distant Supervised Relation Extraction](https://www.ijcai.org/Proceedings/2017/559). In *IJCAI 2017*.
* method: PCNN + word-level memory + sentence-level memory, bag-level multi-instance multi-label learning
* paper2: Jianhao Yan, Lin He, Ruqin Huang, Jian Li, Ying Liu. 2019. [Relation Extraction with Temporal Reasoning Based on Memory Augmented Distant Supervision](https://www.aclweb.org/anthology/N19-1107). In *NAACL 2019*.
* method: PCNN + temporal memory + iterative reasoning
* ppt:  [20200412_zs](ppts/20200412_zs.pdf)

2020/04/20
reporter: Xudong Chen
* paper: Yang Li, Guodong Long, Tao Shen, Tianyi Zhou, Lina Yao, Huan Huo, Jing Jiang.2020. [Self-Attention Enhanced Selective Gate with Entity-Aware Embedding for Distantly Supervised Relation Extraction](https://arxiv.org/abs/1911.11899?context=cs). In *AAAI 2020*.
* ppt:  [20200420_cxd](ppts/20200420_cxd.pdf)
* method: Attention+Gate+Entity-Aware Embedding

2020/04/20
reporter: Runxin Xu
* paper1: Livio Baldini Soares, Nicholas FitzGerald, Jeffrey Ling, Tom Kwiatkowski.2019. [Matching the Blanks: Distributional Similarity for Relation Learning](https://arxiv.org/abs/1906.03158). In *ACL 2019*.
* paper2: Weijie Liu, Peng Zhou, Zhe Zhao, Zhiruo Wang, Qi Ju, Haotang Deng, Ping Wang.2020. [K-BERT: Enabling Language Representation with Knowledge Graph](https://arxiv.org/abs/1909.07606). In *AAAI 2020*.
* ppt:  [20200420_xrx](ppts/20200420_xrx.pdf)
* method: Pre-train Model & Knowledge Graph

2020/05/03
reporter: Yuan Zong
* paper: Wenya Wang, Sinno Jialin Pan. 2020. [Integrating Deep Learning with Logic Fusion for Information Extraction](https://arxiv.org/abs/1912.03041). In *AAAI 2020*.
* ppt:  [20200503_zy](ppts/20200503_zy.pdf)
* method: Transformer & Logic Fusion

2020/05/17
reporter: Shuang Zeng
* paper: Kai Sun, Richong Zhang, Samuel Mensah, Yongyi Mao, Xudong Liu. 2020. [Recurrent Interaction Network for Jointly Extracting Entities and Classifying Relations](https://arxiv.org/abs/2005.00162). In *Arxiv Preprint*.
* ppt:  [20200517_zs](ppts/20200517_zs.pdf)
* method: Recurrent Interaction Network

2020/06/14
reporter: Shuang Zeng
* paper: Guoshun Nan, Zhijiang Guo, Ivan Sekulić, Wei Lu. 2020. [Reasoning with Latent Structure Refinement for Document-Level Relation Extraction](https://arxiv.org/abs/2005.06312). In *ACL 2020*.
* ppt:  [20200614_zs](ppts/20200614_zs.pdf)
* method: Node Constructor + Structure Attention based Sturcture Induction + Multi-hop Reasoning

2020/07/18
reporter: Runxin Xu
* paper: Pengcheng Yin, Graham Neubig, Wen-tau Yih, Sebastian Riedel. 2020. [TaBERT: Pretraining for Joint Understanding of Textual and Tabular Data](https://arxiv.org/abs/2005.08314). In *ACL 2020*.
* ppt:  [20200718_xrx](ppts/20200719_xrx.pdf)
* method: Pretraining for Table Data

2020/07/26
reporter: Xudong Chen
* paper: Pengcheng Yin, Graham Neubig, Wen-tau Yih, Sebastian Riedel. 2020. [A Joint Neural Model for Information Extraction with Global Features](https://www.aclweb.org/anthology/2020.acl-main.713.pdf). In *ACL 2020*.
* ppt:  [20200726_cxd](ppts/20200726_cxd.pdf)
* method: Muti-task+Global Features


2020/08/02
reporter: Shuang Zeng
* paper1: Marco Tulio Ribeiro, Tongshuang Wu, Carlos Guestrin, Sameer Singh. 2020. [Beyond Accuracy: Behavioral Testing of NLP Models with CheckList](https://www.aclweb.org/anthology/2020.acl-main.442/). In *ACL 2020*.
* method: CheckList for generalization in NLP models
* paper2: Suchin Gururangan, Ana Marasović, Swabha Swayamdipta, Kyle Lo, Iz Beltagy, Doug Downey, Noah A. Smith. 2020. [Don’t Stop Pretraining: Adapt Language Models to Domains and Tasks](https://www.aclweb.org/anthology/2020.acl-main.740/). In *ACL 2020*.
* method: Multi-phase Adaptive Pre-training on domains and tasks
* paper3: Yi Luan, Luheng He, Mari Ostendorf, Hannaneh Hajishirzi. 2018. [Multi-Task Identification of Entities, Relations, and Coreference for Scientific Knowledge Graph Construction](https://www.aclweb.org/anthology/D18-1360/). In *EMNLP 2018*.
* method: Mutil-task setup for NER + CR + RE
* paper4: Cheng Li, Ye Tian. 2020. [Downstream Model Design of Pre-trained Language Model for Relation Extraction Task](https://arxiv.org/abs/2004.03786). In *Arxiv Preprint*.
* method: Downstream design for RE using bert
* paper5: Takashi Ishida, Ikko Yamane, Tomoya Sakai, Gang Niu, Masashi Sugiyama. 2020. [Do We Need Zero Training Loss After Achieving Zero Training Error?](https://arxiv.org/abs/2002.08709). In *ICML 2020*.
* method: Flooding loss for double decent on test loss
* ppt:  [20200802_zs_xrx](ppts/20200802_zs.pdf)

2020/08/16
reporter: Xudong Chen
* paper: Bowen Yu, Zhenyu Zhang, Xiaobo Shu, Yubin Wang, Tingwen Liu, Bin Wang, Sujian Li. 2019. [Joint Extraction of Entities and Relations Based on a Novel Decomposition Strategy](https://arxiv.org/abs/1909.04273v3).
* ppt:  [20200815_cxd](ppts/20200815_cxd.pdf)
* method: HBT+Decomposition Strategy

2020/08/30
reporter: Shuang Zeng
* paper: Sarthak Jain, Madeleine van Zuylen, Hannaneh Hajishirzi, Iz Beltagy. 2020. [SciREX: A Challenge Dataset for Document-Level Information Extraction](https://www.aclweb.org/anthology/2020.acl-main.670/). In *ACL 2020*.
* ppt:  [20200830_zs](ppts/20200830_zs.pdf)
* method: Largest Document-level Relation Extraction Dataset, which is in the domain of Science

2020/10/31
reporter: Jiaxing Lin
* paper1: Difeng Wang, Wei Hu, Ermei Cao, Weijian Sun. 2020. [Global-to-Local Neural Networks for Document-Level Relation Extraction](https://arxiv.org/abs/2009.10359). In *EMNLP 2020*
* method: BERT+R-GCN for global rep, MultiHeadAttention for local rep and self-attention for topic rep
* paper2: Wenxuan Zhou, Kevin Huang, Tengyu Ma, Jing Huang. 2020. [Document-Level Relation Extraction with Adaptive Thresholding and Localized Context Pooling](https://arxiv.org/abs/2010.11304). In *ArXiv 2020*
* method: BERT, localized context pooling by using the last transformer layer in BERT, adaptive thresholding and adaptive thresholding loss
* ppt: [20201031_ljx](ppts/20201031_ljx.pdf)


2020/11/14
reporter: Shuang Zeng
* paper1: Hao Peng, Tianyu Gao, Xu Han, Yankai Lin, Peng Li, Zhiyuan Liu, Maosong Sun, Jie Zhou. 2020. [Learning from Context or Names? An Empirical Study on Neural Relation Extraction](https://www.aclweb.org/anthology/2020.emnlp-main.298/). In *EMNLP 2020*.
* method: Contrastive Pre-training for RE + Random Mask Entity
* paper2: Amir DN Cohen, Shachar Rosenman, Yoav Goldberg. 2020. [Relation Extraction as Two-way Span-Prediction](https://arxiv.org/abs/2010.04829). In *ArXiv 2020*.
* method: Reduce Relation Classification task to Question Answering Task with bidirectional question for each relation
* ppt:  [20201114_zs](ppts/20201114_zs.pdf)

2020/12/12
reporter: Jiaxing Lin
* paper1: Jue Wang, Wei Lu. 2020. [Two are Better than One: Joint Entity and Relation Extraction tiwh Table-Sequence Encoders](https://www.aclweb.org/anthology/2020.emnlp-main.133/). In *EMNLP 2020*
* method: Table-filling, table encoder and sequence encoder interact with each other
* paper2: Bin Ji, Jie Yu, Shasha Li, Jun Ma, Qingbo Wu, Yusong Tan, Huijun Liu. 2020. [Span-based Joint Entity and Relation Extraction with Attention-based Span-specific and Contextual Semantic Representations](https://www.aclweb.org/anthology/2020.coling-main.8/). In *COLING 2020*
* method: NER: SpanSpecific representation and sentence-level contextual representation; RE: local representation and sentence-level contextual representation.
* ppt: [20201212_ljx](ppts/20201212_ljx.pdf)

2020/12/26
reporter: Shuang Zeng
* paper1: Juan Li, Ruoxu Wang, Ningyu Zhang, Wen Zhang, Fan Yang, Huajun Chen. 2020. [Logic-guided Semantic Representation Learning for Zero-Shot Relation Classification](https://www.aclweb.org/anthology/2020.coling-main.265/). In *COLING 2020*.
* method: Semantic Mapping in CV + Knowledge Graph Embedding + Rule-based Embedding
* paper2: Junjie Yu, Tong Zhu, Wenliang Chen, Wei Zhang, Min Zhang. 2020. [Improving Relation Extraction with Relational Paraphrase Sentences](https://www.aclweb.org/anthology/2020.coling-main.148/). In *COLING 2020*.
* method: Relational Paraphrase Sentence + Multi-instance Learning
* ppt:  [20201226_zs](ppts/20201226_zs.pdf)


### 2. Semantic Role Labeling
2020/02/23
reporter: Xudong Chen
* paper: Zuchao Li, Shexia He, Junru Zhou, Hai Zhao, Kevin Par Rui Wang. 2019. [Dependency and Span, Cross-Style Semantic Role Labeling on PropBank and NomBank](https://arxiv.org/abs/1911.02851). In *Arxiv Preprint*.
* ppt:  [20200223_cxd](ppts/20200223_cxd.pdf)
* method: BiLSTM + Syntactic Aided + Biaffine

2020/03/22
reporter: Xudong Chen
* paper: Anwen Hu,Zhicheng Dou,Jian-Yun Nie,Ji-Rong Wen. 2019. [Leveraging Multi-token Entities in Document-level Named Entity Recognition](http://playbigdata.ruc.edu.cn/dou/publication/2020_aaai_ner.pdf). In *AAAI 2020*.
* ppt:  [20200322_cxd](ppts/20200322_cxd.pdf)
* method: BiLSTM + Document Attention + CRF

2020/12/05
reporter: Xudong Chen
* paper: Emanuele Bastianelli, Andrea Vanzo, Oliver Lemon. 2020. [Encoding Syntactic Constituency Paths for Frame-Semantic Parsing with Graph Convolutional Networks](https://arxiv.org/pdf/2011.13210.pdf). 
* ppt:  [20201205_cxd](ppts/20201205_cxd.pdf)
* method: GCN+Dependency parsing

### 3. Dependency Parsing
2020/03/15
reporter: Wei Cui
* paper: Daniel Fern´andez-Gonz´alez and Carlos G´omez-Rodr´ıguez. 2020. [Discontinuous Constituent Parsing with Pointer Networks](https://arxiv.org/abs/2002.01824). In *AAAI 2020*.
* ppt:  [20200315_cw](ppts/20200315_cw.pdf)
* method: Constituents as Augmented Dependencies + Pointer Network

2020/04/12
reporter: Wei Cui
* paper: Alireza Mohammadshahi and James Henderson. 2020. [Recursive Non-Autoregressive Graph-to-Graph Transformer for Dependency Parsing with Iterative Refinement](https://arxiv.org/abs/2003.13118). In *Arxiv Preprint*.
* ppt:  [20200412_cw](ppts/20200412_cw.pdf)
* method: Graph-to-Graph Iterative Refinement


### 4. Math Problem Generation
2020/03/01
reporter: Tianyang Cao 
* paper: Xinyu Hua and Lu Wang. 2019. [Sentence-Level Content Planning and Style Specification for Neural Text Generation](https://arxiv.org/abs/1909.09734). In *Arxiv Preprint*.
* ppt: [20200301_cty](ppts/20200301_cty.pdf)
* method: context planning decoder+ style specification

2020/03/08
reporter: Songge Zhao
* paper: Cao Liu, Kang Liu .2019. [Generating Questions for Knowledge Bases via Incorporating Diversified Contexts and Answer-Aware Loss](https://arxiv.org/abs/1910.13108). In *EMNLP 2019*.
* ppt: [20200308_zsg](ppts/20200308_zsg.pdf)
* method: Divisified context + Transformer + Answer-aware loss

2020/03/29
repoter: Tianyang Cao
* paper: Deng Cai, Yan Wang, Wei Bi, ZhaoPeng Tu, XiaoJiang Liu, Shuming Shi. 2019. [Retrieval-guided Dialogue Response Generation via a Matching-to-Generation Framework](https://www.aclweb.org/anthology/D19-1195.pdf). In *EMNLP 2019*.
* ppt: [20200329_cty](ppts/20200329_cty.pdf)
* method: Matching score + skeleton to generation


2020/04/05
repoter: Songge Zhao
* paper: Weichao Wang , Shi Feng , Daling Wang , Yifei Zhang [Answer-guided and Semantic Coherent Question Generation in Open-domain Conversation](https://www.aclweb.org/anthology/D19-1511/). In *EMNLP 2019*.
* ppt: [20200405_zsg](ppts/20200405_zsg.pdf)
* method:RL + AL + CVAE genration

2020/04/26
repoter:Tianyang Cao
* paper: Yun-Zhu Song, Hong-Han Shuai, Sung-Lin Yeh,  Yi-Lun Wu, Lun-Wei Ku, Wen-Chih Peng. 2020. [Attractive or Faithful? Popularity-Reinforced Learning for Inspired Headline Generation](https://arxiv.org/pdf/2002.02095.pdf). In *AAAI 2020*.
* ppt: [20200426_cty](ppts/20200426_cty.pdf)
* method: Article extractor with popular topic attention + popularity predictor + RL

2020/05/24
repoter: Tianyang Cao
* paper: Siqi Bao, Huang He, Fan Wang, Hua Wu and Haifeng Wang. 2020. [PLATO: Pre-trained Dialogue Generation Model with Discrete Latent Variable](https://arxiv.org/pdf/1910.07931.pdf). In *ACL 2020*.
* ppt: [20200524_cty](ppts/20200524_cty.pdf)
* method: Discrete latent variable + context-response matching pretraining

2020/06/21
repoter: Tianyang Cao
* paper: Di Jin, Zhijing Jin, Joey Tianyi Zhou,Lisa Orii,Peter Szolovits. 2020. [Hooks in the Headline: Learning to Generate Headlines with Controlled Styles](http://xxx.itp.ac.cn/pdf/2004.01980.pdf). In *ACL 2020*.
* ppt: [20200621_cty](ppts/20200621_cty.pdf)
* method: Multitask learning and parameters sharing 

2020/06/28
repoter: Songge Zhao
* paper: Tom B. Brown, Benjamin Mann, Nick Ryder, Melanie Subbiah. 2020. [Language Models are Few-Shot Learners](https://arxiv.org/abs/2005.14165). In *Arxiv Preprint*.
* ppt: [20200628_zsg](ppts/20200628_zsg.pdf)
* method: GPT3 pre_train LM

2020/07/12
repoter: Tianyang Cao
* paper: Zhiliang Tian, Wei Bi, Dongkyu Lee, Lanqing Xue, Yiping Song, Xiaojiang Liu,  Nevin L. Zhang. 2020.  [Response-Anticipated Memory for On-Demand Knowledge Integration in Response Generation](https://www.aclweb.org/anthology/2020.acl-main.61.pdf). In *ACL 2020*.
* ppt: [20200712_cty](ppts/20200712_cty.pdf)
* method: teacher-student framework + response-aware document memory construction

2020/07/26
repoter: Songge Zhao
* paper: Chao Zhao, Marilyn Walker, Snigdha Chaturvedi. 2020. [Bridging the Structural Gap Between Encoding and Decoding for Data-To-Text Generation](https://www.aclweb.org/anthology/2020.acl-main.224/). In *ACL 2020*.
* ppt: [20200726_zsg](ppts/20200726_zsg.pdf)
* method: GCN encoder with planning encoder on WebNLG

2020/08/02
repoter: Tianyang Cao
* paper1: Rashmi Gangadharaiah，Balakrishnan Narayanaswamy. 2020. [Recursive Template-based Frame Generation for Task Oriented Dialog](https://www.aclweb.org/anthology/2020.acl-main.186.pdf). In *ACL 2020*.
* paper2: Yanbin Zhao, Lu Chen, Zhi Chen, Ruisheng Cao, Su Zhu, Kai YuLine. 2020. [ Graph Enhanced AMR-to-Text Generation with Mix-Order GraphAttention Networks](https://www.aclweb.org/anthology/2020.acl-main.67.pdf). In *ACL 2020*.
* ppt: [20200802_cty](ppts/20200802_cty.pdf)
* method: slot decoder + tree decoder, dual graph + mix order Graph Attention Network

2020/08/09
repoter: Huan Zhang
* paper: Bayu Distiawan Trisedya, Jianzhong, Qi Rui Zhang. 2020. [Sentence Generation for Entity Description with Content-plan Attention](https://arxiv.org/pdf/1809.00582.pdf). In *AAAI 2020*.
* ppt: [20200809_zh](ppts/20200809_zh.pdf)
* method: content plan + data-to-text

2020/08/23 
repoter: Tianyang Cao
* paper: Tim Van de Cruys. 2020. [Automatic Poetry Generation from Prosaic Text](https://www.aclweb.org/anthology/2020.acl-main.223.pdf). In *ACL 2020*.
* ppt: [20200823_cty](ppts/20200823_cty.pdf)
* method: rhyme constraint + topic constraint (with nonnegative matrix factorization)

2020/09/26
repoter: Tianyang Cao
* paper: Silin Gao, Yichi Zhang1, Zhijian Ou1,Zhou Yu. 2020. [Paraphrase Augmented Task-Oriented Dialog Generation](https://www.aclweb.org/anthology/2020.acl-main.60.pdf) In *ACL 2020*
* ppt: [20200926_cty](ppts/20200926_cty.pdf)
* method: paraphrase generation and two-stage decoder

2020/10/31
repoter: Xiaodan Xu
* paper: Shuang Chen, Jinpeng Wang, Xiaocheng Feng, Feng Jiang, Bing Qin, Chin-Yew Lin. 2019. [Enhancing Neural Data-To-Text Generation Models with External Background Knowledge](https://www.aclweb.org/anthology/D19-1299.pdf). In *ACL 2019*.
* ppt: [20201031_xxd](ppts/20201031_xxd.pdf)
* method: entity linking + seq2seq framework

2020/10/31
repoter: Xiaodan Xu
* paper: Ratish Puduppully, Li Dong, Mirella Lapata. 2019. [Data-to-text Generation with Entity Modeling](https://arxiv.org/pdf/1906.03221) In *ACL 2019*
* ppt: [20201031_xxd](ppts/20201031_xxd.pdf)
* method: entity-special representations + hierarchical attention

2020/11/14
repoter: Tianyang Cao
* paper: Amirhossein Kazemnejad, Mohammadreza Salehi, Mahdieh Soleymani Baghshah. 2020. [Paraphrase Generation by Learning How to Edit from Samples](https://www.aclweb.org/anthology/2020.acl-main.535.pdf) In *ACL 2020*.
* ppt: [20201114_cty](ppts/20201114_cty.pdf)
* method: transformer framework + edit provider + edit performer

2020/11/14
repoter: Tianyang Cao
* paper: Haozhe Ji, Pei Ke1, Shaohan Huang, Furu Wei, Xiaoyan Zhu, Minlie Huang. 2020.[Language Generation with Multi-Hop Reasoning on Commonsense
Knowledge Graph] In *EMNLP 2020*.
* ppt: [20201114_cty](ppts/20201114_cty.pdf)
* method: Multi-layer commonsense knowledge reasoning + GPT2

2020/12/12
repoter: Xiaodan Xu
* paper: Liying Cheng, Dekun Wu, Lidong Bing, Yan Zhang, Zhanming Jie, Wei Lu, Luo Si. 2020.[ENT-DESC: Entity Description Generation by Exploring Knowledge Graph](https://www.aclweb.org/anthology/2020.emnlp-main.90.pdf) In *EMNLP 2020*.
* ppt: [20201212_xxd](ppts/20201212_xxd.pdf)
* method: Multi-graph transformation + aggregation layer

2020/12/12
repoter: Xiaodan Xu
* paper: Xinyu Hua, Lu Wang. 2020.[PAIR: Planning and Iterative Refinement in Pre-trained Transformers for Long Text Generation](https://www.aclweb.org/anthology/2020.emnlp-main.57.pdf) In *EMNLP 2020*.
* ppt: [20201212_xxd](ppts/20201212_xxd.pdf)
* method: Content planner based on BERT + generation framework based on BART + Iterative Refinement

2020/12/19
repoter: Tianyang Cao
* paper: Yufan Zhao, Can Xu, Wei Wu. 2020. [Learning a Simple and Effective Model for Multi-turn Response
Generation with Auxiliary Tasks](https://www.aclweb.org/anthology/2020.emnlp-main.279.pdf) In *EMNLP 2020*.
* ppt: [20201219_cty](ppts/20200219_cty.pdf)
* method:  auxiliary tasks, including masked word recovery and order recovery

2020/12/19
repoter: Tianyang Cao
* paper: Zhangming Chan, Yuchi Zhang, Xiuying Chen, Shen Gao, Zhiqiang Zhang, Dongyan Zhao and Rui Yan. 2020. [Selection and Generation: Learning towards
Multi-Product Advertisement Post Generation](https://www.aclweb.org/anthology/2020.emnlp-main.313.pdf)  In *EMNLP 2020*.
* ppt: [20201219_cty](ppts/20200219_cty.pdf)
* method: Selection Network + Multi-generator Network

2021/01/02
repoter: Songge Zhao
* paper: Rajat Agarwal. 2020. [Acrostic Poem Generation](https://www.aclweb.org/anthology/2020.emnlp-main.94/)  In *EMNLP 2020*.
* ppt: [20210102_zsg](ppts/20210102zsg.pdf)
* method: Language model+Topic Prediction Model

2021/01/16
repoter: Xiaodan Xu
* paper: Qinzhuo Wu, Qi Zhang, Jinlan Fu, Xuanjing Huang. 2020. [A Knowledge-Aware Sequence-to-Tree Network for Math Word Problem Solving](https://www.aclweb.org/anthology/2020.emnlp-main.579.pdf)  In *EMNLP 2020*.
* ppt: [20210116_xxd](ppts/20210116_xxd.pdf)
* method: entity graph + tree-structured decoder + state aggregation mechanism

2021/01/16
repoter: Xiaodan Xu
* paper: Jinghui Qin, Lihui Lin, Xiaodan Liang, Rumin Zhang, Liang Lin 2020. [Semantically-Aligned Universal Tree-Structured Solver for Math Word Problems](https://www.aclweb.org/anthology/2020.emnlp-main.309.pdf)  In *EMNLP 2020*.
* ppt: [20210116_xxd](ppts/20210116_xxd.pdf)
* method: universal expression tree + tree-structured decoder

2021/01/16
repoter: Xiaodan Xu
* paper: Zhipeng Xie, Shichao Sun 2020. [A Goal-Driven Tree-Structured Neural Model for Math Word Problems](https://www.ijcai.org/Proceedings/2019/0736.pdf)  In *IJCAI 2019*.
* ppt: [20210116_xxd](ppts/20210116_xxd.pdf)
* method: top-down goal decomposition + bottom-up subtree embedding

2021/03/20
reporter: Xiaodan Xu
* paper: Arkil Patel, Satwik Bhattamishra, Navin Goyal. 2020. [Are NLP Models really able to Solve Simple Math Word Problems?](https://arxiv.org/pdf/2103.07191.pdf) In *NAACL 2021*.
* ppt:  [20210320_xxd](ppts/20210320_xxd.pdf)
* method: A New DataSet for Math Word Problem Solving, which reveals the deficiency of current benchmark datasets.

2021/04/24
reporter: Xiaodan Xu
* paper: Shangqing Liu, Yu Chen, Xiaofei Xie, Jingkai Siow, Yang Liu. 2021. [Retrieval-Augmented Generation for Code Summarization via Hybrid GNN](https://openreview.net/pdf?id=zv-typ1gPxA) In *ICLR 2021*.
* ppt:  [20210424_xxd](ppts/20210424_xxd.pdf)
* method: Retrieval Augmented + Hybrid GNN with static and dynamic graph.

2021/05/15
reporter: Xiaodan Xu
* paper: Prakhar Gupta, Jeffrey P. Bigham, Yulia Tsvetkov, Amy Pavel. 2021. [Controlling Dialogue Generation with Semantic Exemplars](https://arxiv.org/abs/2008.09075) In *NAACL 2021*.
* ppt:  [20210515_xxd](ppts/20210515_xxd.pdf)
* method: Frame Extraction + Dialogue Generation Framework.

2021/05/15
reporter: Xiaodan Xu
* paper: Deng Cai, Yan Wang, Wei Bi, Zhaopeng Tu, Xiaojiang Liu, Shuming Shi. 2019. [Retrieval-guided Dialogue Response Generation via a
Matching-to-Generation Framework](https://www.aclweb.org/anthology/D19-1195/) In *EMNLP 2019*.
* ppt:  [20210515_xxd](ppts/20210515_xxd.pdf)
* method: Skeleton Extraction + Pipeline Generation.


### 5. Medical Text Processing
2020/03/01
reporter: Huan Zhang
* paper: Bansal, T., Verga, P., Choudhary, N., & McCallum, A. 2019. [Simultaneously Linking Entities and Extracting Relations from Biomedical Text Without Mention-level Supervision](https://arxiv.org/abs/1912.01070). In *AAAI 2020*.
* ppt:  [20200301_zh](ppts/20200301_zh.pdf)
* method: Simultaneously link entities and extract relationships

2020/10/17
reporter: Huan Zhang
* paper: Yun He, Ziwei Zhu, Yin Zhang, Qin Chen, James Caverlee. 2020. [Infusing Disease Knowledge into BERT for Health Question Answering, Medical Inference and Disease Name Recognition](https://arxiv.org/pdf/2010.03746.pdf). In *emnlp 2020*.
* ppt:  [20201017_zh](ppts/20201017_zh.pdf)
* method: disease knowledge + bert + pretrained

2020/12/05
reporter: Huan Zhang
* ppt:  [20201205_zh](ppts/20201205_zh.pdf)
* paper: Alan Ramponi, Rob van der Goot, Rosario Lombardo, Barbara Plank, 2020. [Biomedical Event Extraction as Sequence Labeling](https://www.aclweb.org/anthology/2020.emnlp-main.431.pdf). In *Emnlp 2020*.
* method: biomedical event extraction + sequence labeling



### 6. Named Entity Recognition
2020/03/29
reporter: Huan Zhang
* paper: Angli Liu, Jingfei Du, Veselin Stoyanov,  2019. [Knowledge-Augmented Language Model and Its Application to Unsupervised Named-Entity Recognition](https://arxiv.org/abs/1904.04458). In *NAACL 2019*.
* ppt:  [20200329_zh](ppts/20200329_zh.pdf)
* method: LM + KB + unsupervised + ner(plain text)

2020/04/26
reporter: Huan Zhang
* paper: Changmeng Zheng, Yi Cai, Jingyun Xu, Ho-fung Leung and Guandong Xu, 2019. [A Boundary-aware Neural Model for Nested Named Entity Recognition](https://www.aclweb.org/anthology/D19-1034.pdf). In *EMNLP 2019*.
* ppt:  [20200426_zh](ppts/20200426_zh.pdf)
* method: Boundary-aware + categorical labels prediction + nested ner

2020/05/24
reporter: Huan Zhang
* paper: Esteban Safranchik, Shiying Luo, Stephen H. Bach, 2020. [Weakly Supervised Sequence Tagging from Noisy Rules](http://cs.brown.edu/people/sbach/files/safranchik-aaai20.pdf). In *AAAI 2020*.
* ppt:  [20200524_zh](ppts/20200524_zh.pdf)
* method: Weakly Supervised + Rules

2020/06/14
reporter: Xudong Chen
* paper: Xiaoya Li, Jingrong Feng, Yuxian Meng, Qinghong Han, Fei Wu and Jiwei Li, 2020. [A Unified MRC Framework for Named Entity Recognition](https://arxiv.org/pdf/1910.11476.pdf). In *ACL 2020*.
* ppt:  [20200614_cxd](ppts/20200614_cxd.pdf)
* method: Weakly Supervised + Rules

2020/06/21
reporter: Huan Zhang
* paper: Hiroki Ouchi, Jun Suzuki, Sosuke Kobayashi, Sho Yokoi, Tatsuki Kuribayashi, Ryuto Konno, Kentaro Inui, 2020. [Instance-Based Learning of Span Representations:A Case Study through Named Entity Recognition](https://arxiv.org/pdf/2004.14514.pdf). In *ACL 2020*.
* ppt:  [20200621_zh](ppts/20200621_zh.pdf)
* method: instence-based + ner

2020/06/28
reporter: Yuan Zong
* paper: Xiang Dai, Sarvnaz Karimi, Ben Hachey, Cecile Paris1 2020. [An Effective Transition-based Model for Discontinuous NER](https://arxiv.org/abs/2004.13454). In *ACL 2020*.
* ppt:  [20200628_zy](ppts/20200628_zy.pdf)
* method: ner like dependency parsing


2020/07/12
reporter: Huan Zhang
* paper: Bill Yuchen Lin, Dong-Ho Lee, Ming Shen, Ryan Moreno, Xiao Huang, Prashant Shiralkar, Xiang Ren, 2020. [TriggerNER: Learning with Entity Triggers as Explanations for Named Entity Recognition](https://arxiv.org/pdf/2004.07493v1.pdf). In *ACL 2020*.
* ppt:  [20200712_zh](ppts/20200712_zh.pdf)
* method: entity trigger + ner -> cost-effective result

2020/09/20
reporter: Huan Zhang
* paper: Minlong Peng, Ruotian Ma, Qi Zhang, Xuanjing Huang, 2020. [Simplify the Usage of Lexicon in Chinese NER](https://arxiv.org/pdf/1908.05969.pdf). In *ACL 2020*.
* ppt:  [20200920_zh](ppts/20200920_zh.pdf)
* method: lexicon + named entity recognition

2020/09/26
reporter: Runxin Xu
* ppt:  [20200926_zh](ppts/20200926_xrx.pdf)
* method: Chinese named entity recognition

2020/12/05
reporter: Huan Zhang
* ppt:  [20201205_zh](ppts/20201205_zh.pdf)
* paper: Yuyang Nie, Yuanhe Tian, Xiang Wan, Yan Song, Bo Dai, 2020. [Named Entity Recognition for Social Media Texts with Semantic Augmentation](https://www.aclweb.org/anthology/2020.emnlp-main.107.pdf). In *Emnlp 2020*.
* method: social media texts + semantic AU + ner

2021/01/23
reporter: Yuan Zong
* paper: Qianhui Wu, Zijia Lin, Borje F. Karlsson, Jian-Guang Lou and Biqing Huang 2020. [Single-/Multi-Source Cross-Lingual NER via Teacher-Student Learning on Unlabeled Data in Target Language](https://www.aclweb.org/anthology/2020.acl-main.581/). In *ACL 2020*.
* ppt:  [20210123_zy](ppts/20210123_zy.pdf)
* method: ner + teacher-student


### 7. Law Judgement Prediction
2020/05/03
reporter: Xudong Chen
* paper: Nuo Xu, PinghuiWang, Long Chen, Li Pan, Xiaoyan Wang, Junzhou Zhao,  2020. [Distinguish Confusing Law Articles for Legal Judgment Prediction](https://arxiv.org/pdf/2004.02557.pdf). In *ACL 2020*.
* ppt:  [20200503_cxd](ppts/20200503_cxd.pdf)
* method: GCL + GDO

### 8. Discourse Parsing
2020/05/12
reporter: Wei Cui
* paper: Longyin Zhang, Yuqing Xing, Fang Kong, Peifeng Li, Guodong Zhou. 2020. [A Top-Down Neural Architecture towards Text-Level Parsing of Discourse Rhetorical Structure](https://arxiv.org/abs/2005.02680). In *ACL 2020*.
* ppt:  [20200512_cw](ppts/20200512_cw.pdf)
* method: GRU-CNN-GRU encoder + biaffine attention + Attention-based Encoder-Decoder on Split Point Ranking


### 9. Knowledge Distilling
2020/05/12
reporter: Runxin Xu
* paper: Xiaoqi Jiao, Yichun Yin, Lifeng Shang, Xin Jiang, Xiao Chen, Linlin Li, Fang Wang, Qun Liu. 2020. [TinyBERT: Distilling BERT for Natural Language Understanding](https://arxiv.org/abs/1909.10351). In *ICLR 2020*.
* ppt:  [20200512_xrx](ppts/20200512_xrx.pdf)
* method: Konwledge Distilling


### 10. Data Augmentation
2020/05/31
reporter: Yuan Zong
* paper: Xiaoqi Jiao, Yichun Yin, Lifeng Shang, Xin Jiang, Xiao Chen, Linlin Li, Fang Wang, Qun Liu. 2020. [MixText: Linguistically-Informed Interpolation of Hidden Space for Semi-Supervised Text Classiﬁcation](https://arxiv.org/abs/2004.12239). In *ACL 2020*.
* ppt:  [20200531_zy](ppts/20200531_zy.pdf)
* method: Data mixing + Semi-supervised

2020/12/19
reporter: Yuan Zong
* paper: Akari Asai and Hannaneh Hajishirzi. 2020. [Logic-Guided Data Augmentation and Regularization for Consistent Question Answering (https://www.aclweb.org/anthology/2020.acl-main.499/). In *EMNLP 2020*.
* ppt:  [20201219_zy](ppts/20201219_zy.pdf)
* method: Data Augmentation +  Regularization

### 11. Transformer
2020/06/07
reporter: Runxin Xu
* paper: Hao Peng, Roy Schwartz, Dianqi Li, Noah A. Smith. 2020. [A Mixture of h−1 Heads is Better than h Heads](https://arxiv.org/abs/2005.06537). In *ACL 2020*.
* ppt:  [20200607_xrx](ppts/20200607_xrx.pdf)
* method: Consider multi-head self-attention as a mixture of experts + modify gate mechanism

2020/08/09
reporter: Runxin Xu
* paper: Weiqiu You, Simeng Sun, Mohit Iyyer. 2020. [Hard-Coded Gaussian Attention for Neural Machine Translation](https://arxiv.org/abs/2005.00742). In *ACL 2020*.
* ppt:  [20200809_xrx](ppts/20200809_xrx.pdf)
* method: Replace learned dot-product self-attention with hard-coded gaussian attention.


### 12. Numerical Embedding
2020/05/17
reporter: Songge Zhao
* paper: Mor Geva, Ankit Gupta, Jonathan Berant. 2020. [Injecting Numerical Reasoning Skills into Language Models](https://arxiv.org/abs/2004.04487). In *ACL 2020*.
* ppt:  [20200517_zsg](ppts/20200517_zsg.pdf)
* method: Specific Pre-training + fine-tuning

2020/05/31
reporter: Songge Zhao
* paper: Eric Wallace, Yizhong Wang, Sujian Li, Sameer Singh, Matt Gardner. 2019. [Do NLP Models Know Numbers? Probing Numeracy in Embeddings](https://arxiv.org/abs/1909.07940). In *EMNLP 2019*.
* ppt:  [20200531_zsg](ppts/20200531_zsg.pdf)
* method: to be fixed

### 13. Question Answering
2020/07/05
reporter: Shuang Zeng
* paper1: Lin Qiu, Yunxuan Xiao, Yanru Qu, Hao Zhou, Lei Li, Weinan Zhang, Yong Yu. 2019. [Dynamically Fused Graph Network for Multi-hop Reasoning](https://www.aclweb.org/anthology/P19-1617/). In *ACL 2019*.
* paper2: Nan Shao, Yiming Cui, Ting Liu, Shijin Wang, Guoping Hu. 2020. [Is Graph Structure Necessary for Multi-hop Reasoning?](https://arxiv.org/abs/2004.03096). In *Arxiv Preprint*.
* ppt:  [20200705_zs](ppts/20200705_zs.pdf)
* method: Paragraph Selector + Constructing Entity Graph + Encoding Query and Context + Reasoning with the Fusion Block

2020/07/05
reporter: Xudong Chen
* paper: Shaoru Guo, Ru Li, Hongye Tan, Xiaoli Li, Yong Guan,Hongyan Zhao and Yueping Zhang. 2020. [A Frame-based Sentence Representation for Machine Reading Comprehension](https://www.aclweb.org/anthology/2020.acl-main.83.pdf). In *ACL 2020*.
* ppt:  [20200705_cxd](ppts/20200705_cxd.pdf)
* method: Bert + Frame-based Sentence Representation

2020/09/19
reporter: Ce Zheng
* paper: Jingjing Xu, Yuechen Wang, Duyu Tang, Nan Duan, Pengcheng Yang, Qi Zeng, Ming Zhou and Xu Sun. 2019. [Asking Clarification Questions in Knowledge-Based Question Answering](https://www.aclweb.org/anthology/D19-1172.pdf). In *EMNLP 2019*.
* ppt: [20200919_zc](ppts/20200919_zc.pptx)
* method: Knowledge based data collection

2020/12/19
reporter: Yuan Zong
* paper: Xuguang Wang, Linjun Shou, Ming Gong, Nan Duan, Daxin Jiang. 2020. [No Answer is Better Than Wrong Answer: A Reflection Model for Document Level Machine Reading Comprehension](https://www.aclweb.org/anthology/2020.findings-emnlp.370/). In *EMNLP 2020*.
* ppt:  [20201219_zy](ppts/20201219_zy.pdf)
* method: reflection model

2021/01/23
reporter: Yuan Zong
* paper: Yeon Seonwoo, Ji-Hoon Kim, Jung-Woo Ha, Alice Oh. 2020. [Context-Aware Answer Extraction in Question Answering](https://www.aclweb.org/anthology/2020.emnlp-main.189/). In *EMNLP 2020*.
* ppt:  [20210123_zy](ppts/20210123_zy.pdf)
* method: Block Attention

2021/04/23
reporter: Xudong Chen
* paper: M. Yasunaga, H. Ren, A. Bosselut, P. Liang, J. Leskovec. 2021. [QA-GNN: Reasoning with Language Models and Knowledge Graphs for Question Answering](https://arxiv.org/abs/2104.06378/). In *NAACL 2021*.
* ppt:  [20210423_cxd](ppts/20210423_cxd.pdf)
* method: GCN

### 14. Chinese Word Segmentation and Semi-Supervised Learning
reporter: Yuan Zong
* paper: Ning Ding, Dingkun Long, Guangwei Xu, Muhua Zhu, Pengjun Xie, Xiaobin Wang, Hai-Tao Zheng. 2020. [Coupling Distant Annotation and Adversarial Training for Cross-Domain Chinese Word Segmentation](https://arxiv.org/pdf/2007.08186.pdf). In *ACL 2020*.
* ppt:  [20200717_zy](ppts/20200719_zy.pdf)
* method: Distant Annotation and Adversarial Training

reporter: Yuan Zong
* paper: Mingda Chen, Qingming Tang, Karen Livescu, Kevin Gimpel. 2018. [Variational Sequential Labelers for Semi-Supervised Learning](https://arxiv.org/abs/1906.09535). In *EMNLP 2018*.
* ppt:  [20200823_zy](ppts/20200823_zy.pdf)
* method: VAE and Semi-Supervised Learning

reporter: Yuan Zong
* paper: Jiaao Chen, Zhenghui Wang, Ran Tian, Zichao Yang, Diyi Yang[Local Additivity Based Data Augmentation for Semi-supervised NER](https://arxiv.org/abs/2010.01677). In *EMNLP 2020*.
* ppt:  [20201010_zy](ppts/20201010_zy.pdf)
* method: mixer and Semi-Supervised Learning

reporter: Yuan Zong
* paper: Bosheng Ding, Linlin Liu, Lidong Bing, Canasai Kruengkrai, Thien Hai Nguyen, Shafiq Joty, Luo Si, Chunyan Miao[DAGA: Data Augmentation with a Generation Approach for Low-resource Tagging Tasks](https://arxiv.org/abs/2011.01549). In *EMNLP 2020*.
* ppt:  [20201107_zy](ppts/20201107_zy.pdf)
* method: Data augmentation

reporter: Yuan Zong
* paper: Dayiheng Liu, Yeyun Gong, Jie Fu, Yu Yan, Jiusheng Chen, Jiancheng Lv, Nan Duan, Ming Zhou[Tell Me How to Ask Again: Question Data Augmentation with Controllable Rewriting in Continuous Space](https://arxiv.org/abs/2010.01475). In *EMNLP 2020*.
* ppt:  [20201107_zy](ppts/20201107_zy.pdf)
* method: MRC and data augmentation


### 15. Machine Translation
2020/08/09
reporter: Runxin Xu
* paper: Jian Yang, Shuming Ma, Dongdong Zhang, Zhoujun Li, Ming Zhou. 2020. [Improving Neural Machine Translation with Soft Template Prediction](https://www.aclweb.org/anthology/2020.acl-main.531/). In *ACL 2020*.
* ppt:  [20200809_xrx](ppts/20200809_xrx.pdf)
* method: Soft Template in Target Side.

### 16. Question Generation
2020/09/06
reporter: Xudong Chen
* paper: Liangming Pan Yuxi Xie Yansong Feng Tat-Seng Chua Min-Yen Kan. 2020. [Semantic Graphs for Generating Deep Questions](https://arxiv.org/pdf/2004.12704.pdf/). In *ACL 2020*.
* ppt:  [20200906_cxd](ppts/20200906_cxd.pdf)
* method: GCN.

2021/03/20
reporter: Xiaodan Xu
* paper: Xiyao Ma, Qile Zhu, Yanlin Zhou, Xiaolin Li, Dapeng Wu. 2020. [Improving Question Generation with Sentence-level Semantic Matching and
Answer Position Inferring](https://arxiv.org/pdf/1912.00879.pdf) In *AAAI 2020*.
* ppt:  [20210320_xxd](ppts/20210320_xxd.pdf)
* method: Seq2Seq + Sentence-level Semantic Matching + Answer Position Inferring

2021/04/24
reporter: Xiaodan Xu
* paper: Xiaojing Yu, Anxiao (Andrew) Jiang. 2021. [Expanding, Retrieving and Infilling: Diversifying Cross-Domain Question Generation with Flexible Templates](https://www.aclweb.org/anthology/2021.eacl-main.279.pdf) In *EACL 2021*.
* ppt:  [20210424_xxd](ppts/20210424_xxd.pdf)
* method: Soft Template Retrieval + Neural Generation.

### 17. Language Model
2020/10/10
reporter: Shuang Zeng
* paper: Ikuya Yamada, Akari Asai, Hiroyuki Shindo, Hideaki Takeda, Yuji Matsumoto. 2020. [LUKE: Deep Contextualized Entity Representations with Entity-aware Self-attention](https://arxiv.org/abs/2010.01057). In *EMNLP 2020*.
* ppt:  [20201010_zs](ppts/20201010_zs.pdf)
* method: Pre-training models treating entity as token, proposing entity-aware self-attention mechanism.

2021/01/05
reporter: Huan Zhang
* paper: Colin Raffel, Noam Shazeer, Adam Roberts, Katherine Lee, Sharan Narang, Michael Matena, Yanqi Zhou, Wei Li, Peter J. Liu. 2019. [Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer](https://arxiv.org/pdf/1910.10683.pdf). In *ACL 2019*.
* ppt:  [20210102_zh](ppts/20210102_zh.pdf)
* method: google T5 model


### 18. Abstractive Summarization
2020/12/05
reporter: Xudong Chen
* paper: Hanqi Jin,Tianming Wang,Xiaojun Wan. 2020. [SemSUM: Semantic Dependency Guided Neural Abstractive Summarization](https://ojs.aaai.org//index.php/AAAI/article/view/6312). In *AAAI 2020*.
* ppt:  [20201205_cxd](ppts/20201205_cxd.pdf)
* method: Semantic Dependency Parsing

### 19. Sequence Labeling
2021/01/05
reporter: Huan Zhang
* paper: Ben Athiwaratkun, Cicero Nogueira dos Santos, Jason Krone, Bing Xiang. 2020. [Augmented Natural Language for Generative Sequence Labeling](https://www.aclweb.org/anthology/2020.emnlp-main.27.pdf). In *EMNLP 2020*.
* ppt:  [20210102_zh](ppts/20210102_zh.pdf)
* method: Pre-training models + fine tuning + generated sequence  labeling
