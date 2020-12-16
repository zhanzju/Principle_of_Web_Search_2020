| 第14讲答疑&nbsp;问题列表  |
|--------------|
|这节课最令我惊艳的收获是老师解释为什么选择余弦相似度而不选择正弦相似度，原因其实很好理解，但是答案是在第三层，而我的思维好像只停留在第二层，这样深层次的思考才是我今后应该好好锻炼的吧|
|"关于市面上常见的搜索引擎，输入长句的搜索结果更好还是关键词的搜索结果更好？<br/>比如：“一起吃螃蟹和柿子会中毒吗”和“螃蟹 柿子 中毒”"|
|"向量空间模型是不是就是去停用词，取出实体词，然后将每个实体词的tf-idf（归一化后的）作为这篇文章向量空间的维度，这样就相当于将文章都映射到一个多维空间上了，再设计范数也就是文档向量间距离（n维就用n范数）去计算文档之间以及文档和关键词之间的关联度（相似度）了吗？<br/>然后余弦相似度的话，我觉得可能会出现一种情况，比如向量a是向量b的延展，例如a（1，1，1，1），b（2，2，2，2）这样的话，他们与向量c（1，2，3，4）的夹角是一样的，那么余弦相似度不就没有区分了嘛？但是实际上用n范数的方法计算出的ab、ac之间的相似度应该是不一样的吧？"|
|"1.向量维度最高可以到多少呢？有上限嘛？<br/>2.annoy除了欧式距离还有其他什么距离可以用吗？"|
|向量空间方法用来计算文本相似度对于小规模还行，大规模用ann感觉确实没法训练（用bert训练好的网络来做文档向量可能会可以，但又会时间问题），或者Google这种巨头才能做到，还是tfidf来的出文档向量比较简单可靠~|
|讲到向量空间模型时，表示向量需要确定维度，考虑相似性的时候要适当降维。有没有什么算法可以这种平衡准确性和复杂度。谢谢老师。|
|大问卷字数理论上越多越好。那有没有建议字数呢？|
|最后一次课啦！感谢老师一学期的辛苦～问一个与内容无关的问题，怎样培养自己提问题的能力呢？不管是开组会还是上课，每次都觉得其他同学提的问题很有水平，确实击中了自己不明白的点，但轮到自己总是憋不出什么问题...|
|我们对于单个词语在文中的关联性已经进行了很详细的分析，但是在具体语境中还存在上下文关系，信息的检索本质是语义的检索而不单纯是词汇的检索，我们是不是应该考虑上下文语境的影响作用，提高信息检索的查准率和查全率，但是这一部分的实现思路应该是什么呢|
|感觉传统向量空间模型还是根据文档中词的匹配度来计算相似度，感觉还是更想知道近义词的解决方案|
|什么是词向量|
|因为平时也想通过学习和工作去总结一些方法论，所以想问一下老师怎样去学习和整理平时科研学习中的一些思维方式和方法论？|
|"1.关于向量的问题，我发现自己好想对向量的知识忘的差不多了，那我要是不是要先补一下向量的知识，还是在以后学习搜索引擎过程中边学边补，缺什么补什么？<br/>2.关于ANN，不管是用这个方法，还是python别的第三方库，我需要去理解库本身的原理吗？这节课听您讲的延伸好像挺难的。<br/>3.关于图形化显示的问题，跟着您的课学到现在，基本上能完成简单的搜索，但是运行的方法或者呈现出来的结果似乎不是那么完美，下一步我想进一步完善这个搜索引擎，类似于谷歌那样的界面，请问老师我应该使用什么开发工具，有没有好的已有的框架推荐下？<br/>4.希望老师在答疑中能够总结一下就目前程序已经完成的部分，对应实际的搜索引擎，已经完成了哪些功能？下一步还需要做哪些工作？方便课下我们进一步学习有个正确的方向。"|
|这个学期课程缩短了，结束后有没有什么需要学生自行学习补充的吗，比如去年的课程有没有哪些值得回顾的，python需要系统性的学习吗？|
|不得不说每次看答疑课程，最快乐的时光莫过于看到老师回答自己的问题！不过后面几次课程感觉自己提不出特别有价值的问题了。所以在这里再次表达一下对老师期末考核方式的点赞和感激！如果老师以后还开课，我必须推荐给我的师弟师妹，不来血亏哈哈|
|"1. 这节课提到的将“文档->向量”，是不是就是NLP中的representation learning（embedding）呢？文档向量、word vector以及char vector，它们的作用分别是什么呢（或者说为什么要生成词向量、字向量呢）想听陈老师再解释一下<br/>2. “以始为终，以终为始”：当我在学习新知识/一个新技术的时候，这种思维方式还适用吗？<br/>3. 关于思维导图的使用：我个人也是比较喜欢用思维导图的方式取总结自己学过的内容，但看了陈老师的图后，觉得之前自己做的思维导图上细节太多了。一张思维导图应该做成什么样子才能发挥它最大的作用呢？"|
|觉得老师遇到问题时总能淡然面对，想问一下老师以后在科研中遇到挫折应该怎样面对？谢谢|
|如果想要度量词向量各维度之间的相关性，在不知道各个维度数据分布的情况下，选择什么相关系数来度量各维度之间的相关性比较好？|
|elasticsearch可以当做数据库使用吗|
|课上提到一个将大量词汇坐标投影到一个正交的200维的坐标系中，这种坐标系的构建有较为具体的方式或者思路吗？后面讲到的不规则分区的是其中的一种方式吗？|
|词向量是如何对同一个词的不同词意进行区分的呢|
|向量空间模型单纯对关键词进行建模，我觉得丢失掉最多的是语法上的信息，是否关键词集合已经可以代替文档本身了呢？|
|有关传统的向量空间：它会假设词与词之间是相互独立的，即一个关键词唯一代表一个概念或语义单元，但是在实际中文档里面存在很多的一词多义和同义词现象，那这种情况下传统的向量空间就不再适应了吧……|
|"1 对于搜索排序算法后续的学习，老师可以推荐一条学习路线吗（上课听老师讲的学习模式，学习思维，确实值得大家好好思考，但往往要去实践的时候还是会很迷茫，主要还是因为太菜了）<br/>2 老师对于英语的学习有什么建议吗（听力以及文献阅读写作方面）"|
|今后的搜索可能会采用交互性的吗，通过不断提供备选让用户选择，最终了解用户的搜索意图。现在好像有这样的，但只在有限应用场景里出现，请问在大规模应用上有可行性吗|
|对于研究方向的学习，有两种思路应该和老师这节课一样，先从基础出发，掌握发展脉络，一步步到最新方向；还是先从最新方向入手，需要基础知识的时候再回头补充基础的知识。老师能评价下两种思路吗？|
|有什么方法可以应对缩写问题吗？|
|文档是多维的，这个多维该怎么理解，又该怎么判断文档维度，还有维度是什么意思，是自己设定的吗？|
|如何权衡解决同一问题的算法的优劣？|
|词向量维度是否越多越好，在增加词向量维度时有哪些限制因素|
|老师课上提到“向量空间模型”，我看了一下这个方法是将文档分为一系列词，再用它们的权重组成一个向量，同样我们输入的检索词条也把权重组成一个向量，用判断两个向量夹角大小的方式找出最相似的两个向量，但我有个问题，我们输入的检索语句一般较短，可能每个词只出现一次，那权重若用频率计算，岂不是权重几乎相同？比如我输入“网络搜索引擎”，没有重复词，权重一样，那用这个向量去跟文档向量做内积，还能找出有效的搜索内容吗？|
|既然向量空间搜索法是将查询与候选文档映射到向量空间中，之后在这个空间中计算相似度。那是不是任何输入格式的查询以及候选文档，只要能映射到这个空间，都能够实现搜索。比如现在类似于淘宝app上的以图搜商品这一功能是不是就是使用今天讲的向量空间搜索的方法来实现的呢。|
|老师我想问下想要学习一个新技术的时候怎么确定学习路线。有时候上网找别人推荐的学习路线都各式各样的。是要这个技术相关的知识都先了解一点再自己制定一个路线吗。谢谢老师|
|当文档集发生改变，譬如新加或删除，这将伴随着向量空间的变化，每次文档集的改变是否会造成很大的开销？|
|向量空间模型应用在实际的时候，如果文档内容过长，内积过小或者维数过高，另外，当只有部分词组对上的时候，会出现“假”匹配，在这种情况下，模型还能得到理想结果吗？|
|以角度作为相似度的区分 在向量空间中是否会造成区分度不明显的情况？我脑海中想象的文档向量空间大概是 散落成数个堆（类）的点。尤其对堆内的点来说 以角度区分是不是区分太小了。当然有可能维度高了以后并不是我想象得那样。|
|向量空间的距离衡量方式选取对最终效果有什么影响？|
|特征空间的维度越高，是否向量所能表示语义信息更加丰富？由文本到向量的信息损失更少？|
|首先思考针对一个任务的问题，以问题为驱动来学习，比如课上讲的通过思考搜索中的语义匹配问题引出vsm。但在实际中我可能在学习的时候还不知道vsm这个模型，我可能就想不到语义匹配这个问题，这种情况怎么办？但直接通过学习技术来了解需要解决的问题是不是会限制自己的思考呢？|
|"感觉向量空间模式和之前讲的还是比较相似的，是不是可以理解为用一个模型把他规范了起来。相似性计算就比较能变出花样了。<br/>ANN那个图听的不是很明白，有点迷。"|
|既然大部分语言模型都是在捕捉数据中的统计相关性或共现关系，那么理论上语义是否能够完全由统计信息来度量？目前语言模型的瓶颈主要在哪些方面？|
|本次课程并没有进行代码实现，而是通过讲述建立搜索引擎中遇到的问题，以及解决问题所提出的各种技术，以及这种技术的缺陷，以及解决这种缺陷带来的技术……不断迭代下去。相比于代码实现的思维发散的速度，更快一些，可能效果更好？|
|我们把词映射到一个特征空间中去获得词的向量表达，而老师你上课提到句子的向量可以通过把一句话中所有词加起来获得。我觉得从空间维度上来讲，句子和单词的特征空间是有差异的，单词的加和结果应该还是单词，并不能很好的表征句意，例如 king+female=Queen 还是单词。并且从直觉上来讲句子特征空间维数应该更高，显然是不能通过单词之间的线性计算得到句子的。不知道我这样的理解对不对，以及如果是这样的话我们应该怎么获得更好的句子表征呢？|
|在构建向量的维度时，应该根据什么标准选择呢？|