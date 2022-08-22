・EC2インスタンスへのアクセスはSSHキーで管理されている。IAMユーザーはアクセスキーを用いてEC2インスタンスに接続できない。

・DirectConnectゲートウェイ

プライベート仮装インターフェースを介して、DirectConnect接続を、同じリージョンや異なるリージョンに配置されたご自身のアカウントで1つ以上のVPCに接続できる。

・責任共有モデルのAWS側

物理的な保護。インフラストラクチャー管理、ホストOS

## #45

・WaitCondition

countプロパティで指定する成功のシグナルが送信されない場合に発生する.cfg-signalが正常に作成や更新されたかどうかを示すシグナルをCloudFormationに送信する。

・ELB

インスタンスIDやIPアドレスでターゲットを登録できるようにターゲットグループを設定。IPアドレスに基づいてアクセス制限したアプリケーションを制限。

## #44

・パッチ

セキュリティソフトウェアのパッチは静的ファイル。

・スポットインスタンス

データ分析、バッチ処理、バックグラウンド処理、オプションタスクに適している。

## #43

・PersonalHealthDashborad

AWSがリソースに影響を与える可能性のあるもんぢあが発生している場合に追跡し、アラートを提供するのに役立つ。

・SystemManangerオートメーション

EC2インスタンスと他のAWSリソースの一般的なメンテナンスとデプロイのタスクを簡素化

・SystemManangerインベントリ

EC2とオンプレミスのコンピューティング環境への可視性を提供

・SystemManangerパラメータストア

設定データ管理と機密管理のための安全な階層型ストレージを提供。

・SystemManangerRunCommand

一般的な管理タスクを自動化し、臨時の変更を大規模に実行することができる。

## #42

・DependsOn属性

リソース間の依存関係を定義できる。EC2インスタンスが起動する前にDBインスタンスが作成されるようにするなどできる。

CloudWatch
|  ステータス  |  内容  |
|  ----  |  ----  |
|  OK  |指定されたメトリクス・式が定義されたしきい値内にあることを意味する|
|  ALARM  |指定されたメトリクス・式が定義されたしきい値外にあることを意味する|
|  INSUFFICIENT  |アラームが開始されたばかり・メトリクスが利用できない・アラームの状態を決定するためのメトリクスに十分なデータがないことを意味する。|

## #41

・SurgeQueueLength

正常なインスタンスへのルーティングを保留中のリクエストか接続の合計数。キューがいっぱいになると拒否されて、SplilloverCloutがカウントされる。

・SystemManangerPatchManager

セキュリティ関連の更新パッチをマネージドインスタンスに適用するプロセスを自動化する。

・SSL証明書を発行

公開鍵暗号方式。複数のElasticIPアドレスを持つ複数のネットワークインターフェースを割り当てる。

・SAML

ActiveDirectoryとAWSの間のIDブローカーとして使用できる。アクセス許可を管理し、各ユーザーに一時的な認証情報を付与できる。

・AWS Config

パブリックアクセスのあるS3バケットが作成された場合、監視とアラートを設定できる。

## #40

・CodePipeline

CI/CDツール。

・カスタムリソース

ユーザーがwスタックを作成・更新・削除するたびにCloudFormationを実行する。Node.jsとPython関数の場合、テンプレートにインラインで関数コードを指定できる。

・AWSConfig

リソース設定の変更を追跡できる。サポートされていないサービスは、APIを使用して構成管理プロセスを自動化し、現在と過去のデータを比較する。

・CreateStack

スタック作成に失敗した時にスタックのロールバックを無効にする。

・EnableTerminationProtection

スタックを誤って削除されるのを防ぐ。
## #39

・AddToLoadBalancer

中断中に起動されたインスタンスは追加されない。手動で登録する必要がある。

・リージョン間のAMIのコピー

ソースAMIを変更し、それらの変更をターゲットリージョンのMAIに反映させる場合、ソースAMIをターゲットリージョンに再度コピーする必要がある。

