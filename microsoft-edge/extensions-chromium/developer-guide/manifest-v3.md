---
title: Overview of Manifest V3
description: Migrating from Manifest V2 to V3 will help reduce fragmentation of the web for developers and enhance privacy, security, and performance for end users.
author: MSEdgeTeam
ms.author: msedgedevrel
ms.topic: conceptual
ms.prod: microsoft-edge
ms.technology: extensions
ms.date: 3/11/2022
---
# Overview of Manifest V3

A manifest file is the blueprint of an extension. It includes information such as the version number of the extension, the title of the extension, and permissions needed to run the extension. Migrating from Manifest V2 to V3 will bring several structural changes to how extensions are handled by the browser.

In October 2020, Microsoft announced the [decision to embrace Manifest V3](https://blogs.windows.com/msedgedev/2020/10/14/extension-manifest-chromium-edge/) to help reduce fragmentation of the web for all developers and enhance privacy, security, and performance for end users.

Manifest V3 is an initiative of the [Chromium project](https://www.chromium.org/Home/). Manifest V2 support ends in June of 2023 for all Chromium-based browsers.

An overview of the changes involved, as described in [Overview of Manifest V3 - Chrome Developers](https://developer.chrome.com/docs/extensions/mv3/intro/mv3-overview/):

* Service workers will replace background pages.

* Network request modifications will be handled by the new `declarativeNetRequest` API.

* Remotely hosted code will no longer be allowed. An extension will only be able to execute JavaScript that is included within its own package.

* Promise support will be added to many methods. Callbacks will still be supported as an alternative.

* A number of minor feature improvements will also be introduced in Manifest V3.

To help you plan, consider the following schedule for Microsoft Partner Center and Microsoft Edge changes.

This timeline is subject to change. This article will be updated to share exact details as the milestones draw nearer.

| Timeframe	| Microsoft Partner Center changes | Microsoft Edge changes |
|--- |--- |--- |
| June 2022	| Microsoft Partner Center will no longer accept new Manifest V2 extensions with visibility set as `Hidden` or `Public`. | No change. |
| January 2023 | Microsoft Partner Center will no longer accept updates to existing Manifest V2 extensions. Developers can submit updates for migrating a V2 extension to V3. | Microsoft Edge stops running Manifest V2 extensions. Enterprises can allow Manifest V2 extensions to run on Microsoft Edge using Enterprise policies. |
| June 2023 | No change. | Manifest V2 extensions will no longer function in Microsoft Edge even with the use of Enterprise policy. |

Microsoft continues to iteratively improve the platform and address the feedback shared by extension developers.

Share your questions, comments, and concerns with the team on Twitter [@MSEdgeDev](https://twitter.com/msedgedev/) or via the [Microsoft Edge Insider forums on TechCommunity](https://techcommunity.microsoft.com/t5/articles/manifest-v3-changes-are-now-available-in-microsoft-edge/m-p/1780254).
