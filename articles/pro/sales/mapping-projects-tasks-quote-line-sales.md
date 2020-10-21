---
title: Esleitu proiektuak eta zereginak proiektuetan oinarritutako eskaintzaren lerro batean
description: Gai honek proiektuak eta zereginak proiektuetan oinarritutako ataza lerro batera mapatzeko moduari buruzko informazioa eskaintzen du.
author: rumant
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d726ab09da0e502da99191f7e7469c47f79b6e7c
ms.sourcegitcommit: 6b396ccf5e76230a42a2f933a3aaa5b8149790bb
ms.translationtype: HT
ms.contentlocale: eu-ES
ms.lasthandoff: 10/06/2020
ms.locfileid: "3964892"
---
# <a name="map-projects-and-tasks-to-a-project-based-quote-line"></a>Esleitu proiektuak eta zereginak proiektuetan oinarritutako eskaintzaren lerro batean

_**Honetarako aplikatzen da:** Baliabideen / stockean oinarritutako eszenatokietarako proiektuen eragiketak, Lite hedapena - proformaren fakturazioari aurre egitea_

Proiektuetan oinarritutako aurrekontu lerroetan, dagoeneko aurrekontu lerro batekin lotuta dagoen proiektu baten zeregin zehatzak mapatu ditzakezu.

Zereginak aurrekontu lerro batera mapatzen dituzunean, aurrekontu lerroan zehaztu dituzun elementu hauek zeregin horiei soilik aplikatuko zaizkie:

- Fakturazio-metodoa
- Kobragarritasun-aukerak
- Ez gainditzeko mugak
- Bezeroak

Adibidez, fase bat prezio finkoa duen eta beste fase guztiak denbora eta materialak diren proiektu bat izan dezakezu. Kasu honetan, lehen fasea eta haren seme-alaba guztiak, fase horretako aurrekontu lerroarekin lotu ditzakezu prezio finkoaren fakturazio metodoarekin. Ondoren, beste fase guztiak denboran eta materialetan oinarritutako aurrekontu lerroarekin lotu ditzakezu.

## <a name="associate-tasks-to-project-based-quote-lines"></a>Lotu zereginak proiektuan oinarritutako eskaintzaren lerroak

Atazak kokapen hauetako aurrekontu lerroekin lotu ditzakezu:

- **Proiektua** orrialdea > **Zereginen fakturazioa** fitxa (optimoa)
- **Aipatu lerroa** orrialdea > **Kobratzeko zereginak** fitxa 

### <a name="from-the-project-page"></a>Proiektua orritik

**Proiektua** orrialdeak zereginak lerroen artean lotzeko esperientzia ezin hobea eskaintzen du. Orrialde hau erabil dezakezu zeregin anitz hautatzeko eta haiek guztiak, haurren zereginak gehituta hautatutako aurrekontu lerroarekin lotzeko.

1. **Orokorra** proiektuan oinarritutako aurrekontu lerroaren fitxan, egiaztatu **Proiektua** eremua bete da.
2. **Zereginak barne** eremuan, hautatu **Aukeratutako zereginak soilik**.
3. Gorde proiektuetan oinarritutako eskaintzaren lerroa. Inprimakia freskatzean, **Kobratzeko zereginak** fitxa pantailetan.
4. **Orokorra** fitxan, hautatu proiektuaren esteka **Proiektua** eremutik.
5. **Proiektua** orrialdean, hautatu **Zereginaren fakturazioa** fitxan.
6. Bigarren saretan, zeregin zehatzen fakturazio konfigurazioari aplikatzen zaiona, hautatu zeregin bat edo gehiago eta, ondoren, hautatu **Elkartu aurrekontu lerroak**.
7. Agertzen den elkarrizketa-orrian, hautatu aurrekontuan proiektuan oinarritutako aurrekontu lerroak bistaratuko dituen aurrekontu lerroa.
8. **Fakturazio mota** eremuan, adierazi zeregin horiek kargagarriak edo kargagarriak ez diren.
9. Hautatu kontrol laukia elkarteak hautatutako zereginen seme-alaben zereginak sartu behar dituen ala ez adierazteko. Laukia markatuta hautatutako atazetako haurren zereginak aurrekontu lerroarekin lotuko dira.
10. Hautatu **Ados** elkarrizketa ixteko.