・ReplicaLag

Auroraレプリカについて、プライマリインスタンスからアップデートをレプリケートする際の遅延時間

・CloudWatchエージェント

AWSとオンプレの両方のインスタンスを監視できる。CloudWatchダッシュボードを使用して、リソースのメトリクスとアラームをカスタマイズした状態で確認できる。

・SystemMananger

CloudFormationのテンプレート内のEC2インスタンスのAMIのIDを更新するとき、SystemManangerパラメータストアを用いることで、最新のWindowsAMIを取得してテンプレートがその時点の最新のAMI IDに更新される。

## #38

・変更セット

スタックの変更案が実行中のリソースに与える可能性がある影響を確認できる。(削除など)

・cfn-signal

・EC2インスタンスが正常に作成・更新されたかどうかを示すシグナルをCloudFormationに送信。インスタンスにソフトウェアアプリケーションをインストールする時、CloudFormationにシグナルを送信できる。

・ロールバック

リソース間に依存関係があると、ネストされたスタックでロールバックが失敗する可能性がある。

・Retain

リソースを保持するために、そのリソースに対してRetainを指定する。スタック削除後もそれらのリソースを使用したり変更したりできる。

・長期アクセスキーの代わり

長期アクセスキーの代わりに一時的なセキュリティ認証情報を使用。SDKとCLIはアクセスキーを自動的に処理できる。

## #37

・SystemMananger

問題の迅速な特定と修正に役立つ。インスタンスにパッチを適応するプロセスを自動化する。

・ElasticCacheforRedisのマルチAZ

ノード障害に対応し、管理者の手を煩わせることなく可用性を高める。

・CloudWatch

マウスで期間を選択してマウスボタンを離すと、特定の期間をズームできる。

・DMS

データベースを短期間で安全にAWSに移行できる。移行中でもソースデータベースは完全に利用可能な状態に保たれる。

・AlarmNotification

CloudWatchからのアラームを受信するが、AutoScalingポリシーは実行しない

## #36

・EBSボリュームのファイル復元

ファイルを復元するには、必要なデータを含むEBSスナップショットからボリュームを作成して、EC2インスタンスにアタッチする。

・AutoScaling

以上のあるインスタンスの置き換えはできる。インスタンスの再起動は対応できない。

・プロビジョンドIOPSSSDボリューム

ボリュームサイズに対するプロビジョンドIOPSの最大割合は500:1。プロビジョンドIOPSSSDボリュームのサイズは4GiB~16TiBである。

・ネストされたスタック

複数のテンプレートで同じコンポーネントを宣言する共通パターン。

・スタックセット

1つのCloudFormationテンプレートを使用して、複数のAWSアカウントにスタックを生成できる。

|  アクセスコントロールタイプ  |  AWSアカウントレベルの制御  |  IAMユーザーレベルの制御  |
|  ----  |  ----  |  ----  |
|  ACL  |  ●  |  ×  |
|  バケットポリシー  |  ●  |  ●  |  
|  IAMポリシー  |  ×  |  ●  |

## #35

・RDSの高可用性

マルチAZ配置は、1つだけDBだけを実行し、スタンバイレプリカに同期的に複製する。

・CloudWatch

カスタムメトリクスをサポートしている。ユーザーはいつでもカスタムデータをキャプチャし、CLIかAPIを使用してCloudWatchにデータをアップロードできる。

## #34

・CloudWatchエージェント

サーバーからメトリクスを収集できる。ディクス容量を取得して。CloudWatchアラームにて管理者へ通知できる。

・ELBのスティッキーセッション

リクエストが同じサーバーにルーティングされ、新たに追加されたサーバーを利用していない可能性がある。

## #33

・AMIのコピー

コピーしたAMIはアクセス権限をコピーしない。元のAMIから新しいAMIに起動許可、ユーザー定義タグ、S3バケット許可をコピーしない、コピー操作が完了すると、起動許可、ユーザー定義タグ、S3バケット許可を新しいAMIに適用できる。

