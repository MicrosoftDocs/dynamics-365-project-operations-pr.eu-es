---
title: Konfiguratu proiektu-kategoriak
description: Gai honek proiektuaren kategoriak konfiguratzeari buruzko informazioa ematen du.
author: sigitac
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d82302f12ba75a92f2de0e9746ad7e61ce0cdc6b
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995156"
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

Dynamics 365-ek Shared categories kontzeptua erabiltzen du gastuak aplikazio desberdinetan sailkatzeko, adibidez Dynamics 365 Finance, Dynamics 365 hornikuntza-katea eta Dynamics 365 Project Operations. Sortutako Transakzio-kategoria bakoitzerako, Project Operations-ek erlazionatutako lau kategoria partekatu sortzen dituzte automatikoki: Orduak, Gastuak, Tasak eta Elementua. Partekatutako kategoriak berrikusi eta doitu ditzakezu hona joan **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Kategoriak** \> **Kategoria partekatuak** aukerara.

## <a name="project-categories"></a>Proiektu-kategoriak

Proiektuen kategoriek kategoriaren konfigurazio maila zehatzena adierazten dute eta proiektuaren kontulari batek bereizita eta enpresa bakoitzerako konfiguratu behar ditu.

1. Joan **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Kategoriak** \> **Proiektuen kategoriak** aukerara.
2. Hautatu **Berria**.
3. Aukeratu **Kategoria IDa** aurreko atalean sortutako Partekatutako kategoriakoa. Project Operation-en eragiketei esker, transakzio kategoriarekin lotura duten kategoria partekatuak soilik erabil daitezke.
4. Hautatu kategoria taldea.

## <a name="category-groups"></a>Kategoria-taldeak

Kategoria-taldeak propietateak partekatzeko erabiltzen dira, batez ere profilak argitaratzeko, erlazionatutako proiektu kategorien artean. Transakzio mota bakoitzerako gutxienez kategoria talde bat egon behar da eta proiektu kategoria bakoitzari talde bat esleitzen zaio.

Project Operations-en argitaratzeko zehaztapenak proiektuaren kostu eta diru-sarreren profileko arauek, proiektuen kategoriek eta kategoria taldeek definitzen dituzte. Kategoria taldeak konfigura ditzakezu hona joan **Proiektuen kudeaketa eta kontabilitatea** \> **Konfigurazioa** \> **Kategoriak** \> **Kategoria taldeak**.


[!INCLUDE[footer-include](../includes/footer-banner.md)]