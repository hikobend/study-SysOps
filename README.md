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