・SyStemsManagerPatchManager

セキュリティ関連のアップデートと他のタイプのアップデートの両方でマネージドインスタンスにパッチを適用するプロセスを自動化する。

・EC2インスタンスがすぐに終了する

EBSボリューム制限に達した。EBSスナップショットが破損している。AMIに欠損部分がある。ルートEBSボリュームは暗号化されていて、複合用のKMSキーにアクセスできない。EC2インスタンスの最大起動数は関係ない。

・AWSのコストと使用状況

アカウントとそのIAMユーザーが使用した各サービスカテゴリのAWS使用状況が、時間単位または日単位の明細項目として一覧表示されている。コスト分配のためにアクティブ化されたタグも表示される。

## #32

・ELBのパスベースのルーティング

URLパスに基づいてリクエストを転送するルールを持つリスナーを作成できる。複数のバックエンドサービスにトラフィックをルーティングできる。

・RDSのイベントカテゴリ

RDSのイベントが起きるとSNSを通じて通知を送れる。カテゴリは、作成・削除・復元・通知。

・EBSスナップショット

スナップショットは非同期で行う。

・DLM

DataLifesysleManagerはEBSスナップショットとEBS-Backed AMIの作成・保持・削除を自動化。

・エフィラメントポート

ポート番号1024-65535までの範囲。

・SugerQueueLength

正常なインスタンスへのルーティングを保留中のリクエストか接続の合計数。追加のリクエストか接続は、キューがいっぱいになると拒否

## #31

・CPUUtilization

AutoScalingグループのスケーリングポリシーを制御する。

・S3 1 ゾーン　低頻度アクセス

アクセス頻度は低いが、必要な時にすぐに取り出せる。一つのAZにしか保存しないため、データを失う可能性もあるがやすい。

・TCPとUDP

TCPは送信側と受信側が何度か通信をする。送ったり、送られたり。UDPは送信して帰ってこない。

・EC2AutoScalingの動的なスケーリング

動的スケーリングを設定するには、アラームとスケーリングポリシーを作成し、AutoScalingグループに関連する必要がある。

・スナップショットの暗号化サポート

S3を使用してスナップショットのサーバー側の暗号化を有効にしても、EBSスナップショットはS3-SSEを使用して暗号化できない。

・サブネットの削除

サブネットを削除する前に、その中の全てのインスタンスを削除する必要がある。

## #30

特記事項なし

## #29

・S3の適切なストレージかどうかを判断

ピーク使用時の1秒あたりのリクエストの総数を調べる必要がある。S3は高いリクエスト率に自動的にスケールされる。

・CloudTrail

AWSサービス情報へのアクセスを提供し、CloudTrailログへの読み取り専用アクセスは最小権限の原則に従うベストプラクティスの実装に役立つ。

・Redshiftクラスターを実行する総コストを削減

クラスターで自動スナップショット及び手動スナップショットを無効にする。

・PersonalHealthDashboard

お客様に影響するイベントがAWSで発生したいる場合にアラート・改善のためのガイダンスを提供。

・CostExplorer

コストと使用状況を表示・分析するために使用。今後12ヶ月にどれだけ費やす可能性が高いかを予測し、リザーブドインスタンスを購入するための注意事項を得られる。

・StorageGatewayテープゲートウェイ

StorageGatewayテープゲートウェイの仮装テープライブラリ(VTL)は、バックアップのための費用対効果の高いソリューションを提供

## #28

・INSUFFICIENT_DATA

CloudWatchのアラームの一つ。アラーム開始直後であるか、メトリクスが利用できないか、データが不足していてアラームの状態を判断できない。

・OpsWorksのレシピ失敗を特定

OpsWorksのレシピが失敗したインスタンスにログインし、chefログを確認することでデバッグできる。

・CloudWatch

EC2インスタンスのステータスチェックを監視して、破損したEC2インスタンスを識別できる。