### <a name="from-the-quote-line-page"></a>Aipatu lerroaren orrian

Proiektuaren zereginak lotu ditzakezu **Kobratzeko zereginak** fitxa **Aipatu lerroa** orrialdea.

>[!NOTE]
>Proiektuaren zereginak lerroak aipatzeko lotzeko lekurik onena da **Zereginen fakturazioa** fitxan **Proiektua** orrialdea. Zereginak lotzen badituzu **Kobratzeko zereginak** fitxatik **Aipatu lerroa** orrialdean, proiektu bakoitza eskuz lotu behar duzu.

1. **Orokorra** proiektuan oinarritutako aurrekontu lerroaren fitxan, egiaztatu proiektu bat hautatuta dagoela **Proiektua** eremuan.
2. **Zereginak barne** eremuan, hautatu **Aukeratutako zereginak soilik**.
3. Gorde proiektuetan oinarritutako eskaintzaren lerroa. Inprimakia freskatzean, **Kobratzeko zereginak** fitxa pantailetan.
4. **Kobratzeko zereginak** fitxan, hautatu **Gehitu aurrekontu lerroaren zeregina**.
5. **Aipatu lerro zeregina** orrialdean, **Zereginak** eremuan, hautatu zeregina eta **Fakturazio mota** eremua, hautatu **Gorde**. 
6. Itxi orria. Aukeratutako zeregina aurrekontu lerroarekin lotuta dago orain.

## <a name="disassociate-tasks-from-projectbased-quote-lines"></a>Askatu zereginak proiektuan oinarritutako eskaintzaren lerroetatik

### <a name="from-the-project-page"></a>Proiektua orritik

Metodoak orrialdeak zereginak lerroen artetik askatzeko esperientzia ezin hobea eskaintzen du. Zeregin anitz hautatzeko eta haiek guztiak, haurren zereginak gehituta hautatutako aurrekontu lerrotik askatzeko.

1. **Orokorra** proiektuan oinarritutako aurrekontu lerroaren fitxan,**Proiektua** eremuan, hautatu proiektuaren esteka.
2. **Proiektua** orrialdean, hautatu **Zereginaren fakturazioa** fitxan.
3. Bigarren saretan, zeregin zehatzen fakturazio konfigurazioari aplikatzen zaiona, hautatu zeregin bat edo gehiago eta, ondoren, hautatu **Askatu aurrekontu lerroak**.
4. Agertzen den elkarrizketa-orrian, hautatu aurrekontu lerroa.
5. Hautatu kontrol laukia elkarteak hautatutako zereginen seme-alaben zereginak ere kendu behar diren ala ez adierazteko. Laukia markatuta hautatutako atazetako haurren zereginak aurrekontu lerrotik askatuko dira.
6. Hautatu **Ados**. Abisu mezu batek jakinarazten dizu elkarte hau kentzen baduzu, zereginean aurretik grabatutako datuak alderantzika litezkeela. 
7. Aukeratu **Ados** zereginaren eta proiektuan oinarritutako aurrekontu lerroaren arteko lotura jarraitzeko eta kentzeko.

### <a name="from-the-quote-line-page"></a>Aipatu lerroaren orrian

Proiektuaren zereginak ere aska ditzakezu **Kobratzeko zereginak** fitxa **Aipatu lerroa** orrialdea.

1. **Kobratzeko zereginak** fitxan, hautatu **Ezabatu aurrekontu lerroaren zeregina**.
2. Hautatu **Ados**. Abisu mezu batek jakinarazten dizu elkarte hau kentzen baduzu, zereginean aurretik grabatutako datuak alderantzika litezkeela. 
3. Aukeratu **Ados** zereginaren eta proiektuan oinarritutako aurrekontu lerroaren arteko lotura jarraitzeko eta kentzeko.

>[!NOTE]
> Prozedura honek ez du zeregina proiektutik ezabatzen. Zereginen elkartea proiektuan oinarritutako aurrekontu lerroatik bakarrik kentzen du.
