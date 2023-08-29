![cover.jpeg](cover.jpeg)

# Carol

> 心理学家 Carol Dweck 做过一个实验，她找了一些十岁的孩子，随机分成两组，让他们做道题。
> 
> 之后，对第一组那些完成题目的孩子说：你真聪明。对第二组那些做得不错的孩子说：你真努力，你很认真。
> 
> 你应该感受不到其中的差别，没关系，我们接着说第二部分研究。接下来，她让两组孩子从两道题目中选一道去做，一道“很简单”，另一道“非常之困难”，“但是他们能够从中学到很多”。
> 
> 巨大的差别出现了：被夸聪明的第一组孩子，有五成选了简单的题目；被夸努力的第二组孩子，有九成选了非常之困难的题目。
> 
> 继续看第三部分的研究。
> 
> 她继续让两组孩子做一道非常难的题目，基本上可以说无法解答。“聪明”组几乎没坚持多久，非常沮丧，很快就放弃了；而“努力认真”组，坚持了很长时间，而且很享受这一过程，虽然最后也没能解开这道题，但他们很少有负面情绪。
> 
> 发现问题了吗？被夸奖“聪明”，只要做事的时候遇到困难，你就非常容易陷入自我怀疑和沮丧，立刻放弃；而被夸奖“努力认真”呢？
> 
> 重视努力让孩子拥有一个 TA 自己能掌控的变量，这会让他们认为自己能掌控自己的成功。
> 
> 而重视天赋，会让我们秉持固定型思维，认为聪明与否是无法改变的。我们不敢去尝试有难度的事情，因为如果失败了，就意味着我们是不聪明的。
>
> 与看重聪明的人相比，看重努力的人，更有可能实现自己的目标。这个研究表明，被夸奖聪明的孩子，遇到困难时容易沮丧，很快就会放弃；而被夸奖努力的孩子，能够坚持很长时间，并且享受解决问题的过程。
> 
> 如果不聪明，那就足够努力吧。
> 
> 引用自 @高冷冷

刻意练习很重要。这是一个简单的小工具，可以帮助你回顾自己上一次练习时什么时候，练习了多少次，该项目会不断增加新的练习题。练习题主要围绕 Gopher，你也可以构建自己的题库。

## 使用步骤

1) 克隆项目
2) 完成一个练习题
3) 在 `exercise_book.md` 中记录完成的题目
4) 可以移除自己这次练习的代码，方便下一次练习，也可以保存
5) 在项目根目录执行 `$ go run cmd/carol.go`，查看练习题统计信息，预览如下

```shell
Name                        Last done   Done  Level   Topics
----                        ---------   ----  -----   ------
data_structure/linked_list  1 day ago     1x  medium  数据结构
data_structure/stack        1 day ago     1x  medium  数据结构
----                                    ----
2                                          2
```

## 题库
| 分支 | 题库名 | 更新时间 |
| ---- | ------ | ------- |
| main | Go  | 2023-08-29   |

## 贡献
欢迎任何人提供自己的练习题库。你可以 `fork` 本仓库，创建新的分支，分支命名建议以某个职位、领域，例如 C++、Docker 等。

## 其他

1) `$ go run cmd/carol.go -d 7 -l medium -s 2` 支持 3 个可选参数
   1) `-l`: 获取指定的练习难度，练习难度分别为 `easy`、`medium`、`hard`，默认显示所有难度级别
   2) `-s`: 指定排序字段，1: 题目名称排序、2: 上一次完成时间、3: 完成次数，默认上一次完成时间
   3) `-d`: 指定上一次完成时间的时间范围，可以输入任意阿拉伯数字，例如 7 代表统计 7 天内完成过的练习题，默认不限制时间范围
2) 可以结合艾宾浩斯遗忘曲线 excel 文档来使用，[点击跳转](http://www.xuexili.com/jiyili/1351.html)
3) 如果你感觉对于某个练习题已经得心应手了，可以挑战更高难度的，本项目中提供的题目没有特定的练习顺序，我们可以选择自己感兴趣的
4) 刻意练习有 4 点原则
   1) 目标要明确
   2) 做事时要及其专注
   3) 需要及时看到反馈并进行调整
   4) 走出舒适区，习惯孤独