## #27

・S3のアクセス管理

|  アクセス権  |  内容  |
|  ----  |  ----  |
|  ユーザーポリシー  |  IAMユーザーに対して、S3バケットへのアクセス権限を設定<br>複数バケットやS3以外のものも含めて一元的にユーザー権限を指定する場合など  |
|  バケットポリシー  |  S3バケットごとに、アクセス権限を指定<br>クロスアカウントでのS3バケットアクセス権を付与する場合など  |
|  ACL  |  各バケット及びオブジェクトのアクセス権を指定<br>バケット単位やオブジェクト単位で簡易的に権限を付与する場合など  |

・S3のバケットとオブジェクトのアクセス許可

ACLは各バケットとオブジェクトのアクセス権限を指定できる。フォルダにACLの設定はできない。

・Route53

Route53位置情報ルーティングはコンテンツを地域に制限できる。

## #26

・SQS

SQSはAutoScalingアクションをトリガーできない。

・CloudWatchLogs

ログの収集、保存、分析に役立つ。RC2インスタンス・CloudTrail・Route53・その他のソースログファイルの監視、保存、アクセスができる。

・RDS

グローバルテーブルをサポートしていない。

・Blue/Green

ユーザートラフィックを、アプリケーションやマイクロサービスの以前のバージョンから、ほぼ同一の新しいリリースに徐々に転送するアプリケーション・リリースモデルで、両バージョンが稼働中の状態で実施するもの。

・AutoScalingグループメトリクス

GroupTotalInstancesを使用すると、AutoScalingグループに含まれるインスタンスの合計数を特定する。

・Auroraレプリカ

Auroraが、書き込みDBインスタンスからその他全てのDBインスタンスに、レプリケーションを自動でセットアップする。読み取り操作をスケールでき、可用性を高めることができる、

## #25

・CloudFormation

リソースが削除されないようにするために、DeletionPolicyを設定できる。

・CloudFormationのNoEcho

NoEchoパラメータは機密データのパラメータ隠すのに役立つ。アスタリスクで表示される。

・EC2リソースの削除しないようにする

タグをつけて削除を拒否することで、開発者がインスタンスを削除することを防ぐ。また、開発者用に別のAWSアカウントを作成することで、開発者が本番インスタンスを操作できないようにできる。

・S3にアクセス許可

AWSのルートアカウントの所有者が、S3にアクセス許可を設定するとき、S3バケットポリシー・ユーザーポリシー・S3ACLで管理できる。

・iSCSIデバイスとしてマウント

StorageGatewayのボリュームベートウェイのキャッシュボリュームはオンプレミスサーバーのストレージの拡張機能として機能し、頻繁にアクセスされるデータを低遅延アクセスように保存できる。

・CloudWatch

NetworkIn : インスタンスによって受信された全てのネットワークインターフェースのバイト数

## #24

・CloudWatchで日時確認

グラフの確認で日時開始・終了時間で指定するためAbsoluteタブを使う。

・ELBの監視

CloudWatchメトリクス、ELBアクセスログ、CloudTrailログが役立つ。ELBのヘルスチェックはELBに接続されているインスタンスの状態をチェックするため、ELBの監査には役立たない。

・ApproximateNumberOfMessageVisible

SQSに基づくスケーリングができる。特定のレベルに達したときは常にEC2インスタンスを拡大するポリシーを作成できる。変化する条件に応じてスケーリングするために役立つ。

・S3バケットに読み取り・書き込み許可付与

他のAWSアカウントに許可を付与するため、バケットのアクセス許可を付与するAWSユーザーの正規IDが必要。

・請求アラートにアクセス

アクセスするためには請求アラートを有効にする必要がある。

・クロスリージョンダッシュボード

複数のAWSアカウントと複数のリージョンのCloudWatchデータを1つのダッシュボードにまとめられる

## #23

・S3バケットへのアクセスを許可

