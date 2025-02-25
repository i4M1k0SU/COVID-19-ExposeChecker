# COCOAログチェッカー

## これは何
iOS/AndroidのOSの接触通知ログを解析するツールです。  
正確には、ログ内のmatchCountの値が0ではないものの件数をカウントします。  
正規表現が使えるエディターでしたら、
`"MatchCount" : [1-9]+` として検索をし、ヒット数を見ることで同様にカウント可能です。(iOSフォーマット)  

一般の注意事項や詳細説明は実サイトを御覧ください  
[cocoa-log-checker.com](http://cocoa-log-checker.com)

## 開発経緯
個人的にスマホ内で接触通知のログを毎日クリックして`一致したキーの数` をチェックしていたのですが、スマホでは毎回チェックするのが意外と大変でした。  
そこで、スマホでも簡単に`一致したキーの数`を一括でカウントできるツールを自分用に作成して一般に公開したところ、思いの外反応が多くありました。

そこでこのツールを広く使ってもらうことで、一人ひとり正しく危機感を感じてもらい、気を引き締めて感染症対策に取り組んでいただけ、結果として感染者や重傷者等を一人でも減らせるのではないかと思うようになり継続的に修正や改善を行っています。

このツールの出力結果の件数は極めて感染リスクの低い接触が多く含まれており、この数が多いからと言って、新型コロナウィルスに感染しやすくなる訳ではありません。

しかしニュースなどで報じられているxx万人感染という統計的なデータではなく、自分の2週間の行動の中で、COCOAの新規陽性登録者がどれくらい近くに居たかという自分に直接関係のある数として表示されることで、感染者の多さや身近さを感じていただけると思っております。

初期の頃、いち早く公開することを目標に開発していたため、いまだにvue.js v2 を使用していたり、
きれいにコンポーネントとして分割できていない状況です。


## 誰が作ってるの
個人で開発/運営しております。  
土日や仕事終わりに開発しておりますので、全てのご要望やご提案に対応できない場合があります。ご承知おきください。

また、本ツールに関して製作者は収益を得ておりません。  
所属する組織を含め、いかなる団体とも利害関係はございません。


## 安全なの？
本ツールはクライアントサイド(スマホ内)でのみの処理で解析を行っているため、外部にペーストしたデータが送られるなどはございません。

そもそも接触通知ログには個人を特定できる情報は含まれておりません。


## お問い合わせ
何かございましたら、以下のいずれかにご連絡ください

- Twitter <a href="https://twitter.com/ktansai" target="_blank">@ktansai</a>
- メール <a href='mailto:cocoa.log.checker@gmail.com' target="_blank">cocoa.log.checker@gmail.com

- 不具合報告
  - Twitter等の連絡又は、issueを立てていただけると助かります。
- ご提案がある場合
  - 本リポジトリにて、Pull Requestをお送りいただけると助かります。
  - ユーザビリティや利便性の都合上、全てのPRをマージできるわけではありません。事前にご相談の上 実装いただけますと、手戻りが少ないと考えております。
