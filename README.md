# 2021 字节跳动安全 AI 挑战赛 —— 色情导流用户识别

- 团队名称：ECNU_ICA
- 复赛成绩：0.9611
- 最终排名：rank 7
- 团队成员：im0qianqian、Bin、RR



## 相关链接

- 比赛地址：[https://security.bytedance.com/fe/ai-challenge#/sec-project?id=1&active=0](https://security.bytedance.com/fe/ai-challenge#/sec-project?id=1&active=0)
- 方案总结（待更新）：[https://www.dreamwings.cn/2021_bytedance_security_ai_track1/5828.html](https://www.dreamwings.cn/2021_bytedance_security_ai_track1/5828.html)
- 答辩视频（待上传）



## 目录结构

```
├─datasets
│  └─round_2
│      │  ReadMe.txt
│      │
│      ├─测试数据
│      │      用户id(无标签).csv
│      │      用户基础信息.csv
│      │      用户投稿信息.csv
│      │      用户行为信息.csv
│      │
│      └─训练数据
│              用户基础信息.csv
│              用户投稿信息.csv
│              用户标签.csv
│              用户行为信息.csv
│
├─resources
│  └─round_2
│          个签特征_提交版.csv
│          投稿较多id.csv
│
├─src
│      main_round2_final.ipynb
│
└─submits
    └─round_2
        └─all_model_with_fi
```



## 环境依赖

```
numpy==1.19.2
seaborn==0.11.2
lightgbm==3.1.1
catboost==0.26.1
pandas==1.1.5
tqdm==4.62.2
scikit-learn==0.24.2
matplotlib==3.3.4
wandb==0.12.3
```



## 运行方法

1. 将训练数据与测试数据放置于 `datasets/round_2/训练数据` 与  `datasets/round_2/测试数据` 下（如目录结构所示）
2. 根据环境依赖配置环境（也有 requirements.txt 文件）
3. 确保 `submits/round_2/all_model_with_fi` 文件夹本地存在
4. 执行 `src/main_round2_final.ipynb`