S3バケットへのアクセスを許可するリソースベースのポリシーを作成し、開発アカウントにアクセス権を委任できる。

・クォーターの引き上げ

AWSのサービスごとにデフォルトのクォーターがある。AWSサポートセンターよりケースを作成してEC2インスタンスのクォーターの引き上げを要求する。

・クォーター

制限

・SSH接続したときに接続タイムアウト

セキュリティグループで、SSHポートが許可されていない。秘密鍵が正しくない。ログインするユーザーが間違っている。インスタンスCPUの負荷が高い。

アクセスキーを用いてSSHへログインしない。

・EC2インスタンスの削除保護

DisableApiTerminationを使い、EC2インスタンスで削除保護を有効にする。

## #22

・Billing and Cost Management

AWSの請求の支払い、使用量のモニタリング、コストの計上にに使用するサービス。コスト配分タグを使用してAWSのコストを詳細レベルで追跡できる。

・セキュリティグループとネットワークACL

両方で許可された場合、ACCEPLレコード。ネットワークACLで拒否されたとき、REJECTレコード

・Route53かあらELBにリーティング

Route53からロードバランサーをポイントするエイリアスコードを作成。

## #21

・SSE-C

独自の暗号化キーを設定できる。

・VPN接続の設定

カスタマーゲートウェイをネットワークアドレス変換(NAT)を実行するデバイスの背後にある場合、NATデバイスのパブリックIPアドレスを使用している。

・SQLServer

SQLServerエンジンのマルチAZ配置は、同期レプリケーションを使用し、SQLServerネイティブのミラーリングテクノロジーを採用。

・RDSのメンテナンスウィンドウ

セキュリティパッチをあてると、Dmインスタンスを強制的にオフラインにする可能性がある。

## #20

・DirectConnect

オンプレミスからネットワークからVPCに直接接続するためのプライベート仮装インターフェースを確立できる。

・SystemManager

AWSでインフラストラクチャを表示と制御するために使用できるサービス。

・CloudWatch

インスタンスをモニタリングし、元となるハードウェア障害かAWSによる復旧を必要とする問題により、定常に働かなくなった時に自動的にインスタンスを復旧するEC2アラートを作成できる。

・コスト配分タグの使用

タグを使用してリソースを整理し、コスト配分を使用して、AWSのコストを詳細　レベルで追跡できる。

・SQSキューを削除

ユーザーは手動でキューを削除できる。即時に削除される。

・マルチAZ配置のメンテナンス手順

1. スタンバイに対してメンテナンスを実行する。
2. スタンバイをプライマリに昇格させる。
3. 旧プライマリでメンテナンスを実行し、その旧プライマリが新しいスタンバイになる。

・AutoScalingグループを削除

AutoScalingの最小サイズと希望する容量を0にする

## #19

|  IAMのデフォルト制限  |  個数  |
|  ----  |  ----  |
|  一人のIAMユーザー  |  最大で10つのグループ  |
|  AWSアカウントごとにグループ |  300  |
|  AWSアカウントのロール  |  1000  |
|  AWSアカウントに格納されるサーバー証明書  |  20  |

・ObjectRestoreCompleted

オブジェクトの復元完了の通知をリクエストできる。

・ObjectRestoreCompleted

復元開始の通知をリクエストできる。

・SSE-Cの暗号化

暗号化キーにっっよるサーバー側の暗号化アルゴリズムの情報を指定する必要がある。暗号化アルゴリズムの指定。256ビットの暗号化キー。

・サブネット

VPCに複数のサブネットを作成する場合、サブネットのCIDRブロックは重複できない。

## #18

・ELBを作成

利用可能な場プリックサブネットを少なくとも1つ選択する必要がある。インバウンドトラフィックを許可するセキュリティグループをロードバランサーに割り当てる必要がある。

・IPsec

暗号化によってパケットの秘匿や改ざん検知を実現するプロトコル。

・VPC接続

