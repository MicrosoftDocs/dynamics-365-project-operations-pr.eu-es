---
title: Metodoak osatzeko kostua
description: Gai honek proiektu bat osatzeko kostua kalkulatzeko erabilitako metodoei buruzko informazioa eskaintzen du.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 790b5c98182acdc0a37e3741a40baf7152f0bf66
ms.sourcegitcommit: 2d399bc9d07807626f0d6b2d0cf304240c47591c
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 11/17/2020
ms.locfileid: "4531346"
---
# <a name="cost-to-complete-methods"></a>Metodoak osatzeko kostua

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Gai honek proiektu bat osatzeko kostua kalkulatzeko erabilitako metodoei buruzko informazioa eskaintzen du. Proiektu bat osatzeko kostua kalkulatzeko erabil ditzakezun hainbat metodo daude. 

Proiektu baten aurrekontua sortzen duzunean, **Sortu aurrekontua** orrialdean, **Metodoa osatzeko kostua** eremuan, metodo hau osatzeko kostu hauetako bat hauta dezakezu.

| Metodoa osatzeko kostua    | Deskribapena                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Guztizko kostua - unekoa            | Sartu aurrekontuaren kostuak eskuz **Guztizko kostua** edo **Kopuru osoa** eremuak **Kostuen aurrekontua** botoian **Estimazio orria**. Sistemak sartutako guztizkoei benetako kostuak kentzen dizkie. Guztira proiektua osatzeko kostua da. Metodo honek ez ditu barne eraikitako proiektuen eragiketetan sartutako gastuen kalkuluak eta baliabideen esleipenak erabiltzen Microsoft Dataverse. Guztizko kostua edo guztizko kantitatea eskuz egunera daitezke beharren arabera.  |
| Aurreikuspena-benetakoa, guztira        | Baliabideen esleipena eta gastuen kalkuluak proiektuaren aurreikuspenaren zenbateko osoa zehazteko erabiltzen dira. Benetako kostuak aurreikuspen honekin alderatzen dira, osatutako kostua kalkulatzeko.                                                                                                                                                                                                                                                                          |
| Aurreko kalkuluen arabera         | Aurreko aldian erabili ziren estimazio metodo berak erabiltzen dira hemen. Metodo honek iragarpen eredua behar du, aurreko aldian iragarpen eredua behar bada.                                                                                                                                                                                                                                                                                                                           |
| Ezarri kostua zero izatera | Normalean aurrekontuaren proiektua ezabatu aurretik erabiltzen da, metodo honek zenbateko osoak bat egiten du argitaratutako benetako transakzioekin eta garbitu egiten du **Osatzeko kostua** zutabea. Osatutakoan, emaitza ehuneko 100 da beti. Sortzen duzun kostu lerro bakoitzerako **Iragarpena** kontrol laukia garbitu eta guztizko zenbatekoa aurreko kostuaren aurrekontutik kopiatuko da. Aurreikusitako epearen benetako kontsumoa proiektua osatzeko kostutik kentzen da.              |
| Kostuen txantiloitik           | Aukeratutako aurrekontu proiektuarekin lotutako kostuen txantiloian konfiguratutako metodoa osatzeko kostua.                                                                                                                                                                                                                                                                                                                                                                          |