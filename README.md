
Model Structure/Formula
The NNet08 model employed in SecuRLock follows a feedforward neural network structure with a single hidden layer. This design is both computationally efficient and effective for tasks such as fraud detection.

Structure Description
Input Layer: Accepts multiple features derived from transaction and demographic data, such as transaction amount, time, and account activity.
Hidden Layer: A single hidden layer processes the input features through:
Weighted sums of the inputs.
A non-linear activation function (e.g., sigmoid or ReLU) applied to capture complex relationships in the data.
Output Layer: Produces a score or probability indicating the likelihood of fraud. The output is calculated as a weighted combination of hidden layer outputs using an activation function suitable for classification tasks (e.g., sigmoid).
Model Formulas
Hidden Layer Activation:
ℎ
𝑗
=
𝑓
(
∑
𝑖
=
1
𝑛
𝑤
𝑖
𝑗
𝑥
𝑖
+
𝑏
𝑗
)
h 
j
​
 =f( 
i=1
∑
n
​
 w 
ij
​
 x 
i
​
 +b 
j
​
 )
ℎ
𝑗
h 
j
​
 : Output of the 
𝑗
𝑡
ℎ
j 
th
  hidden neuron.
𝑥
𝑖
x 
i
​
 : Input features.
𝑤
𝑖
𝑗
w 
ij
​
 : Weights connecting inputs to the hidden neuron.
𝑏
𝑗
b 
j
​
 : Bias for the 
𝑗
𝑡
ℎ
j 
th
  hidden neuron.
𝑓
f: Activation function (e.g., sigmoid or ReLU).
Output Layer:
𝑦
=
𝑓
𝑜
(
∑
𝑗
=
1
𝑚
𝑣
𝑗
ℎ
𝑗
+
𝑐
)
y=f 
o
​
 ( 
j=1
∑
m
​
 v 
j
​
 h 
j
​
 +c)
𝑦
y: Final output (fraud score).
𝑣
𝑗
v 
j
​
 : Weights connecting hidden neurons to the output.
𝑐
c: Bias for the output.
𝑓
𝑜
f 
o
​
 : Output activation function (e.g., sigmoid for binary classification).
Error Calculation and Backpropagation:
The error (
𝐸
E) is computed as:
𝐸
=
1
2
∑
(
𝑦
pred
−
𝑦
true
)
2
E= 
2
1
​
 ∑(y 
pred
​
 −y 
true
​
 ) 
2
 
Gradients of 
𝐸
E with respect to weights (
𝑤
𝑖
𝑗
,
𝑣
𝑗
w 
ij
​
 ,v 
j
​
 ) are calculated using backpropagation and updated as:

𝑤
𝑖
𝑗
←
𝑤
𝑖
𝑗
−
𝜂
∂
𝐸
∂
𝑤
𝑖
𝑗
w 
ij
​
 ←w 
ij
​
 −η 
∂w 
ij
​
 
∂E
​
 
𝑣
𝑗
←
𝑣
𝑗
−
𝜂
∂
𝐸
∂
𝑣
𝑗
v 
j
​
 ←v 
j
​
 −η 
∂v 
j
​
 
∂E
​
 
𝜂
η: Learning rate.
