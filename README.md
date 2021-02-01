# AzurLaneCalculation-Summary
用于收集碧蓝航线经验计算，升级所需等公式和算法。


### 后宅经验加成
经验的加成和舒适度的关系如下：
```java
bonus_rate=c_lv/(c_lv+100);
```
其中：`bonus_rate`是加成的百分比，`c_lv`是舒适度。

### 后宅存粮消耗
存粮消耗和舰船数量有关，有存粮的条件下每`15s`经验跳动一次，消耗存粮`4n`（n为同时获得经验舰船数）。
这样时间`t`（每小时）和存粮`s`（每单位存粮）的关系如下：
```java
t=s/(4*n)*15/3600
```
根据上边的公式，能得出以下存粮时间关系，~~方便摸鱼~~。

|存粮（每单位存粮）|时间（单船每小时）|等价关系|
|----|----|----|
|960|1|1船1时|
|1920|2|2船1时|
|2880|3|3船1时|
|3840|4|4船1时|
|4800|5|5船1时|
|5760|6|6船1时|
|11520|12|6船2时|
|23040|24|6船4时|
|34560|36|6船6时|
|46080|48|6船8时|

### 后宅存粮下限及上限（每单位存粮）
后宅存粮下限为`40000`，可供单舰船消耗`41.67小时`；
后宅存粮上限为`90000`，可供单舰船消耗`93.75小时`。
