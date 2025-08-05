Einige Fragen werden häufig gestellt, daher haben wir eine Liste für Benutzer bereitgestellt, die ähnliche Probleme haben.

## Wird eine GPU benötigt?
- **Frage**:
## Wird eine GPU benötigt?

- **Antwort**:
**Eine GPU ist nicht erforderlich.** Aber wenn Sie eine GPU haben, wird das Programm diese automatisch für eine höhere Leistung nutzen.

## Download unterbrochen?
- **Frage**:
Ich bin beim Herunterladen des Modells auf den folgenden Unterbrechungsfehler gestoßen. Was soll ich tun?

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **Antwort**:
Das Netzwerk erfährt Störungen, bitte verwenden Sie eine stabile Netzwerkverbindung oder versuchen Sie, die Netzwerkintervention zu umgehen.

## Wie aktualisiert man auf die neueste Version?
- **Frage**:
Ich möchte einige der Funktionen der neuesten Version nutzen, wie aktualisiere ich sie?

- **Antwort**:
`pip install -U pdf2zh`


## Die folgenden Dateien existieren nicht: example.pdf
- **Problem**:
Beim Ausführen des Programms erhalten Benutzer die folgende Ausgabe: `The following files do not exist: example.pdf`, wenn das Dokument nicht gefunden wurde.

- **Lösung**:
  - Öffnen Sie die Kommandozeile in dem Verzeichnis, in dem sich die Datei befindet, oder
  - Geben Sie den vollständigen Pfad der Datei direkt nach pdf2zh ein, oder
  - Verwenden Sie den interaktiven Modus `pdf2zh -i`, um Dateien direkt per Drag & Drop einzufügen


## SSL-Fehler und andere Netzwerkprobleme

Wenn Sie beim Herunterladen von Modellen oder beim Ausführen von pdf2zh auf SSL-Fehler stoßen, liegt dies wahrscheinlich an Netzwerkproblemen. Hier sind einige Lösungsansätze:

1. **Überprüfen Sie Ihre Internetverbindung**  
   Stellen Sie sicher, dass Ihr Gerät mit dem Internet verbunden ist und eine stabile Verbindung hat.

2. **Proxy-Einstellungen**  
   Wenn Sie einen Proxy verwenden, stellen Sie sicher, dass dieser korrekt konfiguriert ist. Sie können auch versuchen, den Proxy vorübergehend zu deaktivieren, um zu sehen, ob das Problem dadurch behoben wird.

3. **SSL-Zertifikate**  
   Einige Netzwerke blockieren oder verändern SSL-Zertifikate. Sie können versuchen, die SSL-Überprüfung zu deaktivieren (nicht empfohlen für Produktionsumgebungen):

   ```bash
   export PYTHONHTTPSVERIFY=0
   ```

4. **Alternative Download-Quellen**  
   Wenn das Problem beim Herunterladen von Modellen auftritt, können Sie versuchen, die Modelle manuell von einer alternativen Quelle herunterzuladen und sie dann in den entsprechenden Ordner zu verschieben.

5. **Firewall und Antivirensoftware**  
   Überprüfen Sie, ob Ihre Firewall oder Antivirensoftware die Verbindung blockiert. Fügen Sie pdf2zh zur Whitelist hinzu oder deaktivieren Sie die Software vorübergehend.

6. **DNS-Einstellungen**  
   Manchmal können Probleme mit dem DNS-Server zu Verbindungsproblemen führen. Versuchen Sie, Ihren DNS-Server zu ändern (z.B. zu Google DNS: `8.8.8.8` oder `8.8.4.4`).

Wenn das Problem weiterhin besteht, können Sie sich an die [Community](#community) wenden oder die [FAQ](#faq) konsultieren.
- **Problem**:
Beim Herunterladen von Hugging Face-Modellen können Benutzer in China Netzwerkfehler erhalten. Zum Beispiel in [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55), [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70).

- **Lösung**:
  - [GFW umgehen](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Hugging Face Mirror verwenden](https://hf-mirror.com/).
  - [Portable Version verwenden](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [Docker stattdessen verwenden](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [Zertifikate aktualisieren](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), wie in [Issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55) vorgeschlagen.

## Localhost ist nicht erreichbar
Bitte siehe unten.

## Fehler beim Starten der GUI mit 0.0.0.0
- **Problem**:
Die Verwendung von Proxy-Software im globalen Modus kann verhindern, dass Gradio ordnungsgemäß startet. Zum Beispiel in [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77).

- **Lösung**:
Verwenden Sie den Regelmodus

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>Ein Teil des Inhalts dieser Seite wurde von GPT übersetzt und kann Fehler enthalten.</small></h6>