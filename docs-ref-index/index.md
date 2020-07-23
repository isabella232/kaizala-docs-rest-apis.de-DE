---
title: Kaizala-Rest-API | MicrosoftDocs
description: Dieses Thema enthält Rest-API-Referenzinhalte für die Kaizala-API.
ms.date: 05-10-2017
ms.service: kaizala
ms.topic: conceptual
author: ''
ms.author: ''
manager: ''
ms.devlang: https
ms.openlocfilehash: 732aae562aaf823798066952a40526e353072efc
ms.sourcegitcommit: d95e42eaf596f2fd27330bd4bfd6525f356a9f2e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384230"
---
# <a name="kaizala-rest-api"></a>Kaizala-Rest-API

Mit Kaizala können Drittanbieterentwickler Kaizala in Ihre Geschäftsprozesse integrieren, indem Sie die Möglichkeit zum Ausführen einer kuratierten Reihe von Aktionen in Kaizala mithilfe von Rest-basierten API-aufrufen bieten. Der Bereich der API besteht darin, dass externe Systeme den End-Punkt aufrufen und Aktionen bei Bedarf ausführen. Das bedeutet, dass es sich hierbei um ein Pull-Modell handelt, in dem einzelne Endpunkte aufgerufen werden müssen, um bestimmte Aktionen mit Kaizala-APIs auszuführen. Das Push-Modell, auf dem die Kaizala-Plattform Aktionen auslösen kann, kann mit webhooks konfiguriert werden.

## <a name="rest-operations"></a>Rest-Vorgänge

| Vorgang | Beschreibung                                                        |
|-----------------|--------------------------------------------------------------------|
| PIN generieren | Generiert eine einmalige PIN für eine Mobiltelefonnummer, wenn die Application/Connector-ID bereitgestellt wird. |
| Aktualisierungs Token abrufen | Generiert ein Aktualisierungstoken für die angegebene Anwendung/Connector-ID, wenn Pin, Mobiltelefonnummer & Application/Connector-ID bereitgestellt wird. |
| Zugriffs Token generieren | Generiert Zugriffstoken für den Zugriff auf Kaizala-Ressourcen, wenn Update Token, Application/Connector-ID und Application/Connector Secret bereitgestellt wird |
| Gruppe erstellen | Ermöglicht die Erstellung einer a-Gruppe, einschließlich verwalteter öffentlicher Gruppen. Es wird ein Array von Zeichenfolgen als Eingabe benötigt. Jede Zeichenfolge ist eine Mobiltelefonnummer (mit Landesvorwahl). Diese API kann maximal 100 Mobiltelefonnummern als Eingabe annehmen. \ n \ tGroupType: Group/connectgroup. Connectgroup für die verwaltete öffentliche Gruppe. |
| Untergruppe erstellen | Erstellen einer Untergruppe  |
| Mitglieder hinzufügen | Hinzufügen von Mitgliedern zu einer Gruppe |
| Untergruppe hinzufügen | Hinzufügen einer Gruppe als Untergruppe zu einer anderen Gruppe |
| Abonnenten hinzufügen | Hinzufügen von Teilnehmern zu einer öffentlichen Gruppe |
| Fetch Group Details | Abrufen von Details für eine Gruppe |
| FETCH-Member | Gibt eine Liste der Mitglieder in einer Gruppe zurück. |
| Abonnenten abrufen | Ruft eine Liste der Abonnenten einer verwalteten öffentlichen Gruppe ab. |
| Untergruppe abrufen | Abrufen von Untergruppen einer Gruppe |
| Gruppe als Untergruppe entfernen | Gruppe als Untergruppe zu einer anderen Gruppe entfernen |
| Mitglieder entfernen | Entfernt Mitglieder aus einer Gruppe. |
| Abonnenten entfernen | Entfernen von Teilnehmern aus einer verwalteten öffentlichen Gruppe |
| Direkte Gruppen abrufen | Gibt alle mit dem Benutzer verknüpften direkten Gruppen zurück. |
| Nachricht senden | Senden einer Nachricht an eine Gruppe |
| Senden einer Nachricht an einen Abonnenten | Senden von Nachrichten an Teilnehmer in einer öffentlichen Gruppe |
| Hochladen von Medien | Uploads von Medien (Bild, Dokument, Audio, Album oder Video) |
| Umfrage senden | Ermöglicht das Erstellen einer Umfrage und das Senden einer Gruppe |
| Bereitstelleneiner benutzerdefinierten Aktion auf einem Abonnenten | Bereitstelleneiner benutzerdefinierten Aktion an Abonnenten in einer öffentlichen Gruppe |
| Post-Antwort auf eine Aktion | Bereitstelleneiner Antwort auf eine Aktion |
| Bereitstellen der Antwort auf eine Umfrage | Bereitstelleneiner Antwort auf eine Umfrage |
| Aufträge abrufen | Abrufen von Aufträgen in einer Gruppe |
| Abrufen von Umfrage Antworten | Abrufen von Antworten für eine Umfrage |
| Abrufen aller webhooks | Gibt alle webhooks für eine Gruppe zurück. |
| Abonnieren aller Ereignisse | Abonnieren aller Ereignisse auf Aktionsebene |
| Kündigen eines webhooks | Kündigen eines webhooks |