DirectConnectを使用して、リモートのネットワークからVPCへの専用のプライベート接続できる、Site-to-SiteVPN接続を組み合わせると、IPsecで暗号化された接続を作成できる。

・IDフェデレーションとロールベースのアクセス制限

オンプレミスのActiveDirectlyとIAMロールに接続するADコネクターが必要。

・サーバ側の暗号化(SSE-C)を使用したデータの保護

ユーザーが暗号化キーを主導でローテーションする必要がある。

## #17

・Instance Store-Backed Windows AMIからEBS-Backed Windows AMIへの変換はできない。Linuxベースならばできる。

・AZでのインスタンスの起動

AZを設定しないと、自動的に選択される。これにより最適なAZを選択できる。

・CloudWatchメトリクス

データのアップロードには2分かかり、新規メトリクスが表示されるまでは最大15分かかることもある。

・ハイパーバイザー

物理的なマシンの中に、仮想的なコンピュータを作り出し、実行する際に使用

## #16

・アプリケーションが新しいインスタンスにフェールオーバーできるようにする

フェールオーバー先のインスタンスに移動できるセカンダリENIを作成して、フェールオーバー先のインスタンスのセカンダリプライベートIPアドレスをプライマリENIに割り当てる。

・CloudWatchLogsでサポートされる形式

テキストベースの一般的なログデータ形式かJSON形式のログであれば取り込み可能。その最小値は1秒間隔。タイムゾーンの指定おは必須ではない。

## #15

・AutoScalingのライフサイクルフック

ライフサイクルフックをAutoScalingグループに追加して、ログファイルが配信されるまでEC2インスタンスを待機状態(Pending:Wait)にすることができる。

・Proxy Protocolを有効にする

ロードバランサーが、Proxy Protocolが有効になっているプロキシサーバーの背後にないことを確認する。ロードバランサーが、Proxy Protocolが有効になっているプロキシサーバーの背後にないことを確認する。

・SNSでサポートされているプロトコル

SQS、HTTP/s、Email、SMS、Lambda。

・エラーコード

4xxのときは、オブジェクトが見つからず、アクセスが見つからない場合である。

## #14

・CloudWatchとSNS

CloudWatchでEC2のステータスをチェックしてSNSでアラートを通知することでプライベートクラウド上にサーバーを起動できる。

・S3のデータを複製

S3標準と標準IAは、AWSリージョンの少なくとも3つのAZでお客様を冗長的に保存する。追加で操作をする必要はない。

・Elastic BeanstalkログをS3に保存

Elastic Beanstalkの環境構成の設定でS3へのログファイルのローテーションを有効にすることでS3にログを保存できる。

・EC2インスタンス容量の不足

InsufficientInstanceCapacityとエラーが発生すると、リクエストに対応するために必要な十分なオンデマンドキャパシティがない。

AZを指定しないでインスタンスを起動するか、キャパシティを補償するためにリザーブドインスタンスを購入することで解決できる。

## #13

・CloudFormation

テンプレートでは、いくつかの主要なセクションが含まれている。Resourcesセクションは、唯一の必須セクション。

・インスタンスへのアクセス制限

インスタンスにタグ付けして、ユーザーがインスタンスの開始・停止を明示的に許可しても、インスタンスの削除を拒否することで防御層を追加できる。

・バケットACL

デフォルトでは、S3オブジェクトの所有者はそれをアップロードしたAWSのアカウント。アクセス権を付与するとき、オブジェクトのACLを更新することで、バケット所有者にオブジェクトのフルコントロールを付与できる。

## #12

・CloudWatchメトリクス

CPU使用率ではなく同時セッションのカスタムメトリクスと使用してAutoScalingグループで需要に応じた負荷を自動的に処理できる。

・SQSのメッセージライフサイクル

SQSは最長メッセージ保持期間を超えてキューに残っているメッセージを自動的に削除する。デフォルトのメッセージ保持期間は4日間。保持期間の幅は60秒から14日まで。

・監査に備えるベストプラクティス

