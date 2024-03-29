---
layout: post
title: Portfolio / ポートフォリオ
date: 2024-03-05
---

## Autoware を用いた、私有地への右折侵入シミュレーション（開発中）

### イメージ(シミュレーション)

  <img src="https://raw.githubusercontent.com/kodama3008/kodama3008.github.io/cite/screenshots/TurnRight.png" title="右折シミュレーション" width="800" height="500" >

### イメージ(アシュアランスケース)

  <img src="https://raw.githubusercontent.com/kodama3008/kodama3008.github.io/cite/screenshots/GSN.png"  width="800" height="500" >

### 概要

- **プロジェクトの概要**: 安全な自動運転システムの要求仕様をアシュアランスケースで書き出し、シミュレーションを用いて検証する
- **使用技術**: Autoware（シミュレータ）、Plotjuggler（パラメータの抽出）、D-Case（アシュアランスケースの記述と検証）、ROS2（通信）
- **使用言語**: YAML（シナリオ記述）、Python（CSV ファイルで出力されるパラメータの整形）、 Javascript（検証のためのコード）

### プロジェクトの詳細

株式会社 TIER Ⅳ と合同で取り組んでいる研究です。研究テーマは「シミュレーターとアシュアランスケースの連携による自動運転システムのディペンダビリティ保証フレームワーク」であり、自動運転システムのディペンダビリティを確保するための新しいアプローチを提案します。具体的には、Autoware シミュレーターに、D-Case（アシュアランスケース）を連携させ、以下に挙げるメリットを得ることを目的しています。なお、図のアシュアランスケースは私有地への右折侵入シナリオに限定したものであり、また開示可能な範囲に絞っています。

- **実証と検証の強化**:
  - シミュレーションを使用してシステムの振る舞いをテストし、アシュアランスケースに基づいてシステムが要求仕様を満たすことを検証します。これにより、システムの信頼性や安全性に関するアシュアランスを強化できます。
- **使構成パーツの相互関係に関する理解の助け**:
  - アシュアランスケースを記述することで、各要素の関係性が視覚的にわかりやすくなります。また、シミュレーションや、テストケースのフィードバックを、記述したアシュアランスケースと比較することで、アシュアランスケースの漏れ（＝認識不足）を確認できます。

現在は自動運転車が私有地へ右折侵入するシナリオに絞って、シナリオを構成するユースケース単位で検証を行っています。

### GitHub リンク

[https://github.com/kodama3008/shioji_simulation/tree/main](https://github.com/kodama3008/shioji_simulation/tree/main)

## Esmini を用いた、自動運転車と歩行者のシミュレーション

### イメージ

<img src="https://raw.githubusercontent.com/kodama3008/kodama3008.github.io/cite/screenshots/esmini.png" title="Esmini　シミュレーション" width="800" height="500" >

### 概要

- **プロジェクトの概要**: 自動運転車が、ランダムな歩行者な状態に対応するシナリオをシミュレーションする
- **使用技術**: esmini（シミュレータ）
- **使用言語**: XML（シナリオ記述）、python（ランダムなパラメータの設定）

### プロジェクトの詳細

Autoware でのシミュレーションには高性能なデスクトップ PC が必要であり、デスクトップ PC が研究室に設置される期間の間に練習もかねてシナリオを作成しました。歩行者の位置や道路を横断する速度がランダムに設定され、それに対して自動運転車がどのような挙動をするかを検証しました。

### GitHub リンク

https://github.com/kodama-tier4/esmini-sim

## MOM（Matsulab Online Meetingtool）

### イメージ

<img src="https://raw.githubusercontent.com/kodama3008/kodama3008.github.io/cite/screenshots/MOM1.png" title="MOM1" width="800" height="500" >

### 概要

- **プロジェクトの概要**: オンライン会議における情報共有の難しさや、煩わしさを解消する
- **使用技術**: Unity、Cloud Speech-to-Text（音声認識機能）、Monobit エンジン（サーバー）
- **環境**: GitHub（コード管理）、Trello（タスク管理）、Slack（コミュニケーションツール）、Miro（オンラインホワイトボード）
- **使用言語**: C#
- **人数**:6 人

### プロジェクトの詳細

スクラム開発のフレームワークを用いて、6 人で開発を行いました。私はスクラムマスター兼プロダクトオーナーとして、プロダクトバックログの管理や各プラクティスの進行に尽力しました。
プロダクトは、 オンライン会議における情報共有の難しさや、煩わしさを解消することを目的の開発されており、以下の機能が備わっています。

- Zoom のような会議
- チャット機能
- 音声認識機能が備わっており、発言内容が自動で記録され pdf として出力できる
- ホワイトボード機能による、情報の可視化が可能

### GitHub リンク

[https://github.com/CSTmatsunolab/gigiroku2](https://github.com/CSTmatsunolab/gigiroku2)
