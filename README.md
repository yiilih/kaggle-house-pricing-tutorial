### Quick rundown of data analysis
目標：集合 Kaggle house-prices 的 tutorials for python，總結為一份 "數據分析流程"。

- 目前只有基本架構。使用 WSL + venv + VSCode
- 目前只有看到第一個 tutorial。只有看到初步 load data & preview 的階段。還有三份 tutorial 可以繼續加入 
- 歡迎一起來編輯。可以在 Discord 討論。也可以用 Git pull request。 
- 我不會用 containers/Dockers，歡迎會的人來教！感恩先！
- 我也沒用過 Kaggle Colab。也歡迎會的人來教！感恩啦！

Reference:
https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/overview/tutorials


### Download data
Save data to `~/proj/kaggle-house-pricing/data`

```
mkdir -p ~/proj/kaggle-house-pricing/data

# Download with Kaggle API
kaggle competitions download -c house-prices-advanced-regression-techniques -p ~/projs

cd ~/projs
unzip house-prices-advanced-regression-techniques.zip -d kaggle-house-pricing/data
rm house-prices-advanced-regression-techniques.zip
```

### Virtual environment and install packages

```
python3 -m venv venv
source venv/bin/activate
pip install pandas matplotlib seaborn numpy scipy
pip install -U scikit-learn
```

### Start VSCode

```
code .

# Install extensions for Python
```
