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
