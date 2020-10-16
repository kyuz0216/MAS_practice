# MAS_practice
Practice repository for multi agent simulation using python

# 入門チュートリアル_メモ
## Boltzmann Wealth Model  
お金を交換するエージェントのモデル  
少数が富を持ち、大勢が貧困になる  

## モデルの設定
ModelとAgentを作成  
- Model・・・エージェント全体に関すること(例えば、エージェントの総数など)  
- Agent・・・個々のエージェントに関すること(初期条件など)  

## スケジューラの作成  
エージェントが活性化される順序を制御する特殊なモデルの構成要素  
各々のモデルに記述する(def step:)  

## Spatial Element  
gridとcontinuousの２種類がある。  
- grid・・・チェス盤みたいなセル上にエージェントを配置できる  
    - SingleGrid・・・セルごとに1つのエージェントのみ配置できる  
    - MultiGrid・・・同じセルに複数のエージェント配置できる  
- continuous・・・連続空間の任意の場所にエージェントを配置できる  
```
from mesa.space import MultiGrid
```

## データコレクター  
以下の三つのデータを保存する
- モデルレベルの変数  
- エージェントレベルの変数  
- テーブル  

# Reference
- https://mesa.readthedocs.io/en/master/  
- https://ichi.pro/mesa-no-shokai-python-de-no-e-jyento-be-su-no-moderingu-207465600654490  

# memo(関係ある？)  
- http://bin.t.u-tokyo.ac.jp/summercamp2015/document/game3_chika.pdf
