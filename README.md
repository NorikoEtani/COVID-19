# COVID-19
SARIMAモデルを用いた日本のCOVID-19感染予測プログラム

作成日：2021年8月20日

改訂日：2021年9月30日

作成者：江谷典子

電子メール：dr.noriko.etani@ieee.org

一般社団法人 情報処理学会のデジタルプラクティスレポート「時系列解析 SARIMAモデルを用いた日本のCOVID-19感染予測実証実験」をドキュメントとして利用してください．

https://ipsj.ixsq.nii.ac.jp/ej/?action=pages_view_main&active_action=repository_view_main_item_detail&item_id=213180&item_no=1&page_id=13&block_id=8

本プログラムの出力結果は次のURL（研究ブログ）にて公開しています．予測結果を更新する度にSNS twitterでお知らせしています．

・時系列データの分析と予測その１：日本の COVID-19 感染予測　https://researchmap.jp/blogs/blog_entries/view/387354/49dc5d4309d202225ecf14670b29299e?frame_id=844568

・時系列データの分析と予測その２：東京都・大阪府・神奈川県の COVID-19感染予測　https://researchmap.jp/blogs/blog_entries/view/387354/206fc13e488a815b29abb72c3fb04f7e?frame_id=844568

【目的】

日本のCOVID-19感染予測を時系列解析SARIMAモデルを用いて行う．SARIMAモデルの構築と予測の手順を解説しながらプログラムを実行できるGoogle ColaboratoryのColab ノートブック（*.ipynb）を提供する．

【開発環境】

・Google ColaboratoryのColab ノートブック（*.ipynb）

【オープンデータ】

・Our World in Data，Coronavirus (COVID-19) Vaccinations

Mathieu, E., Ritchie, H., Ortiz-Ospina, E. et al. A global database of COVID-19 vaccinations. Nat Hum Behav (2021)

https://ourworldindata.org/covid-vaccinations

owid-covid-data.csv（2020/1/22~）

References：Mathieu, E., Ritchie, H., Ortiz-Ospina, E. et al. A global database of COVID-19 vaccinations. Nat Hum Behav (2021). https://www.nature.com/articles/s41562-021-01122-8


・日本国内の感染者数（NHKまとめ）

https://www3.nhk.or.jp/news/special/coronavirus/data-all/

nhk_new_covid19_domestic_daily_data.csv（2020/01/16~）


・都道府県ごとの感染者数（NHKまとめ）

https://www3.nhk.or.jp/news/special/coronavirus/data/

nhk_new_covid19_prefectures_daily_data.csv（2020/01/16~）

【提供するプログラム】

・correlation.ipynb SARIMAモデルのパラメータ推定，新規感染者数および新規死亡者数の予測，予測結果の作図

・correlation.ipynb 日本の新規感染者数，新規死亡者数，ワクチン2回接種者数（累計）の相関係数計算とheatmap作図

・evaluation.ipynb ラグ次数をaicまたはbicを選択するための回帰モデルの評価

【サンプルデータ】

data.zipを解凍すると次のファイルフォルダが生成されます．

・OpenData　利用しているオープンデータ

　owid-covid-data.csv　世界のCOVID-19感染データ
 
　nhk_news_covid19_domestic_daily_data.csv　日本国内の感染者数（NHKまとめ）
 
　nhk_news_covid19_prefectures_daily_data.csv　都道府県ごとの感染者数（NHKまとめ）
  
・csv　本プログラムで利用している日本・東京都・大阪府・神奈川県の新規感染者および新規死亡者数データ，日本のワクチン2回目接種者数（累計）データ
　
　Japan_0818.csv　日本の新規感染者数・新規死亡者数・ワクチン2回接種者数（累計）
  
　Japan_0819.csv　日本の新規感染者数・新規死亡者数
  
　TOKYO_0819.csv　東京都の新規感染者数・新規死亡者数
  
　OSAKA_0819.csv　大阪府の新規感染者数・新規死亡者数
  
　KANAGAWA_0819.csv　神奈川県の新規感染者数・新規死亡者数
　
・plot_csv　本プログラムで利用している予測プロットデータ

　death_pred.csv　日本・東京都・大阪府・神奈川県の新規死亡者数予測（最大値・最小値）
 
　patien_pred.csv　日本・東京都・大阪府・神奈川県の新規感染者数予測（最大値・最小値）
　

以上

