---
title: Azure Portal での Microsoft Intune の概要
titlesuffix: ''
description: Azure Portal の Microsoft Intune でダッシュボードを作成、共有、および移動する方法について説明します。
keywords: ''
author: dougeby
ms.author: dougeby
manager: dougeby
ms.date: 02/26/2018
ms.topic: article
ms.prod: ''
ms.service: microsoft-intune
ms.technology: ''
ms.assetid: 917c0eed-96d0-49d8-8db8-a6ba13ad0e1f
ms.reviewer: ''
ms.suite: ems
search.appverid: MET150
ms.custom: intune-azure
ms.openlocfilehash: 1b22840429224b70ddaaf5d77f850c4d4af8b5e2
ms.sourcegitcommit: 51b763e131917fccd255c346286fa515fcee33f0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/20/2018
ms.locfileid: "52180903"
---
# <a name="getting-started-with-microsoft-intune-in-the-azure-portal"></a>Azure Portal での Microsoft Intune の概要

Azure Portal は、Microsoft Intune サービスのある場所です。 Azure にはさまざまなサービスがありますが、その多くはおそらく、日常的に使用されることがありません。 Azure でダッシュボードとサイドバーをカスタマイズすれば、いつログインしても必要な情報がすぐに見つかり、Intune でデバイスを管理できます。

## <a name="changing-the-sidebar"></a>サイドバーを変更する

Azure Portal の左側にある__サイドバー__には、利用できるすべての Azure サービスの一覧が表示されます。 この包括的な一覧は既定以外の表示に変更できます。自分にとって最も重要なサービスを常に表示しておくことができます。 次の情報では、サービスの例として Intune を利用し、一覧の一番上に追加します。

![あるユーザーが 'その他のサービス' 一覧で Microsoft Intune を探しています。](./media/azure-add-intune1.png)

1. ページの左側にあるサイドバーから **[すべてのサービス]** を選択します。
2. フィルター ボックスで **Intune** を検索します。
3. **星**マークを選択し、お気に入りサービス一覧の一番下に Intune を追加します。
4. Intune サービスの上にカーソルを合わせます。 Intune を選択してドラッグします。サービス名の右側にある **3 つの垂直ドット**を利用します。

## <a name="changing-the-dashboard"></a>ダッシュボードの変更

既定のランディング ページは**ダッシュボード**です。 このページで、タイルをカスタマイズし、自分にとって最も重要な情報を表示します。

![一般的な新しいダッシュボードのイメージ。 すべてのサービスを含むサイドバーが左に、メインのダッシュボードが中央に表示されます。 ダッシュボードの変更ボタンは上にあります。タイルからすべてのリソース、クイックスタート チュートリアル、サービス正常性、Azure Marketplace にアクセスできます。](./media/azure-default-dashboard.png)

現在のダッシュボードを変更するには、**[ダッシュボードの編集]** ボタンを選択します。 既定のダッシュボードを変更しなくても、**新しいダッシュボード**を作成できます。 新しいダッシュボードを作成すると、**タイル ギャラリー**がある空のプライベート ダッシュボードが与えられ、そこでタイルを追加したり再編成できます。 **全般**カテゴリや**種類**に基づいて、あるいは**検索**、**リソース グループ**、**タグ**を利用してタイルを検索できます。

また、**省略記号**ボタンからダッシュボードに直接、タイルを追加できます。**[ダッシュボードにピン留めする]** を選択します。

![Intune の [ユーザーとグループ - すべてのグループ] の拡大画面。グループの右端で "ダッシュボードにピン留めする" オプションを確認できます。](./media/azure-pin-to-dashboard.png)

この機能は、Intune にグループやユーザーなどのコンテンツを追加した後に重要になります。

## <a name="using-services"></a>サービスの使用

Intune やその他のサービスを Azure で開くたびに、サービスは**ウィンドウ**に表示されます。 **ユーザー**、**グループ**、**クライアント アプリ**など、Intune で最初に使用するワークロードはすべて、全画面ウィンドウで表示されます。 ワークロードを選択すると、そのウィンドウが全画面で開きます。 他のウィンドウは開くときにウィンドウの右側から引き出され、メイン ウィンドウの下で折りたたまれます。

## <a name="next-steps"></a>次の手順

* [ユーザー管理の概要](get-started-users.md) - Intune にユーザーを追加し、モバイル デバイスで会社のリソースにアクセスできるようにします。
