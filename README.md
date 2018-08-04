# Signal-tracking-using-Fuzzy-control-on-SIMULINK
Designed a fuzzy controller on Simulink to track the input signal in real time and selected the optimal parameters.  
设被控对象的传递函数为
![](https://github.com/JierunCHEN/Signal-tracking-using-Fuzzy-control-on-SIMULINK/raw/master/signal_mathematical_function.JPG)  
输入信号为方波，周期为1秒，幅值为1，可以用Pulse Generator模块来产生;    
e^(-0.0002s)表示传输延时0.002s（2ms），可以用Transport Delay模块来表示。  
1）设计两输入单输出模糊控制器，输入为偏差E和偏差变化率EC，输出为控制量U，使系统输出能实时跟踪输入信号。  
2）通过仿真理解并分析E和EC的参数选择对系统稳态误差和动态性能的影响，这些参数包括量化因子，论域的范围，模糊子集个数等。  
3）采用fuzzy-pid混合控制等改进方法，进一步提高控制系统的性能。  
4）仿真采用固定步长求解器，步长设定为1e-4。  
