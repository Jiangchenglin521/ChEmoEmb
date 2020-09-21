# 中文细粒度情感词整理
## 中文情感词和词向量
### sentiment constraints in consideration

> 总述

* 主要是提供一份基于情感本体数据清理好的 目前来说最完整且结构化的情感细粒度词汇。以及一份训练好的供参考的中文情感细粒度的词向量。近15000个词汇供给使用。
* 目的：引入情感信息，让情感分析相关任务从最基本的表示特征上具有更强的说服性，更有理可循。

> 注意

* 目前为第一版本数据，考虑的是sentiment特征，已经有明显的提升
* 与训练词向量选的是 腾讯800w中文词向量，这个词向量的好处是，免费开源，可靠持续更新。

> 使用

* 方法一：可以使用embedding.py脚本训练自己的程序，但是需要自己组建极性数据的pair以及与训练好的词向量。并且要根据自己的需求调整训练参数以及半径，需要调试到好的实验效果。
* 方法二：可以直接使用我提供的数据，本人已经在情感对话，情感分类，情感分布分析上验证过了，都能取得比较好的效果
* 仅做学术研究使用，使用者需要标明出处。
* 数据源：清理好的源情感词典：https://download.csdn.net/download/weixin_40660300/12840023 （设置了很低的积分下载，如没有积分，请联系我，调整积分或者直接发给你）


> TODO：

* 进一步显性的验证带有情感的词向量所表现出的作用，比如说监控一下在attention以及情感词部分模型学习的敏感度。
* 引入情感分布以及情感变换的信息，作序列分析引入constraints中。






## Citation

* 1, Seyeditabari, A., Tabari, N., Gholizadeh, S., & Zadrozny, W. (2019). Emotional Embeddings: Refining Word Embeddings to Capture Emotional Content of Words. arXiv preprint arXiv:1906.00112.

* 2, L. Xu, “Constructing the affective lexicon ontology,” Journal of the China
Society for Scientific & Technical Information, 2008.
