# Bright Dataのスクレイピング用プロキシ

[![Promo](https://github.com/bright-jp/Rotating-Residential-Proxies/blob/main/50%25%20off%20promo.png)](https://brightdata.jp/proxy-types) 

## Bright Dataについて
Bright Dataは、世界中で20,000社以上のお客様にサービスを提供する、受賞歴のある業界トップクラスのプロキシプロバイダーです。1億以上のプロキシIP、クラス最高水準のテクノロジー、そして任意の国・都市・キャリア・ASNをターゲット可能な機能により、当社のプロキシサービスは開発者の皆様にとって最適な選択肢となっています。

## レジデンシャルプロキシ
正確なターゲティング、比類のない安定性、そして高速なレスポンス時間を提供するよう設計されたBright Dataの[スクレイピング用プロキシ](https://brightdata.jp/solutions/scraping-proxy)で、シームレスなスクレイピングを体験してください。

- **72M+ レジデンシャルIP**
- **Stickyセッションおよびローテーティングセッション**
- **成功率 99.95%**
- **HTTP(S) & SOCKS5対応**
- **ジオロケーションターゲティング（無料）**

## 主な特長
- **グローバルカバレッジ**: [195か国](https://brightdata.jp/locations)で利用可能なレジデンシャルプロキシです。
- **高い成功率**: スクレイピングプロジェクトで最大99.95%の成功率を実現します。
- **高速レスポンス**: 平均レスポンス時間は約0.7秒です。
- **倫理的に取得**: すべてのプロキシは、明示的なユーザー同意のもとで取得されています。
- **同時接続セッション無制限**: 制限なく運用をスケールできます。

## 料金プラン
- **従量課金**: $8.4/GB、月額契約は不要です。
- **月額サブスクリプション**:
  - **69 GB**: $7.14/GB、$499/月。
  - **158 GB**: $6.3/GB、$999/月。
  - **339 GB**: $5.88/GB、$1999/月。
  - **Enterprise Plans**: 大規模ニーズ向けにカスタムソリューションをご用意しています。

[![Promo](https://github.com/bright-jp/LinkedIn-Scraper/blob/main/Proxies%20and%20scrapers%20GitHub%20bonus%20banner.png)](https://brightdata.jp/proxy-types) 

## レジデンシャルプロキシの利用開始
1. **無料トライアルを開始**: クレジットカードは不要です。
2. **統合**: APIまたはControl Panelを使用して、IPや設定を管理します。
3. **対応言語**: Python、Java、C#、Node.js、Shell向けにクイックスタート例をご用意しています。

## コード例

### Python

```python
import sys

# Replace '[your customerID]', 'residential', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335',
             'https': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335',
             'https': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 33335);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-residential", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:33335");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-residential", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335',
})
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:33335 --proxy-user brd-customer-[your customerID]-zone-residential:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

## モバイルプロキシ
世界中の数百万の3G、4G、5GのIPを備えたBright Dataの[モバイルプロキシネットワーク](https://brightdata.jp/proxy-types/mobile-proxies)で、実際のモバイルユーザーとしてインターネットにアクセスできます。

- **7,000,000+ モバイルIP**
- **3G/4G/5G モバイルIP**
- **24/7サポートによる稼働率 99.99%**
- **ジオロケーションターゲティング（無料）**

## 主な特長
- **グローバル対応**: [195か国](https://brightdata.jp/locations)のモバイルIPにアクセスできます。
- **高い成功率**: データ収集およびテスト作業で最大99.9%の成功率を実現します。
- **実際のモバイル接続**: モバイルIPは、実デバイスおよび実ネットワークから取得されています。
- **無制限のスケーリング**: 同時接続セッションと高可用性インフラによりスケールできます。
- **キャリアレベルのターゲティング**: 特定のキャリアを指定して、深く正確なインサイトを得られます。

## 料金プラン
- **従量課金**: $8.4/GB、月額契約なしで利用できます。
- **月額サブスクリプション**:
  - **69 GB**: $7.14/GB、$499/月 + VAT。
  - **158 GB**: $6.3/GB、$999/月 + VAT。
  - **339 GB**: $5.88/GB、$1999/月 + VAT。
  - **Enterprise Plans**: カスタム料金およびパッケージをご用意しています。

今すぐ登録して、初回入金額に対して最大$500まで同額マッチを獲得しましょう！

## モバイルプロキシの利用開始
1. **無料トライアルを開始**: クレジットカードは不要です。
2. **統合**: APIまたはBright Data Control Panelを使用して、IPや設定を管理します。
3. **対応言語**: Python、Java、C#、Node.js、Shell向けにクイックスタート例をご用意しています。

## コード例

### Python

```python
import sys

# Replace '[your customerID]', 'mobile', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 22225);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-mobile", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:22225");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-mobile", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225',
})
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell 

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:22225 --proxy-user brd-customer-[your customerID]-zone-mobile:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

## ISPプロキシ
ISPから直接取得されたIPを用いて、安全で安定した高速データ収集を実現するBright Dataの広範な[ISPプロキシネットワーク](https://brightdata.jp/proxy-types/isp-proxies)をご活用ください。

- **700,000+ ISP IP**
- 長期的な安定性を備えた**スタティック レジデンシャルIP**
- **成功率 99.9%**
- **HTTP(S) & SOCKS5対応**
- **国レベルのターゲティング無料**

## 主な特長
- **グローバル対応**: [複数の国](https://brightdata.jp/locations)にわたるISP IPにアクセスできます。
- **高い成功率**: Webサイトへのアクセスで最大99.9%の成功率です。
- **高速かつ安定**: 低レイテンシーと信頼性の高い稼働率（ネットワーク可用性99.99%）を提供します。
- **専用IPアクセス**: 一貫した接続のための専用IPを提供します。
- **倫理的に取得**: すべてのISPプロキシはISPから直接取得され、GDPRおよびCCPAに準拠しています。

## 料金プラン
- **従量課金**: $15/GB、月額契約なしで利用できます。
- **月額サブスクリプション - Shared**:
  - **10 IPs**: $1.80/IP、$18/月 + VAT。
  - **100 IPs**: $1.45/IP、$145/月 + VAT。
  - **500 IPs**: $1.40/IP、$700/月 + VAT。
  - **1,000 IPs**: $1.30/IP、$1300/月 + VAT。
  - **Enterprise Plans**: 大規模なデータ収集ニーズ向けにカスタムソリューションをご用意しています。
 
- **月額サブスクリプション - Dedicated**:
  - **10 IPs**: $3.50/IP、$35/月 + VAT。
  - **100 IPs**: $2.75/IP、$275/月 + VAT。
  - **500 IPs**: $2.60/IP、$1300/月 + VAT。
  - **1,000 IPs**: $2.50/IP、$2500/月 + VAT。
  - **Enterprise Plans**: 大規模なデータ収集ニーズ向けにカスタムソリューションをご用意しています。
 
- **月額サブスクリプション - Pay/GB**:
  - $12.75/GB、$499/月 + VAT。
  - $11.25/GB、$999/月 + VAT。
  - $10.50/GB、$1999/月 + VAT。
  - **Enterprise Plans**: 大規模なデータ収集ニーズ向けにカスタムソリューションをご用意しています。


## ISPプロキシの利用開始
1. **無料トライアルを開始**: クレジットカードは不要です。
2. **統合**: Bright DataのControl PanelまたはAPIを通じて、IPと設定を管理します。
3. **対応言語**: Python、Java、C#、Node.js、Shell向けにクイックスタートガイドをご用意しています。

## コード例

### Python

```python
import sys

# Replace '[your customerID]', 'isp', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 22225);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-isp", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:22225");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-isp", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225',
})
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:22225 --proxy-user brd-customer-[your customerID]-zone-isp:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

## データセンタープロキシ
信頼性の高いデータ収集とWebスクレイピングのために、比類のないスケールと速度を備えたBright Dataの広範な[データセンタープロキシネットワーク](https://brightdata.jp/proxy-types/datacenter-proxies)をご活用ください。

- **770,000+ データセンターIP**
- **[Shared](https://brightdata.jp/solutions/shared-proxies)および[Dedicated](https://brightdata.jp/solutions/dedicated-proxies)のIPオプション**
- **平均レスポンス時間 約0.24秒**
- **HTTP(S) & [SOCKS5](https://brightdata.jp/solutions/socks5-proxies)対応**
- **国レベルのターゲティング無料**

## 主な特長
- **グローバル対応**: [98か国](https://brightdata.jp/locations)のデータセンターIPにアクセスできます。
- **高い成功率**: スクレイピング作業で最大99.9%の成功率を実現します。
- **高速かつ信頼性**: ネットワーク稼働率99.99%と高速な接続速度を提供します。
- **カスタマイズ可能なオプション**: ニーズに応じてSharedまたはDedicatedのIPを選択できます。
- **無制限のスケーリング**: 制限なしで同時接続セッションをサポートします。

## 料金プラン
- **従量課金**: $0.6/GB、月額契約なしで利用できます。
- **月額サブスクリプション - Shared**:
  - **10 IPs**: $1.40/IP、$14/月 + VAT。
  - **100 IPs**: $1.00/IP、$100/月 + VAT。
  - **500 IPs**: $0.95/IP、$475/月 + VAT。
  - **1,000 IPs**: $0.90/IP、$900/月 + VAT。
  - **Enterprise Plans**: 大規模なデータ収集向けに最適化したソリューションをご提供します。

- **月額サブスクリプション - Dedicated**:
  - **10 IPs**: $2.20/IP、$22/月 + VAT。
  - **100 IPs**: $1.70/IP、$170/月 + VAT。
  - **500 IPs**: $1.50/IP、$750/月 + VAT。
  - **1,000 IPs**: $1.30/IP、$1300/月 + VAT。
  - **Enterprise Plans**: 大規模なデータ収集向けに最適化したソリューションをご提供します。


- **月額サブスクリプション - Pay/GB**:
  - $0.51/GB、$499/月 + VAT。
  - $0.45/GB、$999/月 + VAT。
  - $0.42/GB、$1999/月 + VAT。
  - **Enterprise Plans**: 大規模なデータ収集向けに最適化したソリューションをご提供します。

登録して、初回入金額に対して最大$500まで同額マッチを獲得しましょう！

## データセンタープロキシの利用開始
1. **無料トライアルを開始**: クレジットカードは不要です。
2. **統合**: APIまたはBright Data Control PanelでIPと設定を管理します。
3. **対応言語**: Python、Java、C#、Node.js、Shell向けにクイックスタートガイドをご用意しています。

## コード例

### Python

```python
import sys

# Replace '[your customerID]', 'datacenter', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 22225);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-datacenter", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:22225");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-datacenter", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225',
    })
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:22225 --proxy-user brd-customer-[your customerID]-zone-residential:[your password] -k "https://geo.brdtest.com/mygeo.json"
```
### 今すぐ[Bright Data](https://brightdata.jp)に参加して、当社が業界リーダーである理由をご確認ください。