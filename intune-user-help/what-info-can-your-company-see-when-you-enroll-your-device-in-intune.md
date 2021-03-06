---
title: デバイスを登録した場合に会社が確認できる情報
description: IT 部門でマネージド デバイスについて確認できることとできないことについて説明します。
keywords: ''
author: lenewsad
ms.author: lanewsad
manager: dougeby
ms.date: 11/06/2018
ms.topic: article
ms.prod: ''
ms.service: microsoft-intune
ms.technology: ''
ms.assetid: 12655728-a1af-4d89-97bc-925fe36c0dc4
searchScope:
- User help
ROBOTS: ''
ms.reviewer: esmich
ms.suite: ems
ms.openlocfilehash: 63295d7e05889f5a8beb44e399f36a4fbe27544d
ms.sourcegitcommit: 76c7b315b83eb6cb5b996facf1d250fb3e22f1bc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/08/2018
ms.locfileid: "51276117"
---
# <a name="what-information-can-my-organization-see-when-i-enroll-my-device"></a>デバイスを登録した場合に組織が確認できる情報

Microsoft Intune にデバイスを登録しても、組織はユーザーの個人情報を閲覧できません。 デバイスを登録すると、デバイスのモデルやシリアル番号など、デバイスに関する特定の情報を閲覧するアクセス許可が組織に付与されます。 組織はこの情報を使用して、デバイス上の会社データを保護します。

**組織が閲覧できない情報:**

- 通話と Web 閲覧の履歴
- 電子メールとテキスト メッセージ
- 連絡先
- 予定表
-   パスワード
- フォト アプリやカメラ ロールの内容を含む、画像
- ファイル

**組織が常に閲覧できる情報:**

- デバイス モデル (例: Google Pixel)
- デバイスの製造元 (例: Microsoft)
- オペレーティング システムとバージョン (例: iOS 12.0.1)
- アプリ名 (例: Microsoft Word): 個人用デバイスでは、組織はマネージド アプリ インベントリのみを閲覧できます。 会社が所有しているデバイスでは、組織はすべてのアプリ インベントリを閲覧できます。
- デバイスの所有者
- デバイス名
- デバイスのシリアル番号
- IMEI

**組織が閲覧できる可能性がある情報:**

-  電話番号: **会社**が所有するデバイスの場合は、ユーザーの電話番号を確認できます。 **個人**が所有するデバイスの場合、組織が確認できるのは、ユーザーの電話番号の最後の 4 桁のみです。 個々のデバイスの**所有権の種類**を確認するには、デバイスの **[デバイスの詳細]** ページを開きます。
- デバイスの記憶域スペース: 必要なアプリをインストールできない場合、組織がユーザーのデバイスの記憶域スペースを確認し、スペースが少なすぎるかどうかを判断することがあります。  
-  場所: 監視対象となっている iOS デバイスを紛失した場合を除き、組織はユーザーのデバイスの場所を確認できません。 [確認方法](https://go.microsoft.com/fwlink/?linkid=853816)
- アプリ インベントリ: 組織で Mobile Threat Defense を使っている場合、iOS デバイス上のアプリの詳細を見ることができます。 Mobile Threat Defense の詳細については、[こちら](you-are-prompted-to-install-mtd-ios.md)をご覧ください。
- ネットワーク情報: Android デバイスのネットワーク接続情報の一部は、組織のサポートが確認できる場合があります。 たとえば、デバイスを特定の建物内に維持するように組織が定めている場合、デバイスでは接続先のネットワークが識別されます。 
