### Quick rundown of data analysis
目標：集合 Kaggle house-prices 的 tutorials for python，總結為一份 "數據分析流程"。

- 我常用的工具。使用 WSL + venv + VSCode 
- 歡迎一起來編輯。可以在 Discord 討論。也可以用 Git pull request

Reference:
https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/overview/tutorials


### Download data
Save data to `~/proj/kaggle-house-pricing/data`

```
mkdir -p ~/proj/kaggle-house-pricing/data

# Download with Kaggle API  https://github.com/Kaggle/kaggle-api
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
