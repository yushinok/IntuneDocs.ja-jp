---
title: Mobile Threat Defense コネクタと Intune
titleSuffix: Intune on Azure
description: Pradeo Mobile Threat Defense コネクタと Intune を設定します。
keywords: ''
author: brenduns
ms.author: brenduns
manager: dougeby
ms.date: 06/27/2018
ms.topic: article
ms.prod: ''
ms.service: microsoft-intune
ms.technology: ''
ms.assetid: cde4d389-1770-4226-85a3-a2f3b3fb92a3
search.appverid: MET150
ms.openlocfilehash: bf08796be801e1947fc1b18f2b5d2c49a5db945d
ms.sourcegitcommit: 51b763e131917fccd255c346286fa515fcee33f0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/20/2018
ms.locfileid: "52179900"
---
# <a name="pradeo-mobile-threat-defense-connector-with-intune"></a>Mobile Threat Defense コネクタと Intune

Microsoft Intune に統合された Mobile Threat Defense (MTD) ソリューションである Pradeo によって実行されるリスク評価に基づき、条件付きアクセスを利用し、モバイル デバイスから会社のリソースへのアクセスを制御できます。 リスクは、Pradeo アプリを実行するデバイスから収集される製品利用統計情報に基づいて評価されます。

Intune デバイス コンプライアンス ポリシーで有効にした Pradeo リスク評価に基づき、条件付きアクセスのポリシーを構成できます。Intune デバイス コンプライアンス ポリシーは、検出された脅威に基づき、非準拠デバイスから企業リソースへのアクセスを許可したり、拒否したりするために利用できます。

## <a name="how-do-intune-and-pradeo-help-protect-your-company-resources"></a>Intune と Pradeo を利用し、会社のリソースをどのように保護しますか?

Android および iOS 向け Pradeo アプリは、ファイル システム、ネットワーク スタック、デバイスとアプリケーションの製品利用統計情報を可能な限り記録し、Pradeo クラウド サービスにテレメトリ データを送信し、モバイル デバイスの脅威に対するリスクを評価します。

Intune デバイス コンプライアンス ポリシーには、Pradeo リスク評価に基づく、Pradeo Mobile Threat Defense のルールが含まれています。 このルールを有効にすると、Intune は、有効にされたポリシーに基づいてデバイスの準拠状態を評価します。 デバイスが準拠していないことが判明した場合、ユーザーは Exchange Online や SharePoint Online などの会社リソースへのアクセスをブロックされます。 また、ユーザーは、デバイスにインストールされている Pradeo アプリから、問題を解決して会社リソースへのアクセスを回復するための案内を受け取ります。

## <a name="sample-scenarios"></a>サンプル事例

一般的なシナリオを次に示します。

### <a name="control-access-based-on-threats-from-malicious-apps"></a>悪意のあるアプリの脅威に基づいてアクセスを制御する

マルウェアなどの悪意のあるアプリがデバイスで検出されると、脅威が解決されるまで、デバイスで次の行為が禁止されます。

-   会社の電子メールに接続する

-   OneDrive for Work アプリを使用して会社のファイルを同期する

-   会社のアプリにアクセスする

**悪意のあるアプリが検出されたときにブロックする:**

![検出された悪意のあるアプリ](./media/pradeo_maliciousapps_blocked.png)

**修復後、アクセスが与えられる:**

![悪意のあるアプリの検出、アクセス権](./media/pradeo_maliciousapps_unblocked.png)

### <a name="control-access-based-on-threat-to-network"></a>ネットワークに対する脅威に基づいてアクセスを制御する

**Man-in-the-middle** 攻撃など、ネットワークに対する脅威を検出し、デバイスのリスクに基づいて Wi-Fi ネットワークへのアクセスを保護します。

**Wi-Fi 経由のネットワーク アクセスをブロックする:**

![Wi-Fi 経由のネットワーク アクセスをブロックする](./media/pradeo_network_wifi_blocked.png)

**修復後、アクセスが与えられる:**

![修復するとアクセス権が付与される](./media/pradeo_network_wifi_unblocked.png)

### <a name="control-access-to-sharepoint-online-based-on-threat-to-network"></a>ネットワークに対する脅威に基づいて SharePoint Online へのアクセスを制御する

**Man-in-the-middle** 攻撃など、ネットワークに対する脅威を検出し、デバイスのリスクに基づいて会社内のファイルの同期を阻止します。

**ネットワークの脅威が検出されたときに SharePoint Online をブロック:**

![ネットワークの脅威が検出されたときに SharePoint Online をブロック](./media/pradeo_network_spo_blocked.png)

**修復後、アクセスが与えられる:**

![SharePoint で修復時にアクセス権を付与する例](./media/pradeo_network_spo_unblocked.png)

## <a name="supported-platforms"></a>サポートされているプラットフォーム

-   **Android 4.0.3 以降**

-   **iOS 7 以降**

## <a name="prerequisites"></a>必要条件

-   Azure Active Directory Premium

-   Microsoft Intune サブスクリプション

-   Mobile Threat Defense サブスクリプション用の Pradeo のセキュリティ

    -   詳細については、[Pradeo の Web サイト](https://www.pradeo.com/en-US/mobile-threat-protection)を参照してください。

## <a name="next-steps"></a>次の手順

- [Pradeo と Intune を統合する](pradeo-mtd-connector-integration.md)

- [Pradeo アプリを設定する](mtd-apps-ios-app-configuration-policy-add-assign.md)

- [Pradeo デバイス コンプライアンス ポリシーを作成する](mtd-device-compliance-policy-create.md)

- [Pradeo MTD コネクタを有効にする](mtd-connector-enable.md)