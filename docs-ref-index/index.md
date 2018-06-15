---
title: Kaizala REST-API | MicrosoftDocs
description: Dieses Thema enthält Inhalte für REST-API-Referenz für die Kaizala-API.
ms.date: 05-10-2017
ms.service: kaizala
ms.topic: conceptual
author: ''
ms.author: ''
manager: ''
ms.devlang: https
ms.openlocfilehash: 732aae562aaf823798066952a40526e353072efc
ms.sourcegitcommit: a9df86259a9029a137346752ff43e135e2db6d14
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/15/2018
ms.locfileid: "19907312"
---
# <a name="kaizala-rest-api"></a>Kaizala REST-API

Kaizala kann 3. Partei Entwickler integrieren Kaizala in ihre Geschäftsprozesse durch bereitstellen, dass die Möglichkeit zum Ausführen einer curated Reihe von Aktionen in Kaizala mithilfe von REST-API-Aufrufe basiert. Der Bereich der API ist für externe Systeme zum Aufrufen des Endpunkt und Ausführen von Aktionen auf Abruf. D. h., wird dies eine PULL-Modell – sein, in denen einzelne Endpunkte aufgerufen werden, um bestimmte Aktionen Kaizala APIs ausführen müssen. Das PUSH-Modell, in dem Kaizala Plattform Aktionen auslösen kann, kann mithilfe von Webhooks konfiguriert werden.

## <a name="rest-operations"></a>REST-Vorgänge

| Vorgang | Beschreibung                                                        |
|-----------------|--------------------------------------------------------------------|
| Generieren der Pin | Einmaliges PIN für eine Mobiltelefonnummer generiert, wenn Application/Connector-Id angegeben wird |
| Refresh Token abrufen | Aktualisierungstoken für die angegebene Anwendung/Connector-Id generiert, wenn Pin, Mobiltelefonnummer & Id Application/Connector wird bereitgestellt. |
| Generieren Sie Zugriffstoken | Generiert Zugriffstoken, um Kaizala-Ressourcen zugreifen, wenn Aktualisierungstoken, Application/Connector-Id und geheimen Schlüssel Application/Connector bereitgestellt wird |
| Gruppe erstellen | Ermöglicht die Erstellung einer einer Gruppe, einschließlich der öffentlichen Gruppen verwaltet. Array von Zeichenfolgen verwendet als Eingabe. Jede Zeichenfolge ist Mobiltelefonnummer (mit Ländercode). Diese API kann als input.\n\tGroupType maximal 100 Mobiltelefonnummern akzeptieren: Gruppe/ConnectGroup. ConnectGroup für Öffentliche Gruppe verwaltet. |
| Untergruppe erstellen | Erstellen Sie eine Sub-Gruppe  |
| Hinzufügen von Mitgliedern | Hinzufügen von Mitgliedern zu einer Gruppe |
| Hinzufügen einer Untergruppe | Gruppe in eine andere Gruppe als eine Untergruppe hinzufügen |
| Hinzufügen von Abonnenten | Hinzufügen von Abonnenten an eine öffentliche Gruppe |
| Details der Fetch | Abrufen von Informationen für eine Gruppe |
| Abrufen der Member | Gibt die Liste der Elemente in einer Gruppe |
| FETCH-Abonnenten | Ruft die Liste der Teilnehmer über eine verwaltete öffentliche Gruppe |
| FETCH Untergruppe | Abrufen von Untergruppen einer Gruppe |
| Gruppe als Untergruppe entfernen | Entfernen Sie die Gruppe als eine Untergruppe in eine andere Gruppe |
| Entfernen von Mitgliedern | Entfernt Mitglieder aus einer Gruppe |
| Entfernen von Abonnenten | Entfernen von Abonnenten aus einer verwalteten öffentliche Gruppe |
| Direkte FETCH-Gruppen | Gibt alle direkte Gruppen mit dem Benutzer zugeordnet ist |
| Nachricht senden | Senden Sie eine Nachricht für eine Gruppe |
| Senden der Nachricht an einen Abonnenten | Senden Sie Nachricht an Abonnenten in einer öffentlichen Gruppe |
| Medien hochladen | Uploads Medien (Bild, Dokument, Audio, Album oder Video) |
| Umfrage senden | Erstellen einer Umfrage, und für eine Gruppe senden können |
| Erstellen von benutzerdefinierten Aktion für ein-Abonnent | Erstellen von benutzerdefinierten Aktion für Abonnenten in einer öffentlichen Gruppe |
| POST-Antwort auf eine Aktivität | Stellen Sie eine Antwort auf eine Aktion |
| POST-Antwort auf eine Umfrage | Stellen Sie eine Antwort auf eine Umfrage |
| Abrufen von Aufträgen | Abrufen von Aufträgen in einer Gruppe |
| FETCH Umfrageantworten | Abrufen von Antworten für eine Umfrage |
| Abrufen Sie aller Webhooks | Gibt alle Webhooks für eine Gruppe |
| Alle Ereignisse abonniert | Abonnieren Sie alle Ereignisse auf Aktionsebene |
| Melden Sie sich ab einem Webhook | Ein Webhook aufheben |
