# データサイエンスの教科書
本リポジトリはデータサイエンスの知識を日本に広めるべく、整備したものである。 
初心者向けの内容からアドバンスドな内容までを網羅的に取り扱うことを目指す。

## 1. 確率・統計

### 1.1 確率論の基礎

#### 1.1.1 集合論とσ-代数
- 事象の演算（和・積・補集合）とその基本性質  
- Borel集合とBorel σ-代数（実数空間における代表例）  
- σ-代数の構成と完備化の概念  
- 可測空間と測度（測度論の基礎）  
- 確率測度と一般測度の違い  
- 0-1法（ブローリ＝カンテリの補題） の概要

#### 1.1.2 確率空間の定義と公理
- コルモゴロフの公理（3つの公理）  
- 完全加法性／可算加法性  
- 乗法定理と条件付き確率  
- 全確率の定理とその拡張  
- ベイズの定理の数学的定義と直感的理解  
- 排反事象と加法定理（和の法則）

#### 1.1.3 確率変数と分布 
- 離散型確率変数とPMF（確率質量関数）  
- 連続型確率変数とPDF（確率密度関数）  
- 累積分布関数（CDF）の性質（右連続・単調非減少 等）  
- 変数変換と分布の導出（単射変換、Jacobian）  
- 混合型確率変数（連続＋離散の組み合わせ）

#### 1.1.4 期待値・モーメント・共分散
- 期待値の定義（離散/連続）と存在条件  
- 分散の公式と不偏推定（標本分散との関係）  
- 共分散と相関係数（線形依存関係の強さ）  
- 高次モーメント・中心モーメント・生モーメント  
- モーメント母関数（MGF）と累積量生成関数（CGF）  
- 条件付き期待値と独立性（反復期待値の公式など）  
- Tchebychevの不等式、Markovの不等式（上界評価）

#### 1.1.5 代表的な分布
- 離散分布（ベルヌーイ、二項、幾何、ポアソン、超幾何 など）  
- 連続分布（正規、一様、指数、ガンマ、ベータ、コーシー など）  
- 特性関数（Characteristic Function）の定義と性質  
- MGF（Moment Generating Function）との比較  
- Levyの連続性定理（分布収束の基礎）  
- 中心極限定理への応用（正規近似など）  
- 分布間の距離（KLダイバージェンス、Wasserstein距離 等）

#### 1.1.6 極限定理
- 大数の法則（弱法則、強法則）とその応用例  
- Khintchineの強法則（収束のより一般的な視点）  
- 中心極限定理（リャプノフの定理、Lindebergの定理）  
- Berry-Esseenの定理（中心極限定理の誤差評価）  
- ポアソン近似、正規近似（二項分布の近似など）  
- 局所極限定理（確率質量関数レベルでの近似）  
- 安定分布とα-stable分布（一般化された極限定理）

---

### 1.2 統計的推測の基礎

#### 1.2.1 標本分布と母集団
- 標本平均・標本分散と母平均・母分散  
- χ²分布、t分布、F分布の導出過程  
- サンプルサイズの概念と統計的推測への影響  
- 中心極限定理と標本分布の近似

#### 1.2.2 推定理論
- 点推定の考え方（母数を1つの値で推定）  
- 不偏性・一致性・有効性の定義と関係  
- 最尤推定（MLE）、モーメント法、ベイズ推定（事前分布・事後分布）  
- 区間推定と信頼区間の考え方
- 推定量の分散評価（クラメール＝ラオの下限など）

#### 1.2.3 仮説検定
- 帰無仮説・対立仮説、p値、有意水準  
- 区間推定の考え方（母数に対する不確実性の表現） 
- 正規分布近似による信頼区間（z分布、t分布）  
- 比率や分散の区間推定（χ²分布などの応用）  
- 多重比較問題と補正（Bonferroni、Holm、FDRなど）  
- 信頼係数（1−α）とサンプルサイズ設計

#### 1.2.4 仮説検定の一般フレームワーク
- 帰無仮説・対立仮説、p値、有意水準  
- 検定統計量と臨界値（αと有意域）  
- TypeⅠエラーとTypeⅡエラー、検定力の概念  
- 効果量（effect size）と実務的な有意性

#### 1.2.5 母数検定（z検定、t検定、F検定、χ²検定など）
- 単標本・二標本のz検定、t検定（対応あり／対応なし）  
- F検定による分散の比較  
- カテゴリカルデータに対するχ²検定（適合度検定、独立性検定）  
- 検定の適用条件と前提（正規性、等分散性など）

#### 1.2.6 多重比較・サンプルサイズ設計
- 多重比較問題（TypeⅠエラー率の増加）  
- ボンフェローニ補正、Holm法、FDR（Benjamini-Hochberg法）  
- 検定力分析（力関数）とサンプルサイズの見積もり  
- 実験計画法との関連（要因数、ブロック設計など）

#### 1.2.7 ノンパラメトリック手法
- Wilcoxon順位和検定、Mann-Whitney U検定  
- Kruskal-Wallis検定、Friedman検定  
- ノンパラメトリックな信頼区間の構築  
- パラメトリック検定との比較と使い分け

#### 1.2.8 ブートストラップと再標本化法
- ブートストラップ標本の生成と推定量の分布推定  
- ジャックナイフ（データ1点除去法）の考え方  
- パラメトリック／ノンパラメトリック・ブートストラップ  
- バイアス修正、ブートストラップ信頼区間（BCa法など）

---

### 1.3 回帰分析と分散分析

#### 1.3.1 線形回帰の概要
- 単回帰モデル：モデルの立て方、最小二乗法  
- 回帰直線の解釈：切片と傾きの意味  
- 回帰の前提条件（線形性、独立性、等分散性、正規性）  
- 応答変数（従属変数）と説明変数（独立変数）  

#### 1.3.2 重回帰と行列表現
- 多変数回帰モデルの拡張（複数の説明変数）  
- 回帰モデルの行列表示：\( \mathbf{y} = X\beta + \epsilon \)  
- 最小二乗解の行列式（正規方程式）  
- 計算方法とアルゴリズム上の注意点  

#### 1.3.3 Gauss-Markov定理と推定の最適性
- BLUE（Best Linear Unbiased Estimator）の概念  
- Gauss-Markov定理の仮定と証明のスケッチ  
- 共分散行列：推定量の分散評価  
- 有効性と最小分散不偏推定（MVUE）との関係  

#### 1.3.4 回帰診断と残差分析
- 残差プロット、QQプロットの解釈  
- 外れ値・強影響点（Leverage、クック距離など）  
- 分散不均一性（重み付き最小二乗法の導入）  
- 回帰モデルの妥当性評価と修正手法
  
#### 1.3.5 多重共線性と正則化
- 多重共線性の原因と影響（VIFの計算）  
- Ridge回帰、Lasso回帰（正則化の仕組み）  
- Elastic Netとハイパーパラメータ選択  
- 高次元回帰問題におけるスパース推定

#### 1.3.6 モデル選択と交差検証
- AIC、BIC、調整済み決定係数などの指標  
- ステップワイズ法、逐次加除法  
- クロスバリデーション（k-fold、LOOCV）の実践  
- 過学習と汎化性能のバランス  

#### 1.3.7 分散分析（ANOVA）の応用
- 一元配置分散分析とF検定  
- 二元配置分散分析・繰り返し測定ANOVA  
- 固定効果・ランダム効果モデル  
- 多重比較法（Tukey、Scheffé、Bonferroni など）  

#### 1.3.8 カテゴリカルデータ解析
- ロジスティック回帰の回帰係数と対数オッズ  
- Poisson回帰、負の二項回帰（カウントデータ解析）  
- 対数線形モデル：多元表解析  
- モデル適合度検定と情報量基準（G²、AICなど）

---

### 1.4 多変量解析

#### 1.4.1 多変量正規分布とマハラノビス距離
- 多変量正規分布のパラメータ（平均ベクトル・共分散行列）  
- マハラノビス距離と外れ値判定  
- 等高線の楕円形状と可視化  
- ウィシャート分布（共分散行列の事前分布として）

#### 1.4.2 共分散構造と推定
- 共分散行列・相関行列の推定法（MLE、サンプル共分散）  
- スペクトル分解と固有値・固有ベクトル  
- 高次元下での共分散推定（スパース共分散推定など）  
- 欠測データ補完と共分散行列の推定

#### 1.4.3 主成分分析（PCA）とSVD
- PCAの幾何学的解釈（最大分散方向）  
- 特異値分解（SVD）との関連  
- 図示と可視化（2次元・3次元への次元削減）  
- カーネルPCAなどの拡張
#### 1.4.4 因子分析とSEM
- 共通因子モデル（探索的因子分析、EFA）  
- 確認的因子分析（CFA）  
- 構造方程式モデリング（SEM）の概要  
- パス解析とパス図の読み方

#### 1.4.5 判別分析（LDA、QDAなど）
- 線形判別分析（LDA）の原理  
- 二次判別分析（QDA）との比較  
- 判別境界と誤判別率の評価  
- クラス不均衡への対策とロバスト化

#### 1.4.6 混合分布モデルとEMアルゴリズム
- 混合ガウスモデル（GMM）の定義  
- EM（期待値最大化）アルゴリズムの導入と収束  
- モデル選択（AIC、BIC）と混合数の推定  
- 混合モデルのクラスタリング応用

#### 1.4.7 高度な次元削減
- NMF（Non-negative Matrix Factorization）の仕組み  
- t-SNE（t-Distributed Stochastic Neighbor Embedding）  
- UMAP（Uniform Manifold Approximation and Projection）  
- 多様体学習の考え方と比較

#### 1.4.8 多変量ロバスト化と外れ値対策
- ロバスト共分散推定（MCD, M-estimatorなど）  
- 外れ値の検知と処理（Mahalanobis距離、ロバスト手法）  
- 高次元での外れ値問題  
- データ前処理とスケーリングの重要性

#### 1.4.9 多変量解析の応用事例
- マーケティング（セグメンテーション、コンジョイント分析）  
- バイオインフォマティクス（遺伝子解析、RNA-seqなど）  
- 金融リスク管理（ポートフォリオ分析）  
- 画像／テキストなど高次元メディアへの応用
---

### 1.5 ベイズ統計

#### 1.5.1 ベイズ推定の枠組み
- 事前分布、尤度、事後分布、事後予測分布  
- ベイズの定理を用いた更新プロセス  
- ベイズと古典的推定の比較

#### 1.5.2 MCMC（Markov Chain Monte Carlo）
- Metropolis-Hastingsアルゴリズム  
- Gibbsサンプリング  
- 収束判定（R-hatなど）、バーンイン、サンプリング実装上の注意

#### 1.5.3 ベイズ階層モデル
- 階層構造（ランダム効果、固定効果）  
- 部分プーリングと完全プーリング  
- 階層ベイズモデルの応用事例

#### 1.5.4 変分ベイズ法と近似推論
- 変分推論の概念（ELBO、Jensenの不等式）  
- Laplace近似、Expectation Propagation（EP）  
- 大規模データへの応用

#### 1.5.5 ベイズ決定理論と損失関数
- ミニマックス基準とベイズ基準  
- 0-1損失、二乗損失、絶対値損失など  
- ベイズリスクと意思決定

---

### 1.6 時系列解析

#### 1.6.1 時系列データの基礎概念
- 定常性とホワイトノイズ  
- ラグ演算子、自己相関、偏自己相関

#### 1.6.2 ARIMAモデル
- AR、MA、ARMA、ARIMAモデルの定義  
- 季節モデル（SARIMA）  
- モデル選択（AIC、BIC、AICc）

#### 1.6.3 拡張・高度時系列モデル
- VAR（Vector AutoRegressive）モデル  
- 状態空間モデルとカルマンフィルタ  
- GARCHモデルによる分散のモデリング

#### 1.6.4 外生変数・因果推論
- Transfer Functionモデル、Intervention Analysis  
- Granger因果性検定、VARにおける因果推論

---

### 1.7 生存分析とイベント履歴解析

#### 1.7.1 生存関数・ハザード関数
- Kaplan-Meier推定、ログランク検定  
- 累積ハザードとNelson-Aalen推定

#### 1.7.2 Cox比例ハザードモデル
- 部分尤度と変数選択  
- 検証方法と回帰診断

#### 1.7.3 複雑な生存データの解析
- 区間打ち切り、競合リスク、再発イベント  
- 多状態モデルとマルコフ的アプローチ

---

### 1.8 因果推論と欠測データ解析

#### 1.8.1 因果推論の基礎
- 因果ダイアグラム（DAG）、do演算子  
- 交絡、選択バイアス、レイテンシーバイアス

#### 1.8.2 傾向スコア法、マッチング
- PSマッチング、ウェイト付け  
- ダブルロバスト推定

#### 1.8.3 操作変数法、回帰不連続デザイン
- 操作変数（IV）の定義と仮定  
- 回帰不連続（RD）の理論と適用

#### 1.8.4 欠測データの取り扱い
- 欠測メカニズム（MCAR, MAR, MNAR）  
- 完全ケース解析、多重代入法（MI）  
- EMアルゴリズムによる補完

---

### 1.9 ロバスト統計・高次元解析

#### 1.9.1 ロバスト推定の概念
- 外れ値の影響、M推定  
- Huber推定量、RANSAC

#### 1.9.2 高次元統計
- “次元の呪い”とスパース推定  
- Lasso, Ridge, Elastic Net  
- 高次元部分空間学習

#### 1.9.3 大規模データ・オンライン統計
- オンライン更新（逐次最小二乗、Streaming Algorithms）  
- スケーラブルベイズ（Large-scale MCMC、Variational Methods）

#### 1.9.4 確率的グラフィカルモデル
- ベイジアンネットワーク、マルコフネットワーク  
- 因子グラフとメッセージパッシングアルゴリズム

---

### 1.10 発展的トピック・実践上の考察

#### 1.10.1 シミュレーションとブートストラップ
- ブートストラップ標本、ジャックナイフ  
- モンテカルロシミュレーション

#### 1.10.2 選抜バイアスと再現可能性
- p-hacking、multiple testing problem  
- メタアナリシス、データ共有の重要性

#### 1.10.3 論文での統計手法の誤用・注意点
- p値至上主義の問題  
- エフェクトサイズと実用的意義

#### 1.10.4 その他最新動向
- 統計的因果推論の進展（Double Machine Learning など）  
- Bayesian Deep Learning、Probabilistic Programming  
- 高次元ベイジアン、スパースベイジアン推定

---

## 2. 機械学習理論

*（内容は後日追加予定）*

---

## 3. 機械学習理論（深層学習）

*（内容は後日追加予定）*

---

## 4. MLOps

*（内容は後日追加予定）*

---

## 5. MLアプリケーション開発

*（内容は後日追加予定）*
