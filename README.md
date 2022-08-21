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
