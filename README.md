# FAQAgentSolution
AIによる FAQの生成、問い合わせ受付とAIによる回答案の作成、CSAT評価、多言語対応、作成したFAQのDataverse のファイルアップロードへの追加等の機能を提供する、FAQ管理とエージェントでのナレッジの最適化サイクルを回す包括的なソリューションです。

## ソリューションの概要
![image](https://github.com/user-attachments/assets/fa7b1ea1-c3ad-45ca-9977-75f95f62dced)


## ソリューションの仕組み

### 機能

### 機能

### 

## ソリューションの利用
### インポート方法

[最新のソリューションをダウンロード](https://github.com/geekfujiwara/FAQAgentSolution/releases/tag/FAQAgent)します。

ダウンロードしたソリューションをソリューションからインポートします。

![image](https://github.com/user-attachments/assets/4e7b8cbd-31d7-475d-b03b-b16036cbc451)


インポート時に接続の作成が求められますので作成します。

![image](https://github.com/user-attachments/assets/451f8c91-dc7a-48d8-81ff-5f8ca08cbac3)

マネージドソリューションをインポートした場合はマネージドのタブにソリューションがインポートされます。

![image](https://github.com/user-attachments/assets/86d0a48b-add0-4383-bca9-15ea12b4d595)

FAQ Agentを開きます。

![image](https://github.com/user-attachments/assets/2b25e130-2ef0-441d-83c8-aa2285105a3b)


インポートしたソリューションを開き、フローがオンになっていることを確認します。

![image](https://github.com/user-attachments/assets/df61832f-6a74-4cf5-b4b9-529ce8503397)


すべてのカスタマイズを公開します。

![image](https://github.com/user-attachments/assets/85478922-9793-416f-a566-2e79aa44b76b)

これでインポートは完了です。

### 利用方法

ソリューションは主にモデル駆動型アプリのFAQ管理アプリと、エージェントの2つで構成されています。

![image](https://github.com/user-attachments/assets/798fb153-fb87-49dc-b543-9e6c47d35144)

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

自動的にFAQから以下のような情報を出力して連携します。

![image](https://github.com/user-attachments/assets/99e4a89a-ba16-4f19-b286-0a9086f8a6c0)

>[!Note]
>ファイルアップロードのインデックスが完了するには時間を要します。しばらく待ってからエージェントへの問い合わせを行いようにしてください。

以上、ご参考になれば幸いです。




