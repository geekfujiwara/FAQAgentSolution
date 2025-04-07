# FAQAgentSolution
AIによる FAQの生成、問い合わせ受付とAIによる回答案の作成、CSAT評価、多言語対応、作成したFAQのDataverse のファイルアップロードへの追加等の機能を提供する、FAQ管理とエージェントでのナレッジの最適化サイクルを回す包括的なソリューションです。

> [!Note]
> [ギークフジワラのX](https://x.com/geekfujiwara/status/1908231134816903362)まで是非感想・コメントをお寄せください！

## ソリューションの概要
以下の製品を組み合わせて、Power Platform のみで作成しています。そのためソリューションをインポートするだけで利用できます。

![image](https://github.com/user-attachments/assets/66f89e8b-8634-4676-8ee0-23b6bd8cb416)

主な動きを確認できる動画があります。

https://github.com/user-attachments/assets/a7ac2d31-c479-4415-959c-ee4e7e11f26a

## ソリューションの仕組み

### FAQの自動生成
ファイルやテキストから自動的にFAQを作成します。

![image](https://github.com/user-attachments/assets/b8cdce22-3c74-4b91-b307-05689eaab30b)



https://github.com/user-attachments/assets/edd8fc7f-9cb9-4f41-894e-6fa59737b743



### 社内ナレッジを優先し、回答がなかった場合にインターネット検索を行い回答
満足度評価を収集します。

https://github.com/user-attachments/assets/ad7623df-5949-4865-8457-4460fe008941

### CSAT評価の送信

![image](https://github.com/user-attachments/assets/516cfabd-04a7-445c-a4c0-09fe1bf66cab)

収集した結果は分析タブから利用できます。

![image](https://github.com/user-attachments/assets/9f287a99-c9bc-479f-a53f-66e9a8cb79a4)



### 問い合わせ起票
解決に至らなかった場合、問い合わせを起票することができます。問い合わせはFAQに追加されます。

![image](https://github.com/user-attachments/assets/0026f455-bffb-4469-8c86-a9bd0cc8b944)


https://github.com/user-attachments/assets/472ff7f9-3717-41b9-8406-0fff8aec60f8


### 回答案の作成
質問の回答案はAIが作成してくれます。

![image](https://github.com/user-attachments/assets/ebdf8d91-c5fe-449e-a681-8e71f9ca9299)

### 質問者への Teams 通知
回答が作成できたら、Teams で通知することができます。

![image](https://github.com/user-attachments/assets/f1a6dba2-8c69-4bbe-8e2d-600b71084ffc)

### エージェントの多言語対応
エージェントは英語にも対応させています。テスト画面から言語を切り替えると試すことができます。

![image](https://github.com/user-attachments/assets/4468b6d4-954a-45fd-9585-2c653663861c)

https://github.com/user-attachments/assets/77a4d28a-ccd6-4f5c-accf-dd5ff7fd652c

## ソリューションの利用
### インポート方法

[最新のソリューションをダウンロード](https://github.com/geekfujiwara/FAQAgentSolution/releases/tag/FAQAgent)します。

ダウンロードしたソリューションをソリューションからインポートします。

![image](https://github.com/user-attachments/assets/4e7b8cbd-31d7-475d-b03b-b16036cbc451)


インポート時に接続の作成が求められますので作成します。

![image](https://github.com/user-attachments/assets/451f8c91-dc7a-48d8-81ff-5f8ca08cbac3)


インポートしたソリューションFAQ Agentを開き、フローがオンになっていることを確認します。

![image](https://github.com/user-attachments/assets/df61832f-6a74-4cf5-b4b9-529ce8503397)


すべてのカスタマイズを公開します。

![image](https://github.com/user-attachments/assets/85478922-9793-416f-a566-2e79aa44b76b)

これでインポートは完了です。

### 利用方法

ソリューションは主にモデル駆動型アプリのFAQ管理アプリと、エージェントの2つで構成されています。

![image](https://github.com/user-attachments/assets/3c4a5d65-a6a7-4d34-96cf-222b7546190e)


#### FAQの生成
まずは元となるナレッジを作成します。そのFAQはAIを利用して生成します。

> [!Note]
> 元となるファイルやWeb上のテキストがあればFAQを生成できます。

FAQ管理アプリを開きます。

![image](https://github.com/user-attachments/assets/754ed6cc-f50c-48bc-8bf5-d6ba5b0b13f2)

再生ボタンから開くことができます。

![image](https://github.com/user-attachments/assets/a6267ae6-be48-452b-b536-e495d9190e41)

FAQの生成ページを開き、アプリのアクセス許可を行います。

![image](https://github.com/user-attachments/assets/59e5a35f-de98-4c41-a7cc-68e4e958b1d0)

ファイルをアップロードします。すると自動的によみこまれます。

![image](https://github.com/user-attachments/assets/2524be47-7e8c-4438-aabe-62a6c7f7110f)

この情報を利用して生成AIにてFAQ案を作成させます。FAQを作成をクリックします。

![image](https://github.com/user-attachments/assets/2362aaa2-85d7-4310-a834-c36ae415347c)

問題がなければFAQの保存をクリックします。

![image](https://github.com/user-attachments/assets/fa8dda94-28e1-409c-840d-6fbc46fb1bf4)

FAQに切り替えるとFAQが作成されていることがわかります。

![image](https://github.com/user-attachments/assets/c64ca0ea-5fbe-4668-b2b8-8e5f7d79d8ae)

#### Copilot Studio のエージェントへのナレッジの追加
作成したナレッジをエージェントに追加します。

追加先のエージェントを選択します。今回ソリューションに追加したのはPower Platform なんでもアシスタントというエージェントです。こちらを選択します。

![image](https://github.com/user-attachments/assets/9a4cc263-9aaa-4c65-9915-f9c13882e4b1)

ナレッジは公開されているものだけがエージェントに追加されるようになっています。

> [!Note]
> 公開というのはビジネスプロセスフローのこのステージのことです。
>
> ![image](https://github.com/user-attachments/assets/464ab1d9-1d2e-4ea0-a830-5fc2cec7c77f)

一括で公開する機能を用意しています。

BPFをすべて公開ボタンをクリックします。

![image](https://github.com/user-attachments/assets/db7b3bd1-7028-4d0f-a4e3-0d3e20a8dcbd)

FAQのデータを更新します。

公開済みナレッジに表示されました。

![image](https://github.com/user-attachments/assets/f273d49d-30c1-4fb8-96df-228e60779999)

> [!Note]
> FAQでも公開されたことがわかります。
>
> ![image](https://github.com/user-attachments/assets/6c5ed095-5e9c-4546-bb5b-15edf8b22487)
>
> この時点ではエージェントにナレッジはまだ追加されていません。
>
> ![image](https://github.com/user-attachments/assets/87d32a1a-c98d-47e4-bf45-a876678214fb)

次にこのボタンをクリックするとナレッジを選択したエージェントに連携することができます。

![image](https://github.com/user-attachments/assets/e19af2b6-cdf7-4b24-92cc-410214aa0cd7)

エージェントを更新してみると、ナレッジ(ファイルアップロード)にcsvファイルが追加されていることがわかります。

![image](https://github.com/user-attachments/assets/3fa20ee4-456d-4ba2-8877-7b3264f94403)

> [!note]
> 通常のエージェントでは以下の操作は不要ですべてのナレッジを対象とした検索を行いますが、本ソリューション内に含まれているエージェントはファイルのナレッジを選択する必要がありますので、このようなナレッジを更新した際には会話の強化のトピックを選択します。
>
> ![image](https://github.com/user-attachments/assets/043f3427-6c7c-42ff-93c0-d21d77929504)
>
> 以前選択されていたファイルが削除されているのでエラーが発生しています。
>
> ![image](https://github.com/user-attachments/assets/4810ee18-4806-4892-ada3-d01c58c448f3)
>
> チェックするとエラーは消えます。
>
> 保存して終了します。これでトピックにナレッジを関連付けることができました。
>
> ![image](https://github.com/user-attachments/assets/7e5293b7-1ea1-4e72-8d43-04b00e262bad)


#### テスト実行

>[!Note]
>ファイルアップロードのインデックスが完了するには時間を要します。しばらく待ってからエージェントへの問い合わせを行いようにしてください。

質問をしてみると、正しくFAQから回答が得られました。

![image](https://github.com/user-attachments/assets/9c2c1d0d-b5a0-4e42-9ade-dbdf815c07cd)

引用も確認してみます。テーブル形式でインデックスが構成されていることがわかります。

![image](https://github.com/user-attachments/assets/503a5947-b2d2-4ffc-9de1-d350c73e69cc)

以上、ご参考になれば幸いです。




