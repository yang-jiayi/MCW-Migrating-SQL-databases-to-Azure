# SQL データベースを Azure に移行する

Wide World Importers (WWI) の子会社である Tailspin Toys は、いくつかの人気のあるオンライン ゲームを開発した企業です。2010 年に設立された同社は、オンラインの多人数ゲームを含んだ、非常に人気のあるゲーム シリーズの第一弾リリース以降、急激な成長を遂げました。以来、同社はゲーム ポートフォリオの大部分にオンライン機能を追加することで、その成功を積み重ねてきました。

オンライン ゲームの提供を円滑に行うために、同社はレンタルのハードウェアを使って、オンプレミスでゲーム サービスをホストしています。オンライン ゲームの追加によって、同社のゲームの人気は劇的に上昇しましたが、サービスへの需要が急速に増大したため、現在の構成のサポートに問題が生じるようになりました。

WWI は、クラウドへの移行により、どのように全体的なプロセスを改善でき、どのようにオンプレミスのセットアップで抱えている懸念事項や問題を解決できるかについてさらに詳しく知ることに関心を抱いています。現在は、1 つのゲームの VM とデータベースをクラウドに移行するための概念実証 (PoC) を実施しようとしています。また、最終目標はサービス全体を Azure に移行することであるため、クラウドへの移行後に全体的なアーキテクチャがどのようになるかをさらに詳しく理解したいと考えています。

2020 年 6 月

## 対象者

- データベース管理者
- SQL/データベース開発者
- アプリケーション開発者

## 要約

### ワークショップ

このワークショップでは、オンプレミスの VM と SQL Server 2008 R2 データベースを Azure 内の IaaS サービスと PaaS サービスの組み合わせに移行する計画を作成する方法について学びます。お客様の SQL Server 2008 R2 データベースと Azure のマネージド データベース オファリングとの間で、機能パリティや互換性の問題がないかを明らかにするために、評価を実施します。次に、最小限のダウンタイムまたはゼロ ダウンタイムで VM およびデータベースを含む既存のオンプレミス サービスを Azure に移行するためのソリューションを設計します。最後に、お客様のアプリケーションのセキュリティとパフォーマンスを向上させる、Azure で利用可能な高度な SQL 機能のいくつかのデモを実施します。

このワークショップを完了すると、ビジネス クリティカルなアプリケーションおよびデータベースのクラウド移行ソリューションをより効果的に設計および実装できるようになります。

### ホワイトボード設計セッション

このホワイトボード設計セッションでは、オンプレミスの VM と SQL Server 2008 R2 データベースを Azure 内の IaaS サービスと PaaS サービスの組み合わせに移行する計画をグループで作成します。トレーナーは、評価を実施して、顧客の SQL Server 2008 R2 データベースと Azure のマネージド データベース オファリングとの間の機能のパリティと互換性の問題を明らかにするためのガイダンスを提供します。次に、最小限のダウンタイムまたはゼロ ダウンタイムで顧客の VM およびデータベースを含むオンプレミス サービスを Azure に移行するためのソリューションを設計します。最後に、Azure で高度な SQL 機能のいくつかを有効にして、顧客のアプリケーションにおけるセキュリティとパフォーマンスを向上する方法についてのガイダンスを提供します。

このホワイトボード設計セッションを完了すると、ビジネスクリティカルなアプリケーションとデータベースのクラウド移行計画をより効果的に設計できるようになります。

### ハンズオンラボ

このハンズオン ラボでは、オンプレミスの SQL Server 2008 R2 データベースを Azure SQL Managed Instance (SQL MI) に移行するための概念実証 (PoC) を実施します。オンプレミスの SQL Server 2008 R2 データベースと Azure のマネージド データベース オファリングとの間で、機能パリティや互換性の問題がないかを明らかにするために、評価を実施します。続いて、ダウンタイムを最小限またはゼロに抑えながら、お客様のオンプレミスのプレイヤー情報 Web アプリケーションとデータベースを Azure に移行します。最後に、SQL MI で利用できる高度な SQL 機能の一部を有効にして、お客様のアプリケーションのセキュリティとパフォーマンスを向上させます。

このハンズオン ラボを完了すると、ビジネスクリティカルなアプリケーションおよびデータベースのクラウド移行ソリューションをより効果的に実装できるようになります。

## Azure サービスと関連製品

- Azure SQL Managed Instance (SQL MI)
- Azure SQL Database (SQL DB)
- Azure Database Migration Service (DMS)
- Microsoft Data Migration Assistant (DMA)
- Azure App Service
- SQL Server
- VM 上の SQL Server
- SQL Server Management Studio (SSMS)
- Azure 仮想マシン
- \[Visual Studio 2019\]
- Azure 仮想ネットワーク
- Azure 仮想ネットワーク ゲートウェイ
- Azure Blob Storage アカウント

## 関連リファレンス

- [MCW](https://github.com/Microsoft/MCW)

## ヘルプおよびサポート

マイクロソフト SME および MCW を提供する学習パートナーからのフィードバックおよびコメントをお待ちしております。

**日本語版について**

このリポジトリは、2020年6月時点の[MCW-Migrating-SQL-databases-to-Azure](https://github.com/microsoft/MCW-Migrating-SQL-databases-to-Azure)の日本語訳です。

**_お困りですか?_**

- まず、ラボに記載されているすべての指示 (「ハンズオン ラボの前に」のドキュメントを含む) に従っていることを確認します。
- 次に、問題を、その詳細な説明とともに送信します。
- pull 要求を送信しないでください。コンテンツ作成者がすべての変更を行い、pull 要求を送信して承認を求めます。

ワークショップ開催を計画している場合、_早めに資料をレビューおよびテストしてください。_少なくとも 2 週間前には実施することをお勧めします。

### レビューと問題の解決には 5 ～ 10 営業日かかります。