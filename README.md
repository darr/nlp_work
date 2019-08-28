# work

## chinese textual inference

https://github.com/darr/chinese_textual_inference  

project including chinese corpus build and inferecence model,  
中文文本推断项目,包括88万文本蕴含中文文本蕴含数据集的翻译与构建,  
基于深度学习的文本蕴含判定模型构建.  

## product knowledge graph

https://github.com/darr/product_kg  

a knowledge graph that contains the product-product hierarchy producer sales goods relationship,
which sum up to 1300 products and more than 90000 brands,

基于京东网站的1300种商品上下级概念，约10万商品品牌，约65万品牌销售关系，  
商品描述维度等知识库，基于该知识库可以支持商品属性库构建，商品销售问答，  
品牌物品生产等知识查询服务，也可用于情感分析等下游应用．  

### 数据介绍

1, 基本数据内容
![image](https://github.com/darr/product_kg/raw/master/image/info.png)
2, is-a概念上下位关系
![image](https://github.com/darr/product_kg/raw/master/image/is_a.png)
3, sale销售关系
![image](https://github.com/darr/product_kg/raw/master/image/sale.png)
4, 混合关联关系
![image](https://github.com/darr/product_kg/raw/master/image/mix.png)

## HumorDetection

https://github.com/darr/chinese_humor_sentiment

chinese Humor Detection or Computation based on corpus and nlp methods,  
基于语料库与NLP方法的中文幽默计算与检测项目  

### 中文幽默计算模型
模型思想:采用四层双向lstm进行网络搭建,给出一个初步的baseline.以下是训练实际情况.

| 模型 | 训练集 | 测试集 |训练集准确率 |测试集准确率 |备注|模型名称|
| :--- | :---: | :---: | :--- |:--- |:--- |:--- |
| 幽默等级 | 6436 | 1610| 0.8891|0.6137|5分类|BiLSTM |
| 幽默类型 | 5938 | 1460| 0.9357|0.7096|3分类|BiLSTM |
| 幽默类型 | 5938 | 1460| 0.9357|0.7356|3分类|CNN |
| 幽默类型 | 5938 | 1460| 0.9357|0.7103|3分类|CNN-ATT |
| 隐喻类别 | 3515 | 879| 0.9166|0.8089|2分类|BiLSTM |
| 隐喻情绪 | 2904 | 726| 0.8134|0.5399|7分类|BiLSTM |

## poem mining

https://github.com/darr/poem

Chinese Classic Poem Mining Project including corpus buiding by spyder and content analysis by nlp methods,  
基于爬虫与nlp的中国古代诗词文本挖掘项目  

### 阶段性成果

1, 古代诗词语料库,一共采集到92127首古代诗词  
2, 古代诗词外部计量分析结果，结果保存至result文件夹  
3, 诗人足迹一键生成，使用方式如下，结果会直接生成以搜索诗人名字命名的html文件：

以下是举例结果：     

![image](https://github.com/darr/poem/raw/master/results/libai.png)
![image](https://github.com/darr/poem/raw/master/results/liqingzhao.png)
![image](https://github.com/darr/poem/raw/master/results/liyu.png)
![image](https://github.com/darr/poem/raw/master/results/sushi.png)
![image](https://github.com/darr/poem/raw/master/results/taoyuanming.png)
![image](https://github.com/darr/poem/raw/master/results/wentianxiang.png)
![image](https://github.com/darr/poem/raw/master/results/xinqiji.png)

![image](https://github.com/darr/poem/raw/master/results/author_select.png)
![image](https://github.com/darr/poem/raw/master/results/authors.png)


## Chinese word form

https://github.com/darr/chinese_word_form

针对中文词语的笔画拆解，偏旁查询，拼音转换接口．
当前的中文信息处理中，语言外部形式上的特征在各个任务中扮演着越来越重要的角色.
本项目目的是为提供这一接口.


### reuslts

```shell
句子：自然语言处理是人工智能皇冠上的一颗明珠
笔画： ['丿丨𠃍一一一', '丿㇇丶丶一丿㇏丶丶丶丶丶', '丶㇊一丨𠃍一丨𠃍一', '丶一一一丨𠃍一', '丿㇇㇏丨丶', '一一丨㇀丨𠃍一一丨一一', '丨𠃍一一一丨一丿㇏', '丿㇏', '一丨一', '丿一一丿丶丨𠃍一丨𠃍一一', '𠃋丶丨㇆一一丿乚丿乚', '丿丨𠃍一一一一丨一', '丶㇇一一丿乚一亅丶', '丨一一', '丿丨𠃍一一丿㇆丶', '一', '丨𠃍一一一丨丿丶一丿丨𠃍丿丶', '丨𠃍一一丿㇆一一', '一一丨㇀丿一一丨丿㇏']
拼音： ['zi', 'ran', 'yu', 'yan', 'chu', 'li', 'shi', 'ren', 'gong', 'zhi', 'neng', 'huang', 'guan', 'shang', 'de', 'yi', 'ke', 'ming', 'zhu']
偏旁部首： ['自', '灬', '讠', '言', '夂', '王', '日', '人', '工', '日', '月', '白', '冖', '一', '白', '一', '页', '日', '王']


句子：在技术上，深度学习技术会越来越强，新的语言模型和编码器也会越来越好。
笔画： ['一丿丨一丨一', '一亅㇀一丨㇇㇏', '一丨丿㇏丶', '丨一一', '，', '丶丶㇀丶㇇丿丶一丨丿㇏', '丶一丿一丨丨一㇇㇏', '丶丶丿丶㇇㇇亅一', '㇆丶㇀', '一亅㇀一丨㇇㇏', '一丨丿㇏丶', '丿㇏一一𠃋丶', '一丨一丨一丿㇏一𠄌㇂丿丶', '一丶丿一丨丿㇏', '一丨一丨一丿㇏一𠄌㇂丿丶', '𠃍一㇉丨𠃍一丨𠃍一丨一丶', '，', '丶一丶丿一一亅丿丶丿丿一丨', '丿丨𠃍一一丿㇆丶', '丶㇊一丨𠃍一丨𠃍一', '丶一一一丨𠃍一', '一丨丿丶一丨丨丨𠃍一一一丿㇏', '一一丿丨丨亅一丨一', '丿一丨丿丶丨𠃍一', '𠃋𠃋㇀丶𠃍一丿丨㇆一丨丨', '一丿丨𠃍一𠃍㇉一', '丨𠃍一丨𠃍一一丿㇏丶丨𠃍一丨𠃍一', '㇆丨乚', '丿㇏一一𠃋丶', '一丨一丨一丿㇏一𠄌㇂丿丶', '一丶丿一丨丿㇏', '一丨一丨一丿㇏一𠄌㇂丿丶', '𡿨丿一㇇亅一', '。']
拼音： ['zai', 'ji', 'shu', 'shang', '，', 'shen', 'du', 'xue', 'xi', 'ji', 'shu', 'hui', 'yue', 'lai', 'yue', 'qiang', '，', 'xin', 'de', 'yu', 'yan', 'mo', 'xing', 'he', 'bian', 'ma', 'qi', 'ye', 'hui', 'yue', 'lai', 'yue', 'hao', '。']
偏旁部首： ['土', '扌', '木', '一', '，', '氵', '广', '子', '乙', '扌', '木', '人', '走', '木', '走', '弓', '，', '斤', '白', '讠', '言', '木', '土', '口', '纟', '石', '口', '乙', '人', '走', '木', '走', '女', '。']


句子：本项目是中文词语的笔画拆解，偏旁查询，拼音转换接口
笔画： ['一丨丿㇏一', '一丨㇀一丿丨𠃍丿丶', '丨𠃍一一一', '丨𠃍一一一丨一丿㇏', '丨𠃍一丨', '丶一丿㇏', '丶㇊㇆一丨𠃍一', '丶㇊一丨𠃍一丨𠃍一', '丿丨𠃍一一丿㇆丶', '丿一丶丿一丶丿一一乚', '一丨𠃍一丨一𠃊丨', '一亅㇀丿丿一丨丶', '丿㇇丿㇆一一丨㇆丿丿一一丨', '，', '丿丨丶𠃍一丿丨㇆一丨丨', '丶一丶丿丶㇇丶一㇆丿', '一丨丿㇏丨𠃍一一一', '丶㇊丿㇆丨𠃍一一', '，', '一亅㇀丶丿一一丿丨', '丶一丶丿一丨𠃍一一', '一𠃋丨㇀一一ㄣ丶', '一亅㇀丿㇇丨𠃍一丿㇏', '一亅㇀丶一丶丿一𡿨丿一', '丨𠃍一']
拼音： ['ben', 'xiang', 'mu', 'shi', 'zhong', 'wen', 'ci', 'yu', 'de', 'bi', 'hua', 'chai', 'jie', '，', 'pian', 'pang', 'cha', 'xun', '，', 'pin', 'yin', 'zhuan', 'huan', 'jie', 'kou']
偏旁部首： ['木', '工', '目', '日', '丨', '文', '讠', '讠', '白', '毛', '田', '扌', '角', '，', '亻', '方', '木', '讠', '，', '扌', '音', '车', '扌', '扌', '口']


句子：中文信息处理当中，语言外部形式上的特征在各个任务中扮演着越来越重要的角色
笔画： ['丨𠃍一丨', '丶一丿㇏', '丿丨丶一一一丨𠃍一', '丿丨𠃍一一一丶㇂丶丶', '丿㇇㇏丨丶', '一一丨㇀丨𠃍一一丨一一', '丨丶丿𠃍一一', '丨𠃍一丨', '，', '丶㇊一丨𠃍一丨𠃍一', '丶一一一丨𠃍一', '丿㇇丶丨丶', '丶一丶丿一丨𠃍一𠄎丨', '一一丿丨丿丿丿', '一一丨㇀㇂丶', '丨一一', '丿丨𠃍一一丿㇆丶', '丿一丨㇀一丨一一亅丶', '丿丿丨一丨一丨一', '一丿丨一丨一', '丿㇇㇏丨𠃍一', '丿㇏丨', '丿丨丿一丨一', '丿㇇㇏㇆丿', '丨𠃍一丨', '一亅㇀丿㇏㇆丿', '丶丶㇀丶丶㇇一丨𠃍一丨一丿丶', '丶丿一一一丿丨𠃍一一一', '一丨一丨一丿㇏一𠄌㇂丿丶', '一丶丿一丨丿㇏', '一丨一丨一丿㇏一𠄌㇂丿丶', '丿一丨𠃍一一丨一一', '一丨𠃍丨丨一𡿨丿一', '丿丨𠃍一一丿㇆丶', '丿㇇丿㇆一一丨', '丿㇇𠃍丨一乚']
拼音： ['zhong', 'wen', 'xin', 'xi', 'chu', 'li', 'dang', 'zhong', '，', 'yu', 'yan', 'wai', 'bu', 'xing', 'shi', 'shang', 'de', 'te', 'zheng', 'zai', 'ge', 'ge', 'ren', 'wu', 'zhong', 'ban', 'yan', 'zhe', 'yue', 'lai', 'yue', 'zhong', 'yao', 'de', 'jue', 'se']
偏旁部首： ['丨', '文', '亻', '心', '夂', '王', '彐', '丨', '，', '讠', '言', '夕', '阝', '彡', '弋', '一', '白', '牜', '彳', '土', '口', '人', '亻', '力', '丨', '扌', '氵', '目', '走', '木', '走', '里', '覀', '白', '角', '色']

```


## SimilarityCompute

https://github.com/darr/sentence_similarity

Sentence Similarity compute based on cilin, hownet, simhash, wordvector,vsm models，  
基于同义词词林，知网，指纹，字词向量，向量空间模型的句子相似度计算。  

### results

```shell
sentence1:南昌是江西省的省会
sentence2:北京乃中国之首都
cilin 0.9
hownet 0.7857142857142857
simhash 0.46875
simtoken 0.4715704505415333
simvsm 0.0


sentence1:我是中国人，我深爱着我的祖国
sentence2:中国是我的母亲，我热爱她
cilin 0.8375
hownet 0.8068181818181819
simhash 0.734375
simtoken 0.8240455276180504
simvsm 0.7126966450997984


sentence1:一群高贵气质的差人在处罚违章动物
sentence2:城管执法，若不文明会导致很多不公平事故
cilin 0.6363636363636362
hownet 0.36916208791208793
simhash 0.53125
simtoken 0.20195795723403823
simvsm 0.0


sentence1:小明去了姥姥家，姥姥给他买了一本童话书
sentence2:我外婆早早的就出去了，给我带回来一本恐怖小说
cilin 0.7000000000000001
hownet 0.4841269841269841
simhash 0.53125
simtoken 0.5974486426178804
simvsm 0.16903085094570325
```

## law crime mining

https://github.com/darr/law_crime

Law Crime Mining Based on Corpus build and content analysis by NLP methods.
基于领域语料库构建与NLP方法的裁判文书与犯罪案例文本挖掘项目

### 基于刑法的因果字典抽取

根据中国人民刑法，对其进行因果处理，形成crime_name, cause, crime三个字段的抽取，形成量刑的基础,示例如下：

    {
    'crime_name': ['故意伤害罪', '组织出卖人体器官罪'],
    'cause': ['故意伤害他人身体的'],
    'crime': '三年以下有期徒刑、拘役或者管制'
    }
    {
    'crime_name': ['故意伤害罪', '组织出卖人体器官罪'], 
    'cause': ['致人死亡或者以特别残忍手段致人重伤造成严重残疾的'], 
    'crime': '十年以上有期徒刑、无期徒刑或者死刑'
    }
    {
    'crime_name': ['过失致人重伤罪'],
    'cause': ['过失伤害他人致人重伤的'],
    'crime': '三年以下有期徒刑或者拘役'
    }
    {
    'crime_name': ['强奸罪'], 
    'cause': ['以暴力、胁迫或者其他手段强奸妇女的'],
    'crime': '三年以上十年以下有期徒刑'
    }
    {
    'crime_name': ['强制猥亵、侮辱罪、猥亵儿童罪'],
    'cause': ['以暴力、胁迫或者其他方法强制猥亵他人或者侮辱妇女的'], 
    'crime': '五年以下有期徒刑或者拘役'
    }
    {
    'crime_name': ['非法拘禁罪'], 
    'cause': ['非法拘禁他人或者以其他方法非法剥夺他人人身自由的'], 
    'crime': '三年以下有期徒刑、拘役、管制或者剥夺政治权利'
    }
    {
    'crime_name': ['非法拘禁罪'], 
    'cause': ['致人死亡的'], 
    'crime': '十年以上有期徒刑'
    }
    
    
## causal knowledge base

https://github.com/darr/causal_collocation

causal knowledge base including causal pairs extracted from web text using the methods like PMI, Collocation。 
基于网络文本的因果知识库项目，采用PMI，搭配抽取等方法，形成因果对频繁集。  

### 项目运行结果

1、搭配文件：pmi_word有3项内容构成，分别为结果词，结果词性以及结果词语原因词之间的pmi值，用于衡量两者之间关联强度。  

	{ "_id" : ObjectId("5cbd878b831b975b8da3d6cc"), 
	"word" : "自杀", 
	"word_tag" : "v",
	"pmi_words" : [
	[ "留医", "v", 21.868029795027585 ], 
	[ "苦闷", "a", 19.546101700140223 ], 
	[ "干什么", "v", 19.28306729430643 ],
	[ "杨进", "v", 19.28306729430643 ], 
	[ "掀开", "v", 19.259220552352062 ],
	[ "抒发", "v", 18.546101700140223 ], 
	[ "口诛笔伐", "i", 18.365529454498404 ],
	[ "同情", "v", 18.28306729430643 ], 
	[ "抢救", "v", 18.115467345810362 ], 
	[ "思索", "v", 17.898403444071104 ], 
	[ "减肥", "v", 17.67163258222408 ], 
	[ "想起", "v", 17.452992295748743 ], 
	[ "赞扬", "v", 17.28306729430643 ]  }

2、因果搭配举例：

| 原因词 | 结果词 |
| :--- | :---: |
| 熬夜_v| 昏倒_v;交感_v;干涩_a;脱发_v;提神_v;上火_v;超负荷_b;泌尿_v;发烧_v;有心_v;猝死_v;发作_v;睡眠_v;慢性_b;不适_a;脱落_v;诱发_v;急性_b;点燃_v;困扰_v;比赛_v;突发_v;不好_a;感染_v;预防_v;调试_v;造成_v;消耗_v;到位_v;赚钱_v;容易_a;推广_v;健康_a;及时_a;准备_v;处于_v;成为_v;严重_a;工作_v;可以_v;达到_v;出现_v;减少_v;影响_v;存在_v |
| 出轨_v| 失恋_v;召唤_v;停播_v;原谅_v;出轨_v;笼络_v;非常_b;起火_v;不知_v;叫停_v;厉害_a;紧急_a;攻击_v;爆炸_v;受伤_v;比如_v;知道_v;造成_v;制定_v;影视_b;担心_v;生活_v;死亡_v;有利于_v;设计_v;一般_a;合作_v;选择_v;没有_v;维持_v;下降_v;反弹_v;面临_v;可以_v |
| 恋爱_v| 叹老_v;谈婚_v;论嫁_v;求婚_v;恋爱_v;浪漫_a;打断_v;聊天_v;结婚_v;诱导_v;谈话_v;掌控_v;认真_a;拍摄_v;为由_v;感染_v;吸收_v;下去_v;上网_v;可谓_v;出来_v;担心_v;涌入_v;庞大_a;就是_v;下来_v;放松_v;赚钱_v;鼓励_v;采取_v;私募_v;影视_b;创业_v;失败_v;应该_v;所有_b;发生_v;开始_v;需要_v;获得_v;投资_v |
| 挫败_v| 怒斥_v;迷惘_a;渺茫_a;无情_a;出击_v;煎熬_v;简易_a;源于_v;渴望_v;择机_v;自杀_v;阻碍_v;旅行_v;做好_v;付费_v;中小_b;兴起_v;感到_v;爆炸_v;紧急_a;巩固_v;挂牌_v;打破_v;获取_v;主动_a;垄断_v;并购_v;采取_v;成功_a;民营_b;面临_v;准备_v;开始_v;迅速_a;下行_v;亏损_v;调整_v;达到_v;提高_v |
| 沉迷_v| 挂科_v;有的视_v;自闭_v;会考_v;斥骂_v;威逼_v;冷漠_a;劝退_v;利诱_v;惨败_v;找上门_v;及格_v;牵动_v;消解_v;沉迷_v;赌博_v;象征_v;疲劳_a;网游_v;批评_v;耽误_v;炒股_v;思考_v;虚拟_v;危险_a;学习_v;遭到_v;娱乐_v;联系_v;真实_a;面对_v;分享_v;大额_b;防止_v;教育_v;担忧_v;全面_a;缺乏_v;丧失_v;安全_a;炒作_v;贸易_v;转移_v;陷入_v;健康_a;巨大_a;连续_a;造成_v;保证_v;可能_v;损失_v;保持_v;带来_v;调整_v;亏损_v;出现_v;存在_v;持续_v;经营_v;下降_v |
| 肥胖_a| 顺手作_v;返流_v;发胖_v;肥胖_a;补脑_v;摄取_v;疼痛_a;减肥_v;常见_a;沦为_v;慢性_b;临床_v;治疗_v;危害_v;发达国家_i;集聚_v;诊断_v;运动_v;迫切_a;蔓延_v;培养_v;现有_v;限制_v;改善_v;增多_v;一定_b;体现_v;研究_v;配套_v;容易_a;有利于_v;一般_a;健康_a;迅速_a;高于_v;带来_v;导致_v;达到_v;需要_v;管理_v;发生_v;减少_v;出现_v |
| 赌博_v| 妻离子散_i;涉恶_v;反赌_v;金立_v;参赌_v;赌博_v;清查_v;失范_v;涉黑_v;沉迷_v;贱卖_v;自杀_v;贪污_v;抹黑_v;受贿_v;不能自拔_i;洗钱_v;快乐_a;散发_v;乃是_v;屹立_v;逃税_v;斩断_v;离婚_v;并入_v;好像_v;拖欠_v;不知不觉_i;外出_v;整治_v;企图_v;滋生_v;对赌_v;暴富_v;犯罪_v;侦查_v;不明_v;破灭_v;稀释_v;最高_a;发动_v;禁止_v;合伙_v;在于_v;流向_v;意味着_v;带有_v;削弱_v;混乱_a;失去_v;扶贫_v;破产_v;主动_a;证券化_v;必要_a;崛起_v;走向_v;遭到_v;涉及_v;断裂_v;遵循_v;来临_v;立案_v;缓解_v;疯狂_a;从事_v;连续_a;失败_v;开放_v;规避_v;损害_v;监测_v;充满_v;倾向_v;约定_v;想象_v;出来_v;合法_a;可能_v;加大_v;困难_a;享受_v;民事_b;明确_a;保障_v;萎缩_v;监管_v;下跌_v;陷入_v;签订_v;极大_a;期待_v;达到_v;严重_a;稳定_a;出现_v;可以_v;形成_v;获得_v;吸引_v |
| 打架_v| 挑事_v;调皮_a;抢客_v;指向_v;同一个_b;罢工_v;头疼_a;误解_v;实属_v;热闹_a;扰乱_v;同样_b;批评_v;罕见_a;超预期_b;把握_v;合并_v;围绕_v;冲突_v;绝对_a;基本_a;矛盾_a;面对_v;争夺_v;剧烈_a;制定_v;国产_b;监管_v;担心_v;强烈_a;属于_v;控制_v;约定_v;损失_v;无法_v;存在_v;持续_v;出现_v |
| 抢劫_v| 春假_v;闲逛_v;身故_v;抢劫_v;逮捕_v;作案_v;谋利_v;取现_v;诈骗_v;非正常_b;追究_v;死亡_v;还是_v;出去_v;知道_v;频繁_a;遭遇_v;缺乏_v;严重_a;不同_a;带来_v;造成_v;损失_v |
| 枪击_v| 发誓_v;不幸_a;丧生_v;遇难_v;返回_v;恐慌_a;受伤_v;死亡_v;消退_v;伤亡_v;前往_v;损坏_v;犯罪_v;爆炸_v;参加_v;冲突_v;延误_v;修改_v;倾向_v;执行_v;凸显_v;彻底_a;担心_v;帮助_v;能否_v;受损_v;上升_v;取消_v;受到_v;重大_a;回落_v;进入_v;完成_v;明显_a |
| 强奸_v| 刑拘_v;抢劫_v;命名_v;身亡_v;对待_v;撤销_v;尴尬_a;真正_b;频繁_a;遭遇_v;处罚_v;研发_v;受到_v |
| 贪污_v| 违纪_v;毁谤_v;撤职_v;非同寻常_i;走后门_i;无助_a;调离_v;虾夷_v;降职_v;揭发_v;检控_v;公诉_v;亏空_v;无辜_a;违法_v;空穴来风_i;渎职_v;岌岌可危_i;受贿_v;露出_v;指控_v;舞弊_v;掏空_v;造成_v;犯罪_v;民办_b;反腐_v;举报_v;严厉_a;困难重重_i;抵抗_v;查询_v;腐败_a;巨额_b;挪用_v;代表_v;涉案_v;报道_v;撤销_v;叫停_v;筹措_v;倾斜_v;实践_v;垄断_v;低下_a;临时_b;混改_v;关键_a;思考_v;教育_v;普通_a;查封_v;愿意_v;库存_v;公共_b;自主_v;调查_v;中小_b;变更_v;解决_v;输送_v;流失_v;遭到_v;国有_v;并非_v;上市_v;要求_v;对外_v;购买_v;不及_v;获利_v;严重_a;处罚_v;积极_a;重视_v;亏损_v;负面_b;全面_a;建设_v;监管_v;改革_v;研发_v;构成_v;加大_v;工作_v;竞争_v;成为_v;减少_v;重大_a;影响_v;出现_v;一定_b;存在_v;下降_v |
| 增持_v| 汇金_i;反跌_v;增次_v;定投式_b;寿持_v;续增_v;举牌股_v;持工_v;阿合计_v;五牛亥尊_i;停手_v;知晓其_v;如愿以偿_i;领薪_v;尽心_a;走好_v;安邦系_v;牵强_i;狂风暴雨_i;富立_v;监发_v;拔葱_v;张开_v;吃官司_v;凸匹_v;挤出_v;遭疑_v;居首_v;追货_v;高歌猛进_v;围剿_v;炒新_v;悬疑_v;免予_v;让位_v;形不成_v;初始投资_v;雄起_v;保发_v;黯然失色_i;谋取_v;保增_v;消停_v;染指_v;增持_v;征询_v;邀约_v;久违_v;在任_v;详式_b;迷信_v;匪夷所思_i;分布_v;狙击_v;吐槽_v;可想而知_i;更胜一筹_i;添砖加瓦_i;欧债_v;紧逼_v;跌动_v;跃居_v;易主_v;潜水_v;留任_v;改正_v;斥资_v;普涨_v;力保_v;纾解_v;抽资_v;嘲讽_v;稳定_v;捍卫_v;限定_v;议论_v;开山_v;等值_v;出于_v;坐实_v;更替_v;平息_v;托底_a;力挺_v;浮盈_v;好奇_a;自救_v;强平_v;首创_v;拟以_v;井喷_v;掩护_v;趋同_v;责令_v;顺延_v;实施_v;稳住_v;典型_a;热捧_v;濒临_v |


# qa_on_military_kg

https://github.com/darr/qa_on_military_kg

QaSystem based on military knowledge graph that stores in mongodb which is different from the previous one,  
基于mongodb存储的军事领域知识图谱问答项目，  
包括飞行器、太空装备等8大类，100余小类，共计5800项的军事武器知识库，  
该项目不使用图数据库进行存储，通过jieba进行问句解析，问句实体项识别，  
基于查询模板完成多类问题的查询，主要是提供一种工业界的问答思想。  

# results
```shell
问题：中国有几艘航母:
共找到1个答案， 下面是具体明细：
['辽宁舰名称:辽宁舰']


属性值问答－－单实体单属性问答：
问题：神舟五号的长度是多少?:
共找到1个答案， 下面是具体明细：
['神舟五号长度:8.86']


属性值问答－－单实体多属性问答：
问题：神舟五号的长度以及运载火箭是多少？:
共找到1个答案， 下面是具体明细：
['神舟五号长度:8.86', '神舟五号运载火箭:长征2号F（遥五）']


属性值问答－－多实体单属性问答：
问题：神舟五号的长度以及神舟十号的长度是多少？:
共找到2个答案， 下面是具体明细：
['神舟五号长度:8.86']
['神舟十号长度:23.0']


属性值问答－－多实体多属性问答：
问题：神舟五号的长度,运载火箭以及辽宁舰艇的舰长分别为多少是多少？:
共找到2个答案， 下面是具体明细：
['神舟五号长度:8.86', '神舟五号运载火箭:长征2号F（遥五）']
['辽宁舰舰长:304.5']


属性区间值筛选问答－－单属性区间问答：
问题：最大飞行速度大于2500公里的战斗机？:
共找到16个答案， 下面是具体明细：
['麦克唐纳F-15E“打击鹰” 双座双发打击战斗机最大飞行速度:2654000.0']
['F-15A-D“鹰”最大飞行速度:2685000.0']
['F-22“猛禽”战斗机最大飞行速度:2570000.0']
['米格-29“支点”战斗机最大飞行速度:2817000.0']
['苏-24“击剑手”战斗轰炸机最大飞行速度:2670000.0']
['歼-15战斗机最大飞行速度:2940000.0']
['歼-11BS战斗机 最大飞行速度:2876000.0']
['歼-11B战斗机 最大飞行速度:2879000.0']
['米格-31战斗机最大飞行速度:3255000.0']
['苏-47金雕式战斗机最大飞行速度:2600000.0']
['F-15SE沉默鹰式战斗机最大飞行速度:2650000.0']
['XF-103战斗机最大飞行速度:3376000.0']
['米格-1.44战斗机最大飞行速度:3185000.0']
['YF-23战斗机最大飞行速度:2655000.0']
['XF-108轻剑战斗机最大飞行速度:3190000.0']
['YF-12战斗机最大飞行速度:3661000.0']


属性区间值筛选问答－－单属性多区间问答：
问题：服役时间在1950年之后2000年之前的轰炸机？:
共找到17个答案， 下面是具体明细：
['A3D/A-3“空中战士”服役时间:19560101']
['图-22M“逆火 MRA轰炸机和电子战飞机服役时间:19720101']
['图-95/图-142“熊” 远程轰炸机和海上侦察攻击机服役时间:19520101']
['B-52H远程轰炸机服役时间:19550101']
['B/RB-47“同温层喷射”服役时间:19510601']
['西飞轰-6中型轰炸机服役时间:19690201']
['图-160“海盗旗” 远程轰炸机服役时间:19870101']
['“堪培拉” 轰炸机/入侵飞机/侦察机服役时间:19510101']
['F/FB/EF-111战斗轰炸机服役时间:19670718']
['B-57“堪培拉”服役时间:19540101']
['B-2“幽灵” 战略轰炸机服役时间:19970401']
['B-1B“枪骑兵”服役时间:19880701']
['B-58“盗贼”服役时间:19600315']
['“胜利者”中程战略轰略机服役时间:19620101']
['“火神”轰炸机服役时间:19560101']
['幻影IV轰炸机服役时间:19790101']
['苏-7/装配匠-A战斗轰炸机服役时间:19590101']


属性区间值筛选问答－－多属性多区间问答：
问题：服役时间在1950年之后2000年之前且最大航程大于5000千米的运输机？:
共找到0个答案， 下面是具体明细：


属性区间值筛选问答－－单实体属性最值问答：
问题：长度最长的宇宙飞船:
共找到1个答案， 下面是具体明细：
['神舟十号名称:神舟十号', '神舟十号长度:23.0']


属性区间值筛选问答－－单实体属性最值问答：
问题：最大航程最大的运输机:
共找到1个答案， 下面是具体明细：
['安-225梦想式运输机名称:安-225梦想式运输机', '安-225梦想式运输机最大航程:15400000.0']

## histroy hot event base

https://github.com/darr/histroy_hot_event_base

history hot event projrct ,which concentrate on the dayily hot event covers the time range from 2004 to 2019, 16 years in total，
从2004年至2019年共16年的每日热点事件项目，
目标包括构建起从2004年至今共16年的历时热点标题数据库，构建16年历时事件热点知识库。


# doc sentiment analysis

https://github.com/darr/doc_sentiment_analysis

Syntax and Ruler-based Doc sentiment analysis,   
基于依存句法及词性模板篇章级情感计算。  
篇章级情感分析与短文本情感分析不同，而目前对篇章级情感分析的需求很大，  
对海量文本进行篇章情绪分析， 可以辅助各项决策，  
如行业文本情感分析，可直接辅助相关行业的情绪监测，并辅助建模．  
由于篇章级情绪与其余短文本级的情感分析有较大差异，基于学习的情感分析算法又受限于标注语料，  
因此，基于领域情感词典与依存句法规则的情感分析方法情绪分析上也就成了一种候选方案．  

# results

```shell

    央视新闻客户端3月9日消息，当地时间3月8日凌晨1时许，中国水电15局位于马里中部距离首都巴马科700公里处的项目工地现场及营地遭遇大约25至30名不明身份武装人员袭击。吊车、皮卡车、发电机等施工设备和物资均被烧毁；中方人员安全无伤亡，但随身手机、电脑等物品全部被抢。该项目组正在封闭工地并开始撤离。中国驻马里大使馆通报各驻马里中资企业定期排查隐患，采取安保措施，制定应急预案，切实加强防范，必要时考虑暂时撤离危险地区。
    
-0.31560200428208945

    华盛顿时间2018年3月1日，美国总统特朗普宣布，由于进口钢铁和铝产品严重损害了美国内产业，威胁到美国家安全，为重振美国钢铁和铝产业，决定将对所有来源的进口钢铁和铝产品全面征税，税率分别为25%和10%。商务部贸易救济局局长王贺军就此发表谈话。
    王贺军表示，美国进口的钢铁和铝产品大多是民用的中低端产品，并未损害美国国家安全。美国以国家安全为由限制钢铁和铝产品的国际贸易，是对以世贸组织为代表的多边贸易体制的严重破坏，必将对正常的国际贸易秩序造成重大冲击。美方可能出台的措施已经受到欧盟、加拿大、巴西、韩国等国家和地区的反对，美国内多个行业协会也对此表达了不满。
    
0.568083607707761

    最近几天，网上流传着一段高铁吃泡面的视频：一名男子在高铁上吃泡面，被一名女子怒怼。视频中的女子怒吼“整个高铁都知道不能吃泡面”，情绪激动，且言辞激烈。这段视频引起了网友的讨论，有人认为这位女子素质太差，也有人认为高铁上吃泡面，味道确实让人反感。
　　扬子晚报紫牛新闻记者辗转联系上视频中发飙的女子，她称因孩子对泡面过敏，曾跟这名男子沟通过，但对方执意不听，她这才发泄不满。记者无法联系上被怼的吃泡面男子
    
-0.7699229015082449

    北京昌平警方5月9日晚通报称，雷洋“因涉嫌嫖娼”被警车带往派出所的途中突发心脏病身亡。
雷洋家属向财新记者证实雷洋去世的消息，但对警方所称死亡原因、死者手机里位置信息被删以及警方在死者身亡两小时后才通知家属、拒绝家属对遗体拍照留存等做法表示质疑。目前北京市昌平区检察院已介入调查。
5月9日21时24分，北京市公安局昌平分局官方微博@平安昌平通报此事，称“5月7日20时许，昌平警方接群众举报称：位于昌平区霍营街道某小区一家足疗店内存在卖淫嫖娼问题。接警后，警方依法迅速开展查处工作。当晚，在该足疗店查获涉嫌卖淫嫖娼人员六名。期间，民警将涉嫌嫖娼的男子雷某（29岁，本市人）带回审查时，该人抗拒执法并企图逃跑，警方依法对该人采取了强制约束措施。在将该人带回公安机关审查过程中，该人突然身体不适，警方立即将其送往医院，后经医院抢救无效死亡”。
北京昌平警方称，昌平公安分局已将此情况通报检察机关，昌平区检察院已介入并开展侦查监督工作。目前，此次抓获的其他五人因涉嫌协助组织卖淫罪被昌平警方依法采取刑事强制措施。警方仍在进一步工作中。
得知这一通报后，雷洋之兄雷鹏向财新记者表示，雷洋家属对通报中的内容不认可，期待检察院的进一步调查结果。
雷鹏告诉财新记者，他于事发当晚得知这一消息。他介绍，在不久前的4月24日，弟弟雷洋喜得一女，尚未满月。雷洋的同学得知消息后，拟写了一份《关于人民大学雷洋同学意外身亡的情况说明》，雷鹏称这份情况说明是同学根据雷洋妻子口述完成的，“内容属实”。
这份情况说明显示，2016年5月7日，由于雷洋夫妇刚得一女，其亲属欲来京探望，航班预计当晚到达时间23点30分到达。当晚21时左右，雷洋从家里出门去首都机场迎接亲属，之后雷洋便失去联系。
根据这份情况说明，据雷洋妻子回忆，从5月7日23时30分至5月8日凌晨1点，她和亲属不间断打给雷洋电话，但手机一直处于无人接听状态。直到5月8日凌晨1点，电话有人接听，接听人自称来自昌平区东小口镇派出所，并告知亲属需要去派出所，亲属于1时30分左右到达派出所。
这份情况说明披露：“派出所告知的大意是：雷洋因涉嫌嫖娼，在警车带往派出所的途中因心脏病突发死亡。根据昌平区中西医结合医院给出信息，雷洋达到医院时间为2016年5月7日晚22点09分，到达时已经死亡。”
该情况说明还显示：5月8日凌晨4时30分左右，雷洋亲属随警察来到医院，见到雷洋手臂和头部都有明显淤血。警察给出的答复为路途中雷洋反抗强烈，跳车头部着地所致。亲属要求对遗体拍照留存被禁止。
针对警方较早时期的说法，雷洋家属及同学在该情况说明中提出四点质疑：其一、雷洋几乎每周都会踢足球，全年无休，其亲属也没有心脏病史，为何会突发心脏病？其二、雷洋手臂和头部的淤血，若为跳车所致，应有明显外伤。可据家属观察其无明显外伤，按照东小口镇派出所所述，执法后已被制服并招供，为何还会尝试并成功做到跳车？其三、医院给出的雷洋死亡时间为22点9分（达到医院时间），可是在之后长达近两个小时的时间，派出所为何不联系亲属，并且亲属一直打电话也无人接听？其四、亲属交涉后发现，雷洋手机中死亡前几日的通话记录，微信朋友圈里面关于孩子和家庭的信息，手机里面的位置记录都被部分删除，这是何人所为？
据这份情况说明披露，雷洋是湖南澧县人，系中国人民大学2005级环境学院的本科及硕士研究生，目前任职于中国循环经济协会。2012年毕业后，雷洋任职于中国循环经济协会，曾参与多个工业园规划，生态文明规划，污染物处理规划和循环经济规划的编制工作，在知名环境保护期刊《环境保护》《环境科学》《环境工程》上面都发表过论文，是中国环境保护事业中不可多得的青年才俊。
北京昌平警方通报中提到的“强制约束措施”，引起律师界人士的关注。接受财新记者采访时，上海市薛荣民律师事务所薛荣民律师介绍，所谓强制约束措施，一般是约束带或警绳，通俗讲就是把人绑了，防止失控；但是一般称保护性约束：“几人把你按住也能叫约束，多用于醉酒、吸毒及精神病人。”
浙江汉鼎律师事务所严华丰律师向财新记者介绍，强制约束措施，其实就是强行抓捕手段。这一警方自创的概念是相对保护性约束而言的，《治安管理处罚法》第十五条第二款规定，醉酒的人在醉酒状态中，对本人有危险或者对他人的人身、财产或者公共安全有威胁的，应当对其采取保护性措施约束至酒醒。“约束性保护”只能针对有危害性的无行为能力人或限制行为能力人，并且两个条件必须同时满足
    
-0.23620503299530443
提要：26岁产妇在陕西省榆林市第一医院绥德院区待产室生产期间坠楼身亡
-0.5370495669980353

    今天是个特别的日子京津城际铁路实施新的列车运行图复兴号动车组在京津城际铁路按时速350公里运行
5时30分数十名专门前来体验的火车迷齐聚北京南站候车大厅来自天津的老徐就是其中一员他昨天晚上从天津赶来为的就是乘坐首班车见证这一激动人心的时刻发车前，他们拿出自己珍藏的复兴号模型与“金凤凰”合影留念
6时02分随着C2581次列车驶出北京南站很多旅客的目光都聚焦在车厢内的显示屏上345、347、348……有人开始读数字在350闪现的瞬间整个车厢沸腾了一位车迷对身旁的小伙伴说“我突然有点想哭，太激动了”
复兴号在京津城际铁路按时速350公里运行，一是列车运行线路满足条件。今年以来，京津城际铁路的技术装备和基础设施得到全面强化，设备运行维护水平持续提升，外部环境整治成效明显。二是列车开行方案更加优化。针对京津城际铁路不同时期客流特点，中国铁路北京局集团有限公司科学合理调整列车开行方案，安排了高峰日、周一、周二至周四、周五、周六、周日等6张运行图，努力实现运力投放与客流需求精准匹配，满足日常、周末、小长假、春暑运等不同时期的旅客出行需求。
6时32分列车稳稳停靠在天津站来自天津机务段的首发车司机曹文普刚刚走出驾驶室马上就被旅客和火车迷包围大家争相和他合影留念并请他在这趟车的车票上签名
来自西南交通大学的耿昊然在微博上写道“今天你跑出了傲人的速度曾经的等待都不再是等待曾经的遥远也不再是遥远”10年前，9岁的耿昊然跟随父母来体验刚开通的京津城际铁路。如今，他已经成为一名电气工程专业的大学生，与高铁一同成长的他希望学成后能为中国高铁事业贡献自己的力量。文字：孙晓远 高李鹏图片：刘家豪编辑：孙晓远
    
0.6772238572854595
```

## abstact knowledge graph

https://github.com/darr/abstract_knowledge_graph

A systematic knowledge graph that concentrate on abstract thing including abstract entity and action.  
抽象知识图谱，目前规模50万，支持名词性实体、状态性描述、事件性动作进行抽象。  
目标于抽象知识，包括抽象实体，抽象动作，抽象事件。  
基于该知识图谱，可以进行不同层级的实体抽象和动作抽象，  
这与人类真实高度概括的认知是一致的。

### results

```shell
1. 名词抽象路径
爱情 抽象路径为： 爱情->柔->举止->特性->属性
爱情 抽象路径为： 爱情->爱情
爱情 抽象路径为： 爱情->爱
爱情 抽象路径为： 爱情->爱恋->喜欢->好态->态度->静态->事件->万物->实体
爱情 抽象路径为： 爱情->人际关系
爱情 抽象路径为： 爱情->良
爱情 抽象路径为： 爱情->情感->精神->万物->实体
爱情 抽象路径为： 爱情->亲密关系


女朋友 抽象路径为： 女朋友->人->动物->生物->物质->万物->实体
女朋友 抽象路径为： 女朋友->女->性别->特性->属性值
女朋友 抽象路径为： 女朋友->友


儿子 抽象路径为： 儿子->人->动物->生物->物质->万物->实体
儿子 抽象路径为： 儿子->家
儿子 抽象路径为： 儿子->男->性别->特性->属性
儿子 抽象路径为： 儿子->幼->年龄->特性->属性


老板 抽象路径为： 老板->人->动物->生物->物质->万物->实体
老板 抽象路径为： 老板->富->贫富->属性
老板 抽象路径为： 老板->商
老板 抽象路径为： 老板->女->性别->特性->属性值


狗 抽象路径为： 狗->狩猎犬
狗 抽象路径为： 狗->哺乳动物
狗 抽象路径为： 狗->宠物
狗 抽象路径为： 狗->玩赏犬
狗 抽象路径为： 狗->梗犬
狗 抽象路径为： 狗->走兽->动物->生物->物质->万物->实体
狗 抽象路径为： 狗->世界名犬
狗 抽象路径为： 狗->宠物狗
狗 抽象路径为： 狗->牲畜->动物->生物->物质->万物->实体
狗 抽象路径为： 狗->工作犬
狗 抽象路径为： 狗->狗品种
狗 抽象路径为： 狗->狗
狗 抽象路径为： 狗->枪猎犬
狗 抽象路径为： 狗->家庭犬


苹果 抽象路径为： 苹果->苹果
苹果 抽象路径为： 苹果->水果->植物->生物->物质->万物->实体
苹果 抽象路径为： 苹果->文字->语言->信息->精神->万物->实体
苹果 抽象路径为： 苹果->电脑硬件公司


梨 抽象路径为： 梨->水果->植物->生物->物质->万物->实体
梨 抽象路径为： 梨->仁果
梨 抽象路径为： 梨->梨
梨 抽象路径为： 梨->水果->植物->生物->物质->万物->实体


2. 状态词抽象路径
亢奋 抽象路径为： 亢奋->激动->情绪->静态->事件->万物->实体


悲伤 抽象路径为： 悲伤->惨->境况->属性
悲伤 抽象路径为： 悲伤->属性值
悲伤 抽象路径为： 悲伤->坏->好坏->特性->属性
悲伤 抽象路径为： 悲伤->味道->外观->属性
悲伤 抽象路径为： 悲伤->境况->属性
悲伤 抽象路径为： 悲伤->特性->属性
悲伤 抽象路径为： 悲伤->莠
悲伤 抽象路径为： 悲伤->不幸->衰变->变->物理状态->静态->事件->万物->实体
悲伤 抽象路径为： 悲伤->悲哀->情绪->静态->事件->万物->实体


开心 抽象路径为： 开心->属性值
开心 抽象路径为： 开心->激动->情绪->静态->事件->万物->实体
开心 抽象路径为： 开心->境况->属性
开心 抽象路径为： 开心->取悦->使喜悦->变情感->事件->万物->实体
开心 抽象路径为： 开心->喜悦->好情->情绪->静态->事件->万物->实体
开心 抽象路径为： 开心->取乐->使喜悦->变情感->事件->万物->实体
开心 抽象路径为： 开心->良
开心 抽象路径为： 开心->福->境况->属性
开心 抽象路径为： 开心->愿意->意向->静态->事件->万物->实体


3. 动作抽象路径
吹牛 抽象路径为： 吹牛->夸大->表示->使他人感知->事件->万物->实体


吃饭 抽象路径为： 吃饭->吃->摄取->代谢->变常态->变本体->事件->万物->实体
吃饭 抽象路径为： 吃饭->摄取->代谢->变常态->变本体->事件->万物->实体
吃饭 抽象路径为： 吃饭->活着->常态->物理状态->静态->事件->万物->实体
吃饭 抽象路径为： 吃饭->事情->事件->万物->实体


睡觉 抽象路径为： 睡觉->睡->停做->泛动->事件->万物->实体


打牌 抽象路径为： 打牌->娱乐->消闲->变常态->变本体->事件->万物->实体


斗殴 抽象路径为： 斗殴->颤动->定位自移->自移->变空间位置->变关系->事件->万物->实体
斗殴 抽象路径为： 斗殴->争斗->较量->变莠态->变本体->事件->万物->实体
斗殴 抽象路径为： 斗殴->开始->泛动->事件->万物->实体
斗殴 抽象路径为： 斗殴->单位


杀人 抽象路径为： 杀人->杀害->变莠态->变本体->事件->万物->实体
杀人 抽象路径为： 杀人->能->能力->特性->属性值
杀人 抽象路径为： 杀人->属性值
杀人 抽象路径为： 杀人->能力->特性->属性值
杀人 抽象路径为： 杀人->罪


诬陷 抽象路径为： 诬陷->损害->变莠态->变本体->事件->万物->实体
诬陷 抽象路径为： 诬陷->文字->语言->信息->精神->万物->实体
诬陷 抽象路径为： 诬陷->语文->语言->信息->精神->万物->实体
诬陷 抽象路径为： 诬陷->诽谤->贬低->变特性->变本体->事件->万物->实体
诬陷 抽象路径为： 诬陷->莠
诬陷 抽象路径为： 诬陷->伪造->创造->使存现->变本体->事件->万物->实体


打击 抽象路径为： 打击->攻打->变莠态->变本体->事件->万物->实体
打击 抽象路径为： 打击->激怒->变情感->事件->万物->实体
打击 抽象路径为： 打击->打->变形状->变外观->变本体->事件->万物->实体


制裁 抽象路径为： 制裁->用具->器具->无生物->物质->万物->实体
制裁 抽象路径为： 制裁->处罚->变莠态->变本体->事件->万物->实体
制裁 抽象路径为： 制裁->军
制裁 抽象路径为： 制裁->制度->规矩->精神->万物->实体
制裁 抽象路径为： 制裁->阻止->阻动->使之动->事件->万物->实体
制裁 抽象路径为： 制裁->制止->阻动->使之动->事件->万物->实体


4. 其他
离 抽象路径为： 离->退出->变包含->变关系->事件->万物->实体
离 抽象路径为： 离->不同->相比关系->关系->静态->事件->万物->实体
离 抽象路径为： 离->掉下->下去->方向性自移->自移->变空间位置->变关系->事件->万物->实体
离 抽象路径为： 离->分离->变关联->变关系->事件->万物->实体
离 抽象路径为： 离->离开->方向性自移->自移->变空间位置->变关系->事件->万物->实体
离 抽象路径为： 离->消失->物理状态->静态->事件->万物->实体
离 抽象路径为： 离->脱离->变关联->变关系->事件->万物->实体
离 抽象路径为： 离->相距->时空关系->关系->静态->事件->万物->实体


乎 抽象路径为： 乎->词语->语言->信息->精神->万物->实体
乎 抽象路径为： 乎->属性值
乎 抽象路径为： 乎->宗教
乎 抽象路径为： 乎->疑问
乎 抽象路径为： 乎->举止->特性->属性
乎 抽象路径为： 乎->文字->语言->信息->精神->万物->实体
乎 抽象路径为： 乎->回绝->示不同意->表示情感->事件->万物->实体
乎 抽象路径为： 乎->恶->举止->特性->属性
乎 抽象路径为： 乎->洗涤->使净->变外观->变本体->事件->万物->实体
乎 抽象路径为： 乎->材料->无生物->物质->万物->实体
乎 抽象路径为： 乎->莠
乎 抽象路径为： 乎->正确->正误->特性->属性值
乎 抽象路径为： 乎->声->天然物->无生物->物质->万物->实体
乎 抽象路径为： 乎->良
乎 抽象路径为： 乎->正误->特性->属性
乎 抽象路径为： 乎->也

```


## event predict based on eeg

https://github.com/darr/event_predict_based_on_eeg

future event predict demo based on causal event graph that covers the full industries  
that can predict the benefits or bad effects in accordance with the event given by the user,  

基于因果事理图谱的事件预测。

### results

```shell
事件：下雪
有利影响:
蔬菜价格大幅上涨
电石出场价格小幅上涨
钢铁企业废钢采购价格多调整为主
青椒白萝卜价格上涨
北京蔬菜价格大幅上涨
港口粮价上涨
煤价具有继续上涨动力
电石运输成本加大
不利影响:
航班预定下降
港玉米成交再度转淡
中国钢铁需求减弱
焦煤库存显著下降
汽运煤运输困难
市场成交状况较为低迷


事件：感冒
有利影响:
盘中一步反弹
心衰重要
耳压增加
细菌繁殖速度加快
效果不错
假阳性结果
炎症致密实变
不利影响:
患者头痛乏力发热
人体免疫力弱免疫力下降
老年人丧命原因
心脏衰竭
并发症重症死亡几率
患者死亡


事件：心情郁闷
有利影响:
1月自杀率反弹
加重牛皮癣重要
冲脉出现气滞血瘀
交通安全
不利影响:
内分泌失调
病情进一步恶化


事件：孟晚舟事件
不利影响:
美股补跌


事件：孟晚舟被捕
不利影响:
全球市场动荡
国内舆论震动


事件：吃得好
sorry，目前还预测不出来.


事件：吃得不好
不利影响:
整个精力不好


事件：雷雨天气
有利影响:
土豆价格大涨
市场预期较高
影响航班正常首要
不利影响:
航班延误
人力物力财力不足
应停止动火作业
玉米病虫害面积发生
牛蛙病害产生
池水中黄鳝感到不适
交通事故高发
小麦质量等级较下降
报价继续下滑
贸易商出货困难
体内水分流失
蔬菜产量减少
市场采购需求始终维持较低水平
气温偏低
火888灾危险
火灾危险


事件：马云辞职
有利影响:
股市欧元公债收益率攀升
现货黄金早盘一度冲高
市场避险情绪再度爆棚提振白银走高
公司实际控制人变更
不利影响:
公司董事人数不足
金融市场逆转走势
市场一片不安
油价盘中下挫
意大利最古老银行股票开盘即跌


事件：特朗普和金正恩会晤
有利影响:
多种金属价格反弹
镍铅为首有色金属集体上涨
避险需要
不利影响:
美国朝鲜局势更为紧张


```
 
 # wenwen chatbot
 
https://github.com/darr/wenwen_chatbot
 
A chatbot that can be an expert on the common questions like why,how,when,who,what based on the online question-answer website，  
基于线上公开问答数据的知道类问答机器人，与检索方式不同，可以进行常规问题的问答，如为什么，怎么样，是什么等，  
基于该方式，可以作为问答机器人常识接口，也可以作为常识知识库构建 

# results

```shell
问题: 天为什么下雪
回答: ['太冷,', '气候所定', '因为“天”心痛', '怕人太热情了。冷却下。', '因为有降水，遇到冷空气，就变成了雪']

问题: 为什么下雪
回答: ['冬天并不是每个地方都下雪的。某些地方因气温在零下的温度时空中的水汽会变成雪晶然后落下。温度不够低时是不能产生雪的', '下雪是降水的一种形式，气象上称之为固体降水。在一种既有冰晶又有过冷水滴的云体里，这种云称为冰水混合云。在这种云体内，过冷水滴不断蒸发成水汽，水汽源源不断地涌向冰晶的表面，在那儿凝华落脚，使冰晶逐渐增大形成花。花形成后便向下飘落，在飘落的过程中，碰上其他花时，常常粘附在一起，慢慢长大，遇到上升气流时，小花上升的速度比大花快，小花赶上大花发生粘连，几经反复，便逐渐成为直径达几厘米的像棉花又似鹅毛的团。当空气中的上升气流再也托不住这些花时，它们便从云层中飘落下来，如果这时低层空气的温度在0℃以下，花降落到地面，这就是人们所见到的皑皑白。', '地面的水（海水、河水、湖水、江水等等）受阳光照射而蒸发成水蒸汽升腾至空中，由于高空温度较地面要低很多，有时甚至于低到零度以下。在低温的环境中，水蒸汽凝聚成小水滴。天空中的云就是由这些小水滴聚集而形成的。云层中的这些小水滴受空气运动的带动作用而互相碰撞，使自己的粒度变得越来越大。逐渐不断变大的水滴又由于低温的作用而结冰形成小冰珠（实际就是雪），小冰珠又互相碰撞或其外表不断凝聚空中的水蒸汽，使自己的体积不断增大，过大的冰珠由于过重，使上升气流也无法支持而向地面坠落，在坠落中冰珠由于空气磨擦而升温及地面夏季的高温作用渐渐融化成水滴--雨滴；如果冰珠过大（实际可称为“冰球”）在落到地面之前还来不及融化成雨水，落到地面的稍小一点的可以来得及融化就成了雨，稍大一点的来不及融化就只能仍是冰雹。在空中漂浮的看似柔如棉花的云朵里的气流始终是处于剧烈运动之中，这样剧烈运动促使云层不断地上下运动，形成犹如白蘑菇的浓厚云层（夏日多常见的一种云层）。由于这种云层所处位置很高的极低温的环境中，因此形成的冰球也就越大，落到地面还来不及融化成雨水。所以夏季多降冰雹。冬季由于地面温度较低落下的冰雪也无法在中途融化成雨，所以冬天只会下雪。', '在水云中，云滴都是小水滴。它们主要是靠继续凝结和互相碰撞并合而增大成为雨滴的。冰云是由微小的冰晶组成的。这些小冰晶在相互碰撞时，冰晶表面会增热而有些融化，并且会互相沾合又重新冻结起来。这样重复多次，冰晶便增大了。另外，在云内也有水汽，所以冰晶也能靠凝华继续增长。但是，冰云一般都很高，而且也不厚，在那里水汽不多，凝华增长很慢，相互碰撞的机会也不多，所以不能增长到很大而形成降水。即使引起了降水，也往往在下降途中被蒸发掉，很少能落到地面。最有利于云滴增长的是混合云。混合云是由小冰晶和过冷却水滴共同组成的。当一团空气对于冰晶说来已经达到饱和的时候，对于水滴说来却还没有达到饱和。这时云中的水汽向冰晶表面上凝华，而过冷却水滴却在蒸发，这时就产生了冰晶从过冷却水滴上“吸附”水汽的现象。在这种情况下，冰晶增长得很快。另外，过冷却水是很不稳定的。一碰它，它就要冻结起来。所以，在混合云里，当过冷却水滴和冰晶相碰撞的时候，就会冻结沾附在冰晶表面上，使它迅速增大。当小冰晶增大到能够克服空气的阻力和浮力时，便落到地面，这就是雪花。在初春和秋末，靠近地面的空气在0℃以上，但是这层空气不厚，温度也不很高，会使雪花没有来得及完全融化就落到了地面。这叫做降“湿雪”，或“雨雪并降”。这种现象在气象学里叫“雨夹雪”。']

问题: 中国没有大航海
回答: ['国家根本没这回事的想法', '因为中国没有西方的海盗文化。', '中国只是做点生意拜访邻居。别的国家这方面还不发达。外国发现新大陆带动了其他国家。争相开始发展吧', '西方的航海探险是为了获得海外的财富，满足统治者对金钱的渴望，而明朝时郑和下西洋是为了彰显大明朝的国威，注重的是朝贡贸易，是为了满足皇帝和后宫对异域珍宝的需要。主要目的不是为了对外扩张。', '你好！只要没有天灾人祸的话凭中国的地理位置完全可以养活百姓，自给自足。我们地大物博，只要皇帝需要，皇宫可以迁移天下任何地方。而西方列强不一样，他们的国土跟个厕所那么大，他们需要生存只能够征服别人，所以西方的交通发达，中国对大海，新陆地没有兴趣。如有疑问，请追问。']

问题: 为什么是西班牙发现新大陆
回答: ['点儿高', '努力,运气好', '因为有你在后面指路', '因为他生病时躺在床上看地图时候发现的', '欧洲人认为是新大陆，以前欧洲人不知道有美洲。']

问题: 新大陆
回答: ['美洲大陆', '所有的美洲国家', '南北美洲的国家', '哥发现的是北美西印度群岛，严格来说只是当时大陆的外围，继现在的，古巴，巴哈马，牙买加，还有一些岛国，忘了，', "国家。。。。。。。。。。。首都阿根廷。argentina。布宜诺斯艾利斯。Buenos。Aires。安提瓜和巴布达。antigua-barbuda。圣约翰。Saint。John's。巴巴多斯。barbados。布里奇敦。Bridgetown。玻利维亚。bolivia。苏克雷。Sucre。巴西。brazil。巴西利亚。Santiago。多米尼克。dominica。罗索。Roseau。厄瓜多尔。ecuador。基多。Quito。古巴共和国。guba。。。。。。。。。。。。。。。。。。。。。。。。。。。。。。。。评论0。。。。。。。。。。。。。。。。。。。。。。。。。。。。。。。。。0。。。。。。。。。。0。。。。。。。。。加载更多。。。。"]

问题: 为什么美洲文明消失了?
回答: ['产生了，然后被灭了。、。', '美洲的文明集中在中美洲，其他地方比较少', '我觉得主要原因还是因为美洲没有马据说美洲原本是有马但是被美洲原住民吃光了马匹在古代是很重要的东西无论是打仗还是运输和交流几乎都要用到的', '有文明啊，美洲文明的代表有玛雅文明，印加文明和阿兹特克文明。此外，奥尔梅克文明，瓦哈卡文明，特奥蒂瓦坎文明和托尔特克文明等在美洲发展史上也占有重要地位。不过，这些文明在葡萄牙，西班牙等殖民者的打击下基本都毁了，这些文明的历史和文字也在殖民者的大屠杀中最终失传，真是可惜啊', '美洲大陆与其他大陆隔大西洋、太平洋两大洋，这就使当地文明在航海技术落后的情况下缺乏与其他文明互动的可能。没有了这种文明交流，一个地方的文明发展就有局限性。这种情况不仅出现在美洲，包括大洋洲、撒哈拉以南非洲都由于地理原因导致的缺乏交流而与欧亚北非地区的文明产生巨大的落差。反观欧亚北非地区，自东往西存在中国、印度、波斯、中东、埃及、希腊、罗马、迦太基以及北方游牧民族等多种文明，这些文明充分互动交流，一种文明发达后，就将其先进元素传递给相邻地区，多次的这种互动导致这一地区的文明水平普遍高于其他地区。若反其道而行之，即使是发达的中国文明在闭关锁国后也很快落后于其他文明。可见文明间的交流对文明发展是极其重要的。']

问题: 草船借箭为什么不用火箭?
回答: ['射火箭是技术活好拨。那么多人射火箭。不小心把自己的东西烧了怎么办', '这个问题~你肯定知道答案~但是你还是来问了因为你觉得这样很好玩~好吧那我告诉你：别玩啦~', '当时大雾弥漫，根本看不清楚，事后才知道是草船，当时曹军哪知道是用草船借箭，还以为是孙刘联军来进攻呢。', '曹贼又不知道是草人！~知道了就不会放箭了！~再说！~没火也是可以杀人的！~干嘛脱裤子放屁——多此一举！·', '首先,当时曹军是仓促应战,而火箭在那时还属于高科技,不成熟,作战之前要准备.第二,火箭造价可不便宜啊,就算曹操当时很强,他也没有很多.第三,剧情不允许.第四,你要问罗贯中.']

问题: 为什么马能吃草?
回答: ['为了活命', '进化来的结果', '因为它妈妈吃草', '牛还吃草下奶呢', '身体结构的不同..', '存在就是有道理的。', '素食动物都大，食物来源多啊', '马吃草就。相当于。你要吃饭没什么可晕的', '马饿呗，草比较近。再看看别人怎么说的。', '因为长时间的自然生存，它们的牙齿和咀嚼力，还有盲肠的进化，使它们能在大自然中有一席生存之地！']

问题: 为什么人会死?
回答: ['自然规律', '生老病死自然法则', '身体技能老化,逐渐死亡', '因为人得细胞被慢慢的氧化……', '因为这是一种轮回,准备去投胎咯！', '生是为。了证明。死是为了。。解脱', '人呼吸的氧气在体内进行化学反应导致人的衰老。疾病也能让人毙命。', '因为遗传和领受的文化导致了死亡，现在明白神给予生命的话语能解决人的罪，从而得到生命', '正常死亡是因为人体内的部分细胞不能完成更新，导致机体的死亡。非正常死亡吗，那就原因太多了……', '老的实质是细胞新生速度大于衰退速度，如果还是小于的话，没有人会说老，是张大，到有一天只有细胞的衰败，不主义维持现有实体状态，就是死鸟']

问题: 为什么会得高血压?
回答: ['血压≥140/90mmhg即为高血压。不过需要在安静情况下、不在同一天测量3次以上才可以确认。。高血压病是多基因疾病，迄今已发现近百种基因可能与之有关。。高血压病具有明显的家族发病倾向。。肥胖是青少年高血压的重要病因之一。。某些个性特征诸如焦虑、恐惧、紧张、压抑等对青少年血压会产生影响。。此外，高盐饮食也是高血压的一个发病因素。', '高血压常被认为是成年人的病症，实际上儿童高血压并不少见。据报道，美国和日本儿童高血压发病率分别为14.1％和13.3％，我国北京儿童医院对5000名6～18岁儿童和青少年进行血压普查时，发现血压偏高者占9.36％，1979年广东省心血管病研究所，对3826名4～16岁农村儿童进行普查，按我国沿用的标准，高血压的患病率为0.86％，这个数字表明，在我国有数以万计的儿童高血压患者。。儿童高血压分为原发性高血压和继发性高血压两种。原发性高血压发病机理比较复杂，血压长高与多种因素有关。目前多数学者认为主要由下列因素引起。。（1）神经内分泌因素：小儿的大脑、中枢神经处于发育不完善时期，容易兴奋和疲劳，对于神经脆弱的獐来说，或受到家庭、学校、社会环境因素中的不良刺激，会使大脑皮质兴奋和抑制失衡，引起全身小动脉痉挛及周围阻力增加，导致血压升高。。（2）遗传因素也是高血压发病的一个重要因素。父母患有高血压病的子女发生高血压病的机会是父母无高血压病者的2倍。。（3）高糖、高脂饮食及营养过剩等引起的肥胖症。。儿童及青年高血压症状多不典型，与成人也不全相同。有的无症状，有的表现头痛、头晕、眼花、恶心呕吐，婴幼儿因不会说话，常表现烦躁不安，哭闹，易努，体重不增，发育停滞。此时应引起注意；此类病人多有高血压病家族史；如血压较高多为继发性高血压，应进一步查找原因；另外，此类病人并发症较少，一般不会发生脑卒中，心肌梗塞及肾功能不全。除药物治疗外，非药物治疗更为重要，应劝告其加强体力活动，维持理想体重，限制食盐摄入及禁烟等。。青年性高血压者的体育运动。有些18-21岁的青年,在体格检查时发现血压高,其中多数人属于非原发性高血压病,即青年性高血压。青年性高血压有下列特点：一、在发育期间出现，到20-21岁以后,血压就逐渐降至正常。血压的这种暂时性增高是由于发育时间某些内分泌腺功能亢进，交感神经兴奋性增高所引起的。二、多见于体格成长得很快、身高增长得迅速、性情较易兴奋激动的青少年。三、收缩压稍高，在130毫米汞柱以上,但不超过150毫米汞柱;舒张压不增高。四、本人没有自觉症状，只是在体格检查时由医生发现血压高；被检查者一向在参加体育运动后没有不适反应，有些人甚至运动成绩很好。。对于有青年性高血压的青年人，如果一向有体育运动基础，现仍参加一般运动，运动后无不适反应，那么，可照常运动，只是不宜参加举重和技巧运动，并要定期复查，观察血压变化。。对于有青年性高血压的运动员，一般允许继续参加运动训练，但要加强医务监督，定期检查身体，暂不宜参加足球、篮球、举重和器械体操等项运动，因为前两种运动能引起神经系统高度兴奋，后两种运动包括有鼓劲、闭气性质的练习，会加重血液循环的困难。如果上述四个项目的运动员患了青年性高血压，可以继续练习，但暂不宜参加大运动量训练']

问题: 为什么会得痔疮?
回答: ['根据你的病情描述图片显示考虑，环状混合痔。目前脱出伴便血考虑三度。注意饮食，避免辛辣食物，保持大便通畅。高锰酸钾温水坐浴，，可以继续运用达必康痔疮膏等。一般能够自己恢复，如果症状不缓解，建议肛肠科进一步就诊。。+', '痔疮是由于长期便秘或其他原因所致的直肠长时间受压导致局部静脉回流受阻。静脉曲张。管壁过度膨胀而形成痔疮。。。痔疮的治疗首先要保持大便通畅，进食易消化、少含渣滓的食物。饮食应粗细搭配，少饮浓茶、咖啡、酒类及少进辛辣食物，以减少对肛管的刺激。便后要温水坐浴，局部应用痔疮栓或痔疮膏。。', '痔疮，与不良的生活饮食习惯和便秘有关，如果不治疗，自己是不会恢复的.生活中我们吃的黑木耳还有治疗痔疮的功效，可以将木耳摘去污物，洗净，加水少许，文。火煮。成羹，每日服食指导意见：要注意饮食和休息，每天早上起床或早餐后养成定期蹲便的良好习惯以防便秘，。肛门局部用达必康，必要时用栓剂进行润滑以保护直肠黏膜便可。多做提肛、踢腿的动作可帮助恢复，如出现严重症状，如肿物脱出不能收回及出血量多等因及早就医', '分析：。轻微的痔疮，如果没有什么症状的可能没有什么大的危害，但是如果痔疮症状比较明显的，比如痔疮疼痛厉害的，同时伴有出血情况的，时间长了病人很痛苦，另外长期出血容易导致贫血。有的人痔疮不及时治疗，容易导致溃疡面形成肛裂，甚至肛瘘，这样就很危险了。建议：所以不管是什么病，建议还是及早治疗比较好，症状轻时可以先使用达必康有一定作用。不要等到严重了再治疗，一方面病人痛苦，另一方面治疗难度加大，费用加大。+', '1、与人类肛门的解剖结构有关：由于直肠上静脉及它的分支无静脉瓣，人类直立姿势，从而使地球吸引力能够对回流的血液形成向下的力，使肛门部静脉血管曲张、迂曲、增生，形成痔疮。。2、与工作性质有关：久坐、久站、久蹲工作的人多见。。3、与排便习惯有关：便无定时、如厕过久均能诱发痔疮。。4、与饮食习惯有关：嗜食辛辣刺激食物，如食辣椒、大量饮酒等。。5、与妊娠有关。妊娠中晚期因肛门直肠静脉充血加重，易发生痔。。6、与局部感染有关：如肠道感染、寄生虫等。']

问题: 降准以后会怎样
回答: ['人民币贬值，制造业库存太多，消费提振不起，做生意越来越难了。。。', '下周一主力又有逢高出货的机会了，大盘肯定会高开，之后将冲高回落。', '降息可以吸引贷款扩大投资，降准可以增加货币的流通量，都是为了搞活经济，利好股市和房地产。', '降准降息是宽松货币政策的举措，会导致市场中纸币增多，钱多了就不值钱了，所以物价会上涨。当然实际情况没有这么简单，降准降息多印钱会让物价上涨没错，但是央行选择降准降息多印钱的时机一般会选经济开始疲软，物价开始下降的时候，所以你单单看数据可能看不出来。', '此轮降准为定向降准，不是直接投放货币的政策，从目的来说还找不出会让物价上涨的必然关系！不过，切不可单纯的认为物价真能保持稳定。我们可以简单的说一下，假如国际石油、天然气等基础能源继续这样涨下去，而此时人民币又处于贬低状态，这对能源进口大国的中国来说完全就是双重利空，极有可能使我国物价重演输入性通货膨胀的悲剧！']

问题: 投资人投资意愿下降以后会怎样
回答: ['1.。行业投资增速蟹将，将会引起对该行业投资预期下降。2.。事实是最好的证据。', '设有一个群体。此时投资和存款获利均等，现在是银行利率上调，存款获利增加。选择投资的人肯定减少了，即投资意愿减低，他们选择投资是50%', '正确答案：d。解析：由语境可知，投资增速下降对经济增城速度的影响是很大，而且这种影响是负面的，后面的几个行业是例子，因此d选项“首当其冲”符合语境。“首当其冲”是指比喻最先受到攻击或遭遇灾害，常被人误用为首先接受任务，或首先应当做某事。故本题正确选项为d', '商家来说相当于是资金成本上涨了，会直接影响资金的投资欲望，进而转向稳健的理财计划，存款利率上涨了，如果利率上涨了，那么就可以对市场输送更多的资金，那么银行的钱就会多，那么对企业，那么来看存款利率和贷款利率首先你要明白利率对于资金的作用，存款肯定就会多，但是如果贷款利率上涨', '首先要明白。利率是什么。。利率是资金的价格。既你持有资金的成本举个简单的例子。现在银行的贷款利率是8%。。你能够贷到款。你有一个项目投资的回报率是10%现在你肯定愿意去投资，因为你可以赚取2%现在市场的利率上升了。假如银行的贷款利率是11%，而项目投资的回报率还是10%你现在肯定不会愿意贷款去投资了。那么投资就减少了']

问题: 为什么要有女朋友
回答: ['我靠不是吧', '生活就是这样。。。。你不谈女朋友，怎么有爱情的结晶。。。。那样会很寂寞的', '心中有喜欢的女孩，就和她聊天，她喜欢什么你就喜欢什么，天天和她在一起玩，时间长了就是女朋友了', '那是应该人家努力去追求得来的结果，其实每个人都可以拥有的。。。努力了就会有不努力就永远也不会有。。', '因为人家有钱。！有车。！有房。！有长相！。要着4条你都有！我不信你没女朋友！长相是次要的。关键还是带有钱！！男人有多好色！女人就有多爱财！！！！']

```

# word_cloud

https://github.com/darr/word_cloud

A toolbox or kit for image-shape adjusted word cloud based on plain text, local file or web articles,  
面向本地文件, 在线网页, 程序输入的字符云自动生成组件,支持用户自定义图片字符形状, 生成给定网页,文本的高频词和关键词词云.        

# 效果展示:
 
![image](https://github.com/darr/word_cloud/raw/master/results/mao-topwords.jpg)  

![image](https://github.com/darr/word_cloud/raw/master/results/mao-keywords.jpg)  

![image](https://github.com/darr/word_cloud/raw/master/results/huawei-topwords.jpg)  

![image](https://github.com/darr/word_cloud/raw/master/results/huawei-keywords.jpg)  

![image](https://github.com/darr/word_cloud/raw/master/results/jiangxi-topwords.jpg)  

![image](https://github.com/darr/word_cloud/raw/master/results/jiangxi-keywords.jpg)  



