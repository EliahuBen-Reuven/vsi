---



copyright:
  years: 2017
lastupdated: "2017-10-24"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}


# 既存の仮想サーバーの再構成
{: #reconfiguring-virtual-servers}

仮想サーバーがプロビジョンされた後、いつでもその構成をアップグレードまたはダウングレードすることができます。  

**重要な注:** 事前設定フレーバーではさまざまなパブリック仮想サーバーが使用可能です。期間限定で、事前設定フレーバーの前に使用可能だった仮想サーバーをどれでも変更することができます。次に、既存のインスタンスをマイグレーションまたはキャンセルし、リオーダーする必要があります。 

フレーバーを使用する仮想サーバーの個別のコア、RAM、およびディスク・サイズを変更することはできません。自分が必要とする事前設定コア、RAM、およびディスク・サイズを持つ別のフレーバーを選択する必要があります。選択する仮想サーバー・フレーバーによって、有効なコア、RAM、およびディスク・サイズが決まります。  

専用仮想サーバーは、よりカスタマイズ可能なため、個別のコア、RAM、およびディスク・サイズを変更できます。

既存の仮想サーバーを再構成するには、以下のステップを使用します。
{:shortdesc}

## (事前設定フレーバーを使用する) 既存の仮想サーバーの変更
1. ユーザー固有の資格情報を使用して、[{{site.data.keyword.slportal_full}} ![「外部リンク」アイコン](../icons/launch-glyph.svg "「外部リンク」アイコン")](https://control.softlayer.com/) にアクセスします。 
2. デバイス・リストから、再構成する仮想サーバーの名前をクリックします。
3. **「構成」**タブで**「変更」**または**「デバイス構成の変更」**をクリックして、以下の項目を更新することができます。 
  <dl>
  <dt>サイズ</dt>
  <dd>新しいサイズを選択します。</dd>
  <p><note>注: ローカル・ストレージを使用するフレーバーを変更する場合、非ローカル・ストレージを使用するフレーバーに切り替えることはできません。同様に、非ローカル・ストレージを使用するフレーバーを変更する時は、ローカル・ストレージを使用するフレーバーに切り替えることはできません。
  </note></p>
  </dl>
4. 仮想サーバーの変更を指定したら、構成の更新を完了します。
  <dl>
  
  <dt>アップグレード日付</dt>
  <dd>即時更新するための「即時」チェック・ボックスをクリックするか、更新をアクティブにする時刻をスケジュールに入れることができます。</dd>

  <dt>アップグレード時刻</dt>
  <dd>更新をアクティブにする日付 (YYYY-MM-DD) を入力します。</dd>

  <dt>メモ</dt>
  <dd>デバイスについて該当するメモを入力します。</dd>
  </dl>

5. **「続行」**をクリックします。
6. オーダーの確認で正確性を確認します。アップグレードを編集するには、**「編集」**をクリックします。
7. **「確認」**をクリックしてオーダーを確認し、デバイスに変更を適用します。

## (事前設定フレーバーの前の) 既存の仮想サーバー、または専用仮想サーバーの変更
1. デバイス・リストから、再構成する仮想サーバーの名前をクリックします。
2. **「構成」**タブで、**「コアまたは RAM のアップグレード (Core or RAM upgrade)」**リンクをクリックして、以下の項目を更新することができます。 
  
|   アップグレードのオプション       |  説明                                                                                              |
| ----------------------- | ----------------------------------------------------------------------------------------------------------- |
| アップグレードの日付            | 更新をアクティブにする日付 (YYYY-MM-DD) を入力します。|
| アップグレード時刻            | 更新をアクティブにする日の時刻をドロップダウン・ボックスから選択するか、即時更新するために**「即時」**チェック・ボックスをクリックします。|
| コア| 該当する場合、更新するコアの数を選択します。|
| RAM| 該当する場合、更新するデバイスに適用する RAM の量を選択します。|
| アップリンク・ポート速度      | 該当する場合、デバイスの新しいアップリンク・ポート速度を選択します。|
| パブリック帯域幅        | 該当する場合、デバイスのパブリック処理能力の量 (GB 単位) を選択します。|
| 1 番目のディスク – 5 番目のディスク | 該当する場合、1 番目のディスクのディスク・スペースまたはストレージのオプションを選択します。詳しくは、下記の**ディスクの注**を参照してください。                                                                                                  |
| メモ| デバイスについて該当するメモを入力します。|
{: caption="表 1. デプロイメント・オプション" caption-side="top"}   
  
  **ディスクの注:**
  * ローカル・ストレージと SAN ストレージの両方が使用可能です。選択した項目を入念にチェックして、ストレージ・オプションが正しいことを確認してください。
  * パブリック仮想サーバーでは、ローカル・ストレージをアップグレードするときに、より多くのコアまたは RAM が必要な場合、2 次ディスクを失う可能性があります。ローカル・ストレージを使用する仮想サーバー・フレーバーを変更する場合、フレーバーはユーザー用に事前設定されているため、同等でないフレーバーを選択することはできません。
3. **「続行」**をクリックします。
4. オーダーの確認で正確性を確認します。アップグレードを編集するには、**「編集」**をクリックします。
5. **「確認」**をクリックしてオーダーを確認し、デバイスに変更を適用します。
