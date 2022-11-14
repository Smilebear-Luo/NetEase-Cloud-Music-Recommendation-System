## 文件结构
.
├── feature
│   ├── song_play_count.csv
│   └── user_action_seq_feature.csv
├── feature_get_song_play_count.ipynb
├── feature_get_user_action_seq.ipynb
├── input
│   ├── members.csv
│   ├── sample_submission.csv
│   ├── song_extra_info.csv
│   ├── songs.csv
│   ├── test.csv
│   └── train.csv
├── model_SVD.ipynb
├── model_rank.ipynb
├── model_recall.ipynb
├── preprocess
│   ├── train.csv
│   └── val.csv
├── preprocess.ipynb
└── readme.md

## 文件说明
feature文件夹用于存储额外提取的特征数据.
input文件夹用于存放原始数据,请将原始数据放置其中.
preprocess文件夹用于存放处理后的训练数据与验证数据.

## 代码说明
所有代码均以ipython notebook形式组织，请使用相关应用打开(推荐jupyter).
请先运行preprocess.ipynb文件，用于处理原始数据，进行特征工程，提取基础特征，生成的数据保存在preprocess文件夹中.
其中，两份代码是用于提取后续模型运行所需要的特征：feature_get_song_play_count.ipynb用于提取召回模型所需的词频数据和feature_get_user_action_seq.ipynb用于提取用户播放歌曲序列特征，生成的特征数据均保存在feature文件夹中.
另外三份代码均为核心模型代码.