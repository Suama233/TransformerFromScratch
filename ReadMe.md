原视频地址 : https://youtu.be/ISNdQcPhsts?si=v2zegWQ6ggZ8EjXC

源代码仓库 : https://github.com/hkproj/pytorch-transformer

原论文地址 ( Attention Is All You Need ) : https://arxiv.org/abs/1706.03762

建议前置 : 大概知道 Transformer 是什么 ( 因为这里更多关于实现 , 对于些理论也会有感想但不成体系 ), 大概了解 torch 进行模型构建与训练的基本框架

这个仓库完全基于 Umar Jamil 的实现 . 其仓库与原视频使用的代码略有不同 , 但完全无关理解与本质 . 这里选用了仓库的代码 , 并对基本每个 .py 文件提供了用 .ipynb 写的具体讲解.但没有提供无注释的源 .py 代码还请去原仓库查看,也可自己将所有 .block 复制到 .py 里直接运行 .

**所有笔记全部来自于自己的理解** , 也就是说大部分甚至可能是错的 . 如果哪里有问题请在 issue 中提出 . 

注意并没有添加额外模块来实现 import notebook 的功能,也就是说仓库本身是不能运行的 .  

对于一些不太好理解的地方 , 添加了 appendix.ipynb 文件 , 包含一些单个细节的可视化与理解 , 这个文件是可以在此环境下独立运行的

原视频中一些没有具体展开提 , 但仓库中有的部分 , 这里暂时没有包含 , 将来可能会补 ( 

关于具体实现的顺序 ( 与原视频相同 ) : 

- 首先是 model.py 的全部 .
- 然后是 train.py 的前半部分 . 弄清楚大概流程 , 构建 tokenizer
- 然后是 dataset.py 的内容
- 顺便将相关参数提炼出来 , 放到 config 里
- 最后完善 train.py