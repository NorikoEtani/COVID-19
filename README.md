# COVID-19
SARIMAモデルを用いた日本のCOVID-19感染予測プログラム

作成日：2021年8月20日

作成者：江谷典子

電子メール：kerotan@kcn.ne.jp


【目的】

日本のCOVID-19感染予測を時系列解析SARIMAモデルを用いて行う．SARIMAモデルの構築と予測の手順を解説しながらプログラムを実行できるGoogle ColaboratoryのColab ノートブック（*.ipynb）を提供する．

【開発環境】

・Google ColaboratoryのColab ノートブック（*.ipynb）

【オープンデータ】
Our World in Data，Coronavirus (COVID-19) Vaccinations

Mathieu, E., Ritchie, H., Ortiz-Ospina, E. et al. A global database of COVID-19 vaccinations. Nat Hum Behav (2021)

https://ourworldindata.org/covid-vaccinations

owid-covid-data.csv（2020/1/22~）

References：
[1]Mathieu, E., Ritchie, H., Ortiz-Ospina, E. et al. A global database of COVID-19 vaccinations. Nat Hum Behav (2021). https://www.nature.com/articles/s41562-021-01122-8


日本国内の感染者数（NHKまとめ）

https://www3.nhk.or.jp/news/special/coronavirus/data-all/

nhk_new_covid19_domestic_daily_data.csv（2020/01/16~）


都道府県ごとの感染者数（NHKまとめ）

https://www3.nhk.or.jp/news/special/coronavirus/data/

nhk_new_covid19_prefectures_daily_data.csv（2020/01/16~）


【提供するプログラム】

・correlation.ipynb SARIMAモデルのパラメータ推定，新規感染者数および新規死亡者数の予測，予測結果の作図

・correlation.ipynb 日本の新規感染者数，新規死亡者数，ワクチン2回接種者数（累計）の相関係数計算とheatmap作図

・evaluation.ipynb ラグ次数をaicまたはbicを選択するための回帰モデルの評価

【サンプルデータ】

・OpenData　利用しているオープンデータ

・csv　本プログラムで利用している日本・東京都・大阪府・神奈川県の新規感染者および新規死亡者数データ，日本のワクチン2回目接種者数（累計）データ


・plot_csv　本プログラムで利用している予測プロットデータ


以上

