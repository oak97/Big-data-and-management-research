一  文件说明

```shell
.
├── COVID-19-csse_covid_19_data-csse_covid_19_time_series（下载的原始数据）
│   ├── time_series_covid19_confirmed_global.csv
│   ├── time_series_covid19_deaths_global.csv
│   └── time_series_covid19_recovered_global.csv
├── UK.csv（整理后的英国三月数据）
├── USA.csv（整理后的美国三月数据）
├── get_data.ipynb（整理原始数据的源代码）
├── get_data.pdf
├── time_seq.ipynb（作业内容：包括时间序列绘图、模型建立）
└── time_seq.pdf
```



二  作业内容

1. 首先整理了美国（USA）和英国（UK）3月1日-3月29日的数据  
2. 因为同一国家的不同指标量级差别较大、同一指标在不同国家量级差别也较大，所以我们从3个角度绘制折线图  
- 如果不从量级上比较，只看形状，会发现相比英国，美国各个指标形状的上升趋势更明显，波动却较小
- 英国后期累积死亡人数比累积治愈人数明显多，而美国后期的累积治愈人数明显上升
- 随着时间增长，美国各项指标的总数比英国高得多  
3. 将3月1日-3月22日的数据作为训练数据，训练出模型后预测3月23日-3月29日的数据，并与真实数据进行比较