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

