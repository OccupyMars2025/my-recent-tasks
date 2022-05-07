# my-recent-tasks
document my finished  tasks and to-do tasks. The newer tasks will be listed firstly.

#  2022/5/6 - :
【PaddlePaddle Hackathon 第二期】任务总览    
https://github.com/PaddlePaddle/Paddle/issues/40234    
 (【PaddlePaddle Hackathon 2】18、为 Paddle 新增 paddle.heaviside 和 paddle.Tensor.heaviside API #41872 
https://github.com/PaddlePaddle/Paddle/pull/41872           reference code)


# 2022/5/4 -  :   
【PaddlePaddle Hackathon 第二期】任务总览#40234        
(https://github.com/PaddlePaddle/Paddle/issues/40234)    
 [PaddlePaddle Hackathon 2 No.22] add paddle.index_add to Paddle #42475           
 (https://github.com/PaddlePaddle/Paddle/pull/42475)        
 refer to paddle.index_fill
 

# 2022/5/4 - 5/6 :   
【PaddlePaddle Hackathon 第二期】任务总览#40234     
 【PaddlePaddle Hackathon 2 No.11】在 Paddle 中新增 paddle.index_fill 功能 #42468    
 https://github.com/PaddlePaddle/Paddle/pull/42468
       
After accomplishing task 11, you may also be interested in the task 22:    
【PaddlePaddle Hackathon 2】22、在 Paddle 中新增 paddle.index_add 功能 #40311     

      
# 2022/3/20 - 2022/5/4:         
【PaddlePaddle Hackathon 第二期】任务总览#40234      
[PaddlePaddle Hackathon 2nd No.16] add API RReLU #42466      
https://github.com/PaddlePaddle/Paddle/pull/42466
the source code is firstly gotten by modifying the source code of dropout op, but the dropout op is implemented in version 1.X
Now it is version 2.x,  

TODO: In unittest, in training mode, I cannot get the output of rrelu by using numpy.      
How the random number generation mechanism in paddle and numpy communicates with each other ???    

TODO: fix bug: if I uncomment those test cases that I have commented off in the file
python/paddle/fluid/tests/unittests/test_rrelu_op.py , then I will have the error "'X' contains uninitialized tensor"