IT運用管理の証拠収集、第三者の監査済みAWSコンプライアンスレポート、侵入テストの実行が該当。

・WRITE ACLリスト

他のAWSアカウントがそのバケット内のオブジェクトを作成、上書き、削除することを許可する。同等のS3バケットポリシーアクセス許可はs3:DeleteObject

## #11

・CloudWatchアラームのアクションシュミレート

SetAlarmStateAPIを使用して任意の状態に設定することにより、アラームをテストできる。

・EBSのパフォーマンス向上

EBS最適化インスタンスかEBSの種類を変更が考えられる。

・RDSのフェイルオーバー

DBインスタンスのDNSレコードをスタンバイDBインスタンスを指すように自動的に変更することで、スタンバイレプリカへの切り替えがアプリケーションへのアクセスに影響を与えない。

・CloudFormationのエラー時の挙動

エラー時の自動ロールバック機能が有効になっている。エラーが発生するまでにスタックを作成したすべてのAWSリソースは削除される。

## #10

・AutoScalingインスタンスのヘルスチェック

インスタンスを異常ありとマークすると、置き換えがスケジュールされる。インスタンスを終了し、新しいインスタンスを起動する。

・AWSの予想請求額をモニタリングする請求アラームの作成

予想請求額のアラームを作成する前に、請求アラートを有効にする必要がある。有効にすると、AWSの予想請求額をモニタリングし、請求メトリクスデータを使用してアラームを作成できる。

・アプリケーションのセキュリティの管理

SysOps管理者がこの問題を修正する必要がある。

・Memcachedのメトリクス

Evictions : 新しく書き込むための領域を確保するためにキャッシュが排除した、期限切れではない項目数。

## #9

・Route53のDNSレコードグループ

ドメインのzone apexをマッピングするためにエイリアスコードを使用できる。

・RDSイベント通知

DBセキュリティグループに対してイベント通知を設定。DBセキュリティグループが変更されると、通知が送信される。

・EBSのスナップショット

EBSスナップショットを作成している間も読み書きできる。

・AutoScalingのスケジュールスケーリング

スケジュールされたアクションのタイミングは一位である必要がある。AutoScalingは競合を知らせるエラーメッセージを表示する。

## #8

・EBS-Backed EC2インスタンスの再起動

再起動のみではホストは変更しない、一度停止してから起動することで新しいホストで実行される。

・CloudFormationのテンプレート待機

WaitConditionリソースとCreationPolicy属性を使用して、適切に構成されるまでスタックを待機する必要がある。

・EBSボリュームの初期化

空のEBSボリュームは、作成するとすぐに最大のパフォーマンスを発揮し、初期化を必要としない。

## #7

・クラスタープレイスメントグループ

低ネットワークレイテンシーと高ネットワークスループット。

・RDSメンテナンスウィンドウ

メンテナンスウィンドウを設定していない場合、AWSはデフォルトのメンテナンスウィンドウを選択する。

・Route53加重ルーティングポリシー

指定した比率に指定してトラフィックを制御できる。

・ELBのアクセスログ

ELBのアクセスログには、リクエストを受け取った時間、クライアントのIPアドレス、レイテンシー、リクエストのパス、サーバーレスポンスなどの情報が含まれている。EC2インスタンスのIPアドレスが含まれない。

・CloudFormation

アプリケーションとインフラストラクチャを維持し、バージョン管理にGitを使用して変更を追跡できる。

## #6

・責任共有モデル

EC2インスタンスはお客様が管理するので、パッチとセキュリティは会社が管理する

・クロスリージョンレプリケーション

コンテンツをレプリケートする

・仮装プライベートゲートウェイ

VP接続のAmazon側であり、VPCとデータセンター、ホームネットワーク、コロケーション施設との間の接続を確率するのに役立つ。

## #5

・IAMポリシー

IAMポリシーはグローバルに作動し、特定のIPアクセスのみを制限するためにユーザーに関連付けできる。

