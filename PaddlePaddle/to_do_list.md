# 0. (2022/8/29 7:00) release note 2.3.1
https://www.paddlepaddle.org.cn/documentation/docs/zh/develop/release_note_cn.html#id7
If you want to have an overall understanding of PaddlePaddle, you can refer to the above website
<img width="887" alt="image" src="https://user-images.githubusercontent.com/31559413/187099330-35477a18-a46d-43fc-a0dc-2d2566192cae.png">


# 1. (2022/8/27 11:00)task-irrelevant knowledge to study when this task is finished:
## what is "hook" ???
所有继承 nn.Layer 的 sublayer 都建议：

重写 forward 函数，尽量避免重写 __call__ 函数
__call__ 函数通常会包含框架层面的一些通用的处理逻辑，比如 pre_hook 和 post_hook 。重写此函数可能会覆盖框架层面的逻辑。

尽量将 forward 函数作为 sublayers 的调用入口
推荐这样写，但动转静也支持对 sublayers 的其他函数转写处理

python\paddle\fluid\dygraph\jit.py 
paddle.jit.save, paddle.jit.load, paddle.jit.to_static are all in this file.
## this file has enormous usage of "hook"
## you can also refer to  pre-commit

# 2. (2022/8/28 11:00)study souce code : https://github.com/sxyu/sdf  (pip install pysdf)
this project includes **Eigen**, **pybind11**  and  it  seems to be used in https://github.com/PaddlePaddle/PaddleScience     
most important: this project is very **light** and very suitable for your self-learning
