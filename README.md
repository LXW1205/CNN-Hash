# 我的九月份论文

## CNN
【1】颜水成老师在AAAI2014上发表了第一篇将深度学习和哈希学习结合在一起的工作，不是一个端到端的工作。在第一阶段使用了坐标下降的方法。

    [Supervised Hashing for Image Retrieval via Image Representation Learning(AAAI14)]

【2】用了一个端到端的方法，loss是triplet-loss,考虑到了bit之间的冗余问题.只是找triplet对,然后进行loss计算。在结构上,选取了类似 NIN(考虑怎么好)的想法,最后hash bit 时，没有进行全连接的方法，而是分着连接，好处是减少了冗余.

    [Simultaneous Feature Learning and Hash Coding with Deep Neural Networks(CVPR15)]
    
【3】

    [Deep Semantic Ranking Based Hashing for Multi-Label Image Retrieval(CVPR15)]    
    
## RNN-text
【1】不是一个端到端的方法，很多地方处理的比较粗糙。考虑词嵌入和位置嵌入，卷积后结合，得到隐式特征，再将显示特征加进来，最后还得使用tf-idf得到的进过进行监督。

    [Convolutional Neural Networks for Text Hashing(ijcai15)]
    
【2】RNN文本分类，用了线性的上下文，将时间的复杂度降为O(N),RCNN结构很好。使用了双向RNN作为CNN-max-pooling的输入

    [Recurrent convolutional neural networks for text classification (AAAI15)]
    
【3】这篇论文就是RCNN的推崇者，在RCNN的基础上，加了一层。参考文献倒是有很多可借鉴的。分析的也还好.RNN因为更看重后面的内容，效果不好。CNN要考虑卷积大小，所以提出了一个结合的方法。词序很重要，一个文本分类的脉络。要看。序列长度对模型的影响。RCNN在short text上效果并没有那么的好

    [Learning text representation using recurrent convolutional neural network with highway layers(arxiv16)]
    
【4】曹樾的将CNN 和 RNN 结合起来的cross-modal模型。将各个目标函数放在一起。

    [Deep Visual-Semantic Hashing for Cross-Modal Retrieval(KDD16)]

## 推荐系统
【1】google的文章，以后要多关注。只用线性的方法做，泛化性能不好。用深度提取特征，在稀疏高质的情况下效果不好，将其结合。

    [Wide  Deep Learning for Recommender Systems]
## 杂
【1】将编码的学习和哈希函数的学习进行相互促进。

    [Optimizing Affinity-Based Binary Hashing Using Auxiliary Coordinates(Nips16)]
    

    
【2】这个帮助不大，做对话系统什么的

    Sequential Short-Text Classification with Recurrent and Convolutional Neural Networks
 
## 要看





【4】Supervised and Semi-Supervised Text Categorizationusing LSTM for Region Embeddings

【5】Deep Fusion LSTMs for Text Semantic Matching

【6】Long-term Recurrent Convolutional Networks for Visual Recognition and Description

【7】sequence to sequence learning with neural networks

【8】he kai ming

【9】Long short-term memory.

【10】A convolutional neural network for modelling sentences（ACL14）

【11】Convolutional Neural Networks for Sentence Classification(引用高)

【12】Bidirectional recurrent neural networks(双向RNN)

【13】Dropout: A simple way to prevent neural networks from overfitting(dropout)

【14】Semantic compositionality through recursive matrixvector spaces(高引用)

【15】Network in Network

【16】Deep Semantic Ranking Based Hashing for Multi-Label Image Retrieval(CVPR15)

【17】Deep Learning of Binary Hash Codes for Fast Image Retrieval(CVPR15)

【18】Deep Hashing for Compact Binary Codes Learning(CVPR15)