・IPスプーフィング

送信元のIPアドレスを偽装し、通信を行う攻撃手法。

・パケットスニッフィング

ネットワークノード間で送信される情報のパケットを収集および記録するプロセス

・AutoScaling

踏み台ホストを含むシステムを設計していて、人間の介入差しに可用性を持たせるには、AutoScalingグループで最小と最大を1に設定して常時1台起動するようにする。

## #4

・EBS-Backed AMI, Instance Store-Backed AMI

EBS-Backed AMIは、EBSベースのAMIによって作成される。Instance Store-Backed AMIは、S3ベースのAMIによって作成される。

・読み取りパフォーマンスの向上

CloudFrontを使用すると、リクエストをキャッシュすることで負荷を軽減。RDSリードレプリカは読み込み負荷を軽減。ElasticCacheは頻繁に使用されるデータをキャッシュする

・サブネット

デフォルトサブネットはパブリックサブネットを指定している。またインターネットへの接続は、ElasticIPかパブリックIPを持っている場合にのみアクセスできる。サブネット最小の範囲は

## #3

・EBS-Backed AMIのステータスチェック情報の確認

インスタンスを停止して再起動することで、障害が発生したホストから正常なホストで切り替わり、障害を復旧できる。

## #2

・EC2インスタンスに追加のEBSをアタッチ

追加ボリュームは、ボリュームを切り離して、同じAZで稼働している他のインスタンスにアタッチできる。

・EC2インスタンスに障害発生

EC2インスタンスにElasticIPを割り当てる。障害が発生したときは新しいインスタンスを生成し、ElasticIPアドレスを新しいインスタンスに割り当てる。

・ハードコード

コンピュータプログラムを開発する際に、特定の動作環境を決め打ちして、その環境を前提としたデータをソースコードの中に直に記述する

・AWS Configルール

AWSリソースの設定内容を評価する・リソースで発生する設定変更を継続的に追跡し、これらの変更がルールの条件に違反していないかどうかを確認

・SDK

アプリケーションを開発・デプロイをする。APIのようなもの？よくわからん

・ウェブIDフェデレーション

カスタムインサインインコードを作成したり独自のユーザーIDを管理しなくてよい。AmazonなどのWebサービスでログインすれば、AWSのサービスを使えるようになる。

## #1

・ネットワークACL

複数のホストでIPアドレスの制限をかけるときに使用する。

・AutoScaling

1つか複数のロードバランサをアタッチし、インスタンスがヘルスチェックに合格しても、インスタンスは置き換えない。ロードバランサのヘルスチェックを有効し、インスタンスがヘルスチェックに合格しないと置き換える

・AutoScalingにインスタンスを追加

AutoScalingグループの希望する容量を増やす。インスタンスを手動で起動し、ELBに登録するわけではない。

・スケーラブルにSQSメッセージの処理を改善

SQS job Pbserverパターンを利用してキュー内のメッセージ数(ジョブリクエスト)に応じてインスタンスを自動で増減する。CloudWatchでモニタリングする項目をSQSに指定する。

・帯域幅

最高周波数と最低周波数の差

・EBS最適化オプション

EC2インスタンスとEBSボリューム間の帯域幅の改善に役立つ

・VPCピアリング接続

AWSネットワークを介して、同じリージョンや異なるリージョンのVPCを接続する費用対効果が高いソリューション。2つのVPC間でプライベートなトラフィックのルーティングを可能。通信の単一障害点や帯域幅のボトルネックは存在しない。

・DirectConnect

VPCとオンプレミスのデータセンター間の接続を提供する

・ElasticCacheのCurrConnections

クライアントの接続数(リードレプリカの接続を除く)。

・ELBのSpilloverCount

拒否されたリクエストの数。リクエストの最大がSurgeQueueLengthを超えるとカウントする。

・RDSのマルチAZ展開

コンソールを使用してRDSインスタンスを変更し、マルチAZオプションを選択する。
