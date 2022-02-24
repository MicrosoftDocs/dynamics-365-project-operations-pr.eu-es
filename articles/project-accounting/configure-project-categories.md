---
title: Konfiguratu proiektu-kategoriak
description: Gai honek proiektuaren kategoriak konfiguratzeari buruzko informazioa ematen du.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 3698b68b5dd0460343d26af0fcea5b9a56be4083
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "4131913"
---
# <a name="configure-project-categories"></a>Konfiguratu proiektu-kategoriak

_**Honi aplikatzen zaio:** Baliabideetan/Izakinik gabeko produktuetan oinarritutako adibideen Project Operations_

Project Operations-ek gaitasun sendoak eskaintzen dituzte proiektuetako diru-sarrerak eta gastuak sailkatzeko. Kategoriek proiektuen transakzioen berri emateko eta aztertzeko gaitasuna eskaintzen dute eta liburuak liburu nagusira eramaten dituzte.

Ondorengo diagramak transakzio kategorien, partekatutako kategorien eta proiektuen kategorien arteko korrelazioa erakusten du. 

Transakzio kategoriak proiektuen transakzioen oinarrizko taldekatzea dira. Taldekatze horren barruan, aplikazio eta moduluen artean parteka daitezkeen kategoria partekatuen multzoa dago. Zehaztasunetan are gehiago sakonduz, proiektuen kategoriak kategorien maila zehatzenak dira. Proiektuen kategoriak pertsona juridikoei, moduluei eta aplikazioei dagozkie.

![Transakzio-kategorien, kategoria partekatuen eta proiektu-kategorien arteko korrelazioa](media/project-categories.png)

## <a name="transaction-categories"></a>Transakzio-kategoriak

Transakzio kategoriek proiektuen transakzioen oinarrizko taldekatzea adierazten dute eta ez dira konpainia edo transakzio motak. Adibidez, Contoso Robotics-ek Diseinua, Bidaia, Instalazioa eta Zerbitzuen Transakzio kategoriak erabiltzen ditu Proiektuaren transakzioak taldekatzeko.

Transakzio kategoriak Project Operations moduluan definitzen dira. 
1. Joan **Ezarpenak** \> **Transakzio-kategoriak** aukerara, inprimakia irekitzeko. 
2. Sortu transakzioen kategoria berria hautatuta **Berria** edo hautatuz **Inportatu Excel-etik**.

## <a name="shared-categories"></a>Partekatutako kategoriak

Dynamics 365-ek Partekatutako kategoriak kontzeptua erabiltzen du gastuak aplikazio desberdinetan sailkatzeko, adibidez Dynamics 365 Finance, Dynamics 365 Supply Chain eta Dynamics 365 Project Operations. Sortutako Transakzio-kategoria bakoitzerako, Project Operations-ek erlazionatutako lau kategoria partekatu sortzen dituzte automatikoki: Orduak, Gastuak, Tasak eta Elementua. Partekatutako kategoriak berrikusi eta doitu ditzakezu hona joan **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Kategoriak** \> **Kategoria partekatuak** aukerara.

## <a name="project-categories"></a>Proiektu-kategoriak

Proiektuen kategoriek kategoriaren konfigurazio maila zehatzena adierazten dute eta proiektuaren kontulari batek bereizita eta enpresa bakoitzerako konfiguratu behar ditu.

1. Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Kategoriak** \> **Proiektuen kategoriak** aukerara.
2. Hautatu **Berria**.
3. Aukeratu **Kategoria IDa** aurreko atalean sortutako Partekatutako kategoriakoa. Project Operation-en eragiketei esker, transakzio kategoriarekin lotura duten kategoria partekatuak soilik erabil daitezke.
4. Hautatu kategoria taldea.

## <a name="category-groups"></a>Kategoria-taldeak

Kategoria-taldeak propietateak partekatzeko erabiltzen dira, batez ere profilak argitaratzeko, erlazionatutako proiektu kategorien artean. Transakzio mota bakoitzerako gutxienez kategoria talde bat egon behar da eta proiektu kategoria bakoitzari talde bat esleitzen zaio.

Project Operations-en argitaratzeko zehaztapenak proiektuaren kostu eta diru-sarreren profileko arauek, proiektuen kategoriek eta kategoria taldeek definitzen dituzte. Kategoria taldeak konfigura ditzakezu hona joan **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Kategoriak** \> **Kategoria taldeak**.
