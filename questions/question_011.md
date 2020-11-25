| 第11讲答疑&nbsp;问题列表  |
|--------------|
|BM25算法相对于tf-idf是不是相当于某种程度上限制了score的范围？为什么BM25的score计算要用 d/avgDl, 而不是用开根号或取对数等计算方法？|
|深度神经网络是否可以用于搜索呢|
|能否使用正则表达式来分解布尔查询|
|对于布尔查询的查询语句，是否可以采用分治的方法：碰到括号就把括号里的查询子句交给一个函数A去处理，在里面再碰到括号就再把更里面的查询字句交给递归调用A去处理，直到处理到不包含括号的布尔表达式，将查询结果返回。这个过程就像是树的深度优先遍历|
|表达式是不是可以使用栈读取成对括号里的内容，然后其他部分使用二叉树的中序遍历来进行解析？|
|除了通过自己实现搜索功能来理解搜索原理外，能否专门讲讲如何利用现有工具实现高效的搜索？|
|计算词频的时候是不是在正文中也需要根据词语出现的位置进行权重变化，比如首句和结尾句的语句可能会有总结性，需要较大的权重|
|是否可以根据bool查询的优先级规则设计打分规则呢？像“（华为｜苹果）&手机”这个例子，手机的优先级更高，所以rank的时候把它设置为x2，华为则设置成x1|
|感觉对tfidf和bm25的区别没有太理解|
|用过知网上高级检索之类的功能，他们都是用点选的方式限定条件而不是让用户自行输入and、or,这种方式是否更加友好？|
|文本相似度还有别的计算方法吗|
|如果考虑查询词在候选文档内的位置信息，我能够想到的是一些标题，摘要，关键字(非正文)，还可以有哪些方式呢？|
|自己对于and和or的理解，像在多个文档中两个词都出现的话可以用and处理，很少一起出现的词可以用or处理|
|咱们最后在讲如何把“华为and手机”这种表示转化为“华为&手机”时，是不是也要考虑用户搜索的时候本身就输入的是“华为&手机”这种情况呢|
|布尔查询中，不同集合之间不能硬性合并吧，比如有的元素包括苹果手机但不包括5G，这种也需要选到列表里，然后要怎么做排序呢|
|老师我想问一下，咱们这个课上讲的搜索引擎是先去实现一个基础功能，再优化改进。很多其他编程几乎也都是这个思路，那从大的方面来讲，优化应该从什么方面切入呢？是自己想到哪优化哪一块还是说提前能想好从哪几方面进行|
|查了一些资料发现现有的搜索引擎检索模型还有很多种，比如向量空间模型，基于的是文档特征组成的t维向量；概率模型、语言模型基于的是概率相关性；机器学习排序算法基于了200多种因子，也可以人工对相关文档打分。|
|布尔查询不会给出文档的相关程度，这种特点比较适用于哪种查询需求呢？|
|在科研的过程中，如何有意识地培养自己的元思考能力？|
|如何在tf-idf与bm25之间进行选择？计算更复杂会不会在数据量大的时候占用过多的时间？|
|bm25算法存在一个缺陷，只能命中文档中重合的词，后续是否有相似语义部分的改进呢，实现一些语义搜索|
|关于布尔查询...是不是只能查出来是否在文档中而不能找到相关性（也就是不能进行排序）呢？同时怎么平衡准确率和召回率的问题呢……|
|对元思考还有一些没理解…感觉老师讲的元思考是一种系统化科学化的思维方式？|
|最后讲的问题，可否用正则匹配解决？或者是直接在处理前将空格消去？|
|针对tf-idf和bm25不足的地方，他不能体现单词的位置信息，那有没有什么算法是解决这个问题的呢，或者该怎么去优化呢，感觉对于不同位置的特征词赋予不同的系数权值有点模糊|
|搜索引擎在未来扮演怎样的角色，是否会与一些新技术结合产生更大的价值|
|tfidf有什么不足之处 应如何改进|
|基本的一个逻辑可以是，分词之间默认and，感觉这样也是符合用户搜索逻辑的。|
|bm25中 R（q，d）的这么复杂的公式是怎么得出来的呢？相比于tf-idf的公式，感觉R（q，d）没有这么直观|
|现在常用的搜索引擎都有针对布尔语句进行处理吗|
|学习思想和比代码更关键，学会了思想用什么语言都可以实现|
|对于5g手机这种分词为5g,手机的词。可以通过探测下一个and or not这些符号的位置来决定是否加&将他们连一起吧|
|对关键词设权重的时候，可以在后台设立一个统计平台，根据历史搜索来确定权重吗|
|请问老师，对于不规范的布尔表达式查询，怎么样才能最大程度猜到用户真正想查询到的东西呢。|
|突然想到 按照现有的逻辑 如果文档集发生增删,那么ranking以及indexing是需要重新做一遍的。那么主流搜索引擎对于网页的爬取更新应该是比较及时迅速的,他们是如何应对这个问题的呢？的确是要每次更新都重新计算ranking和indexing吗？|
|BM25中公式中的k1和b的参数设置如何根据需要自己调节？|
|1.在对搜索结果排序时能否把包含搜索词(全部字)的排在搜索结果前面，然后再把剩下的按与搜索词相似度排序 <br/>2.打分算法现在已经讲了好几种了，那实际中应该如何选择|
|对bm25中使用的idf公式还不是很理解。分子文档总数减去关键词词频后，idf不就可能会出现负值了吗？|
|根据用户的诉求不同所设置的权重不同，那我们没搜索一次还要重新设置一次权重吗？|
|布尔查询时查询cut中连在一起的词感觉都是“与”的关系，那可不可以直接把输出中连在一起的集合之间加上&呢|