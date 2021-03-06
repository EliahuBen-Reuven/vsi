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

# 専用ホストおよび専用インスタンスのプロビジョニング
{: #ordering-vs-dedicated}

専用インスタンスをプロビジョンする方法には、2 つの選択肢があります。1 つ目は {{site.data.keyword.Bluemix}} カタログを使用する方法で、2 つ目は {{site.data.keyword.slportal_full}}を使用する方法です。カタログと{{site.data.keyword.slportal}}には、固有のログイン ID が必要です。カタログのユーザー名とパスワードはポータルへのログインには使用できず、ポータルのユーザー名とパスワードはカタログのログインには使用できません。
{{site.data.keyword.Bluemix_notm}} カタログまたは{{site.data.keyword.slportal}}の資格情報をセットアップするには、[{{site.data.keyword.Bluemix_notm}} への登録](https://console.bluemix.net/docs/admin/adminpublic.html#signing-up-for-bluemix){: new_window}を参照してください。
{:shortdesc}

## Bluemix カタログへのログイン
{{site.data.keyword.Bluemix_notm}} カタログにログインして専用ホストと専用ホスト・インスタンスのプロビジョニングを開始するには、以下のステップを使用します。 

1. 新しいブラウザー・ウィンドウを開き、[https://console.ng.bluemix.net/catalog/](https://console.ng.bluemix.net/catalog/){: new_window} と入力します。
2.	**「ログイン」**リンク (右上隅) をクリックします。 
3.	E メールまたは IBM ID を入力して**「続行」**をクリックします。
4.	パスワードを入力して**「ログイン」**をクリックします。
5.	**「インフラストラクチャー」>「コンピュート」**と選択します。
6.  **「仮想サーバー」**タイルをクリックします。
7.	**「専用仮想サーバー」**オプションを選択します。
8.  **「作成」**をクリックします。 

{{site.data.keyword.slportal}}のメインページが表示されます。

## カスタマー・ポータルへのログイン
{{site.data.keyword.slportal}}にログインして専用ホストと専用ホスト・インスタンスの注文を開始するには、以下のステップを使用します。

1.	新しいブラウザー・ウィンドウを開き、[https://control.softlayer.com](https://control.softlayer.com){: new_window} と入力します。 
2.	ユーザー名とパスワードを入力し、**「ログイン」**をクリックするか、**「IBM ID でログイン」**をクリックします。
3.	E メールまたは IBM ID を入力して**「続行」**をクリックします。
4.	パスワードを入力して**「ログイン」**をクリックします。

{{site.data.keyword.slportal}}のメインページが表示されます。

## 専用ホストのプロビジョニング 
専用ホストをプロビジョンするには、以下のステップを使用します。

1.	**「デバイス」**アイコンをクリックします。
2.  **「専用仮想サーバー (時間単位) (Dedicated Virtual Server Hourly)」**または**「専用仮想サーバー (月単位) (Dedicated Virtual Server Monthly)」**のリンクをクリックします。 

   **注:** 専用サーバーはプライベート・サーバーです。

*「クラウド・サーバーの構成」*ページが開きます。このページから、専用ホストに関連付けられた専用インスタンスも、関連付けられていない専用インスタンスもオーダーできます。インスタンスのオーダーの詳細は、[専用ホスト・インスタンスのプロビジョニング]{: provision-dedicated-instances}に記載されています。

4.	フォームの右側にある**「ホストの作成」**ボタンをクリックします。
5.	次の情報を入力します。
    
    <table>
    <CAPTION>表 1. 専用ホストのプロビジョニングの選択</CAPTION>
    <THEAD>
    <TR>
    <th>フィールド</th>
    <th>値</th>
    </TR>
    </THEAD>
    <TBODY>
    <tr>
    <td>数量</td>
    <td>オーダーする専用ホストの数を入力します。1 つのプロビジョニング・オーダーにつきデプロイ可能な専用ホストは 2 つのみである点に留意してください。</td>
    </tr>
    <tr>
    <td>場所</td>
    <td>ホストを配置する {{site.data.keyword.cloud}} データ・センターを選択します。利用可能なデータ・センターのリストについては、製品情報を参照してください。</td>
    </tr>
    <td>専用ホスト</td>
    <td>デフォルトで、56 コア X 242 RAM X 1.2 TB</td>
    </tr>
    </TBODY>
    </table>
    
    *「構成」*ページの右側にオーダーのサマリーが表示されます。 
    
6.  **「注文に追加」**ボタンをクリックします。
7.  *「チェックアウト」*ページで選択内容を確認し、*「専用ホストの拡張システム構成 (Dedicated Host Advanced System Configuration)」*までスクロールダウンします。
8.  次の情報を入力します。

    <table>
    <CAPTION>表 2. 専用ホストの拡張システム構成</CAPTION>
    <THEAD>
    <TR>
    <th>フィールド</th>
    <th>値</th>
    </TR>
    </THEAD>
    <TBODY>
    <tr>
    <td>POD 選択</td>
    <td>ドロップダウン・ボックスをクリックし、専用ホストを配置する POD を選択します。</td>
    </tr>
    <tr>
    <td>ホスト名</td>
    <td>サーバーの永続的または一時的な名前を入力します。例えば、server1 などです。</td>
    </tr>
    <tr>
    <td>ドメイン</td>
    <td>インターネットのドメイン名と競合しないサブドメイン名を入力します。例えば、test.acme.com などです。</td>
    </tr>
    </TBODY>
    </table>

9.  **「クラウド・サービスのご利用条件」**チェック・ボックスをクリックします。
10. 支払情報を確認または入力し、**「送信」**ボタンをクリックします。プロビジョニング注文番号が示された画面にリダイレクトされます。この画面は、プロビジョニングの注文の受信を示すものでもあるため、印刷できます。

    プロビジョニング注文の確認、プロビジョニング注文の承認と処理、プロビジョニングの完了を示す一連の E メールが管理者に送信されます。プロビジョニング完了 E メールには、{{site.data.keyword.Bluemix_notm}} へのログイン後に**「デバイスの詳細」**ページに直接移動するためのリンクが含まれています。もう 1 つの選択肢として、{{site.data.keyword.slportal}}への直接ログインがあります。

## 専用ホスト・インスタンスのプロビジョニング
{: #provision-dedicated-instances}
専用ホスト・インスタンスのプロビジョニングは、**「デバイス」**メニューを使用するか、**「デバイス」**アイコンを使用するという 2 つの方法で行うことができます。

### デバイス・メニューを使用した専用ホスト・インスタンスのプロビジョニング
{: #ordering-dedicated-devices-menu}

1 つ目のオプションは、{{site.data.keyword.slportal}}のメインページの**「デバイス」**メニューを使用して専用ホスト・インスタンスをプロビジョンする方法です。以下のステップで、このプロセスを説明します。

1.	**「デバイス」>「デバイス・リスト」**をクリックします。 
 
    *「デバイス」* ページに、ユーザーのアカウント内のすべてのデバイス・タイプ (専用ホスト、仮想サーバー、ベア・メタル・サーバー、および NetScaler アプリケーション・デリバリー・コントローラー) が表示されます。 

2.	**「デバイス名」**の下のリンクをクリックして、専用ホスト・インスタンスのホストを選択します。
    
    *「デバイス詳細」*ページの**「構成」**タブが表示されます。**「チケット」**タブには、アクティブ・サポート・チケットがリストされ、**「割り振り」**タブには、選択した請求対象期間のメモリー使用量が表示されます。これらのタブの詳細情報については、「デバイス詳細を使用した専用ホストおよびインスタンスの管理」を参照してください。

3.	**「インスタンス」**フレームまでスクロールダウンします。

    専用ホストの請求処理方法 (月単位または時間単位) は、専用ホスト・インスタンスの請求処理を決定します。月単位で請求処理されるホストを使用する場合は、時間単位で請求処理されるホスト・インスタンスと月単位で請求処理される専用ホスト・インスタンスの両方をプロビジョンできることに留意してください。インスタンスをプロビジョンする時、**「時間単位の追加 (Add hourly)」**と**「月単位の追加 (Add monthly)」**という 2 つのリンクが使用可能になります。時間単位で請求処理される専用ホストがプロビジョンできるのは、時間単位で請求処理される専用ホスト・インスタンスのみのため、**「時間単位の追加 (Add hourly)」**リンクのみが表示されます。 

4.	ホストが時間単位または月単位で請求処理される場合は、**「時間単位の追加 (Add hourly)」**リンクをクリックします。ホストが月単位で請求処理される場合は、**「月単位の追加 (Add monthly)」**リンクをクリックします。*「クラウド・サーバーの構成」*ページにリダイレクトされます。 

5.	次の情報を入力します。
       
    <table>
    <CAPTION>表 3. 専用ホスト・インスタンスの選択</CAPTION>
    <THEAD>
    <TR>
    <th>フィールド</th>
    <th>値</th>
    </TR>
    </THEAD>
    <TBODY>
    <tr>
    <td>数量</td>
    <td>単一ホストにデプロイされる専用ホスト・インスタンスの数。</td>
    </tr>
    <tr>
    <td>配置</td>
    <td>
    <ul>
    <li>自動割り当て – ユーザーがホストを指定するのに対して、自動割り当てでは、{{site.data.keyword.Bluemix_notm}} が自動的にインスタンスをホストに割り当てます。インスタンスは、容量があるデータ・センターに配置されます。インスタンスの自動割り当てを行う場合、専用ホストの容量はまったく使用されません。</li>
    <li>ホストの指定 – アカウントに関連付けられている専用ホストは、専用ホストの下に表示されます。</li>
    </ul>
    </td>
    </tr>
    <tr>
    <td>専用ホスト</td>
    <td>インスタンスのプロビジョン先のリストから専用ホストを選択します。</td>
    </tr>
    <tr>
    <td>コンピューティング・インスタンス</td>
    <td> プロビジョニングの注文内の各インスタンスについて、メモリーと CPU を選択します。</td>
    </tr>
    <tr>
    <td>RAM</td>
    <td> プロビジョニングの注文内の各インスタンスについて、RAM を選択します。</td>
    </tr>
    <tr>
    <td>オペレーティング・システム</td>
    <td>インスタンスのオペレーティング・システムを選択します。サーバーとオペレーティング・システムの間で矛盾がある場合、エラー・メッセージが発行されます。例えば、Microsoft SQL Server で Linux を選択する場合です。</td>
    </tr>
    <tr>
    <td>1 番目のディスク</td>
    <td>注文内の各インスタンスについて、「SAN」または「ローカル」を選択します。</td>
    </tr>
    <tr>
    <td>追加のディスク</td>
    <td>1 つの専用ホスト・インスタンスにつき、最大 4 つの追加ブート・ディスク (SAN またはローカル) をプロビジョンできます。</td>
    </tr>
    <td>ネットワーク・オプション</td>
    <td> 該当のオプションを選択するか、デフォルト値を使用します。</td>
    </tr>
    <tr>
    <td>アドオン</td>
    <td> 該当のオプションを選択するか、デフォルト値を使用します。</td>
    </tr>
    <tr>
    </TBODY>
    </table> 

6.	**「注文に追加」**ボタンをクリックします。
7.  *「清算」*ページで*「拡張システム構成」* の下に、次の情報を入力します。

<table>
    <CAPTION>表 4. 専用ホスト・インスタンスの拡張システム構成</CAPTION>
    <THEAD>
    <TR>
    <th>フィールド</th>
    <th>値</th>
    </TR>
    </THEAD>
    <TBODY>
    <tr>
    <td>VLAN の選択</td>
    <td>少なくとも 1 台のサーバーを注文済みの場合は、ご使用のアカウントで VLAN に新しいサーバーを追加します。</td>
    </tr>
    <tr>
    <td>プロビジョン・スクリプト</td>
    <td>プロビジョニング後の一定のステップを自動化できるスクリプトを指定します。</td>
    </tr>
    <tr>
    <td>SSH 鍵</td>
    <td>SSH 鍵の公開鍵を指定します。これにより、サーバーのプロビジョン後にサーバーにログインできます。</td>
    </tr>
    <tr>
    <td>ユーザー・メタデータ</td>
    <td>カスタム・プロビジョニング・スクリプトのオプション・メタデータ。</td>
    </tr>
    <tr>
    <td>ホスト名</td>
    <td>サーバーの永続的または一時的な名前を入力します。例えば、server1 などです。</td>
    </tr>
    <tr>
    <td>ドメイン</td>
    <td>インターネットのドメイン名と競合しないサブドメイン名を入力します。例えば、test.acme.com などです。</td>
    </tr>
    </TBODY>
    </table>

8.  **「クラウド・サービスのご利用条件」**と**「サード・パーティー・サービス契約」**のチェック・ボックスをクリックします。
9. 支払情報を確認または入力し、**「送信」**ボタンをクリックします。プロビジョニング注文番号が示された画面にリダイレクトされます。この画面は、プロビジョニングの注文の受信を示すものでもあるため、印刷できます。


専用ホスト・インスタンスがプロビジョンされると E メールを受け取ります。

### 「デバイス」アイコンによる専用ホスト・インスタンスのプロビジョニング
専用ホスト・インスタンスをプロビジョンするための 2 つ目のオプションは、{{site.data.keyword.slportal}}のホーム・ページの**「デバイス」**アイコンを使用する方法です。以下のステップで、このプロセスを説明します。

1.	**「デバイス」**アイコンをクリックし、専用仮想サーバーの下で**「時間単位 (Hourly)」** または**「月単位 (Monthly)」**を選択します。
2.	[「デバイス・メニューを使用した専用ホスト・インスタンスのプロビジョニング」](#ordering-dedicated-devices-menu)のステップ (ステップ 5 から) に従います。

### 次のステップ
仮想サーバーがプロビジョンされたら、その管理を開始できます。詳しくは、[仮想サーバーの管理](../vsi/vsi_managing.html)を参照してください。


