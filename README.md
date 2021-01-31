# AzurLaneCalculation-Summary
用于收集碧蓝航线经验计算，升级所需等公式和算法。


### 后宅经验加成
经验的加成和舒适度的关系如下：
```java
bonus_rate=c_lv/(c_lv+100);
```
其中：`bonus_rate`是加成的百分比，`c_lv`是舒适度。

### 后宅存粮消耗
存粮消耗和舰船数量有关，有存粮的条件下每`15s`经验跳动一次，消耗存粮`4n`（n为同时获得经验的舰船数）。
$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
${$tep1}{\style{visibility:hidden}{(x+1)(x+1)}}
$$
