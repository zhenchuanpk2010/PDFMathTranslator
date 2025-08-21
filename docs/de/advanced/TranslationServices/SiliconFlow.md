# SiliconFlow

## Kostenloser Übersetzungsdienst

[SiliconFlow](https://siliconflow.cn) bietet einen kostenlosen Übersetzungsdienst für dieses Projekt an.

Derzeit wird für den kostenlosen Übersetzungsdienst das Modell `THUDM/GLM-4-9B-0414` verwendet.

### Verwendung

#### Kommandozeile

```bash
pdf2zh_next --siliconflowfree example.pdf 
```

#### WebUI

1. Wählen Sie "SiliconFlowFree" aus der Dropdown-Liste "Übersetzungsoptionen" - "Dienst" aus.
2. Klicken Sie auf die Schaltfläche "Übersetzen" am unteren Rand der Seite, um mit der Übersetzung zu beginnen.
3. Nach Abschluss der Übersetzung finden Sie die übersetzte `PDF`-Datei im Abschnitt "Übersetzt" am unteren Rand der Seite.


### Datenschutzrichtlinie

Die Dateiinhalte werden an den Server des Projektbetreuers [@awwaawwa](https://github.com/awwaawwa) gesendet und dann an SiliconFlow zur Übersetzung weitergeleitet.

Die Betreuer dieses Projekts sammeln nur Fehlerinformationen, die von SiliconFlow zurückgegeben werden, um damit verbundene Dienste zu debuggen. Ihre Dateiinhalte werden nicht gesammelt.

SiliconFlow Datenschutzrichtlinie: [简体中文](https://docs.siliconflow.cn/cn/legals/privacy-policy)/[English](https://docs.siliconflow.cn/en/legals/privacy-policy)



## Andere Modelle von SiliconFlow verwenden

[SiliconFlow](https://siliconflow.cn) bietet auch andere Modelle für die Übersetzung an.

### Verwendung

1. Registrieren Sie ein Konto bei [SiliconFlow](https://siliconflow.cn)

2. Erstellen Sie einen API-Schlüssel unter [SiliconFlow API Key](https://cloud.siliconflow.cn/me/account/ak). Klicken Sie dann auf den Schlüssel, um ihn zu kopieren.

#### Kommandozeile

```bash
pdf2zh_next --siliconflow --siliconflow-model "Pro/deepseek-ai/DeepSeek-V3" --siliconflow-api-key <your-api-key> example.pdf
```

#### WebUI

1. "Übersetzungsoptionen" - **"Dienst"** Dropdown-Liste: Wählen Sie "SiliconFlow"  
2. "Übersetzungsoptionen" - **"Basis-URL für SiliconFlow API"**: Behalten Sie den Standardwert bei  
3. "Übersetzungsoptionen" - **"Zu verwendendes SiliconFlow-Modell"**: Geben Sie "Pro/deepseek-ai/DeepSeek-V3" oder andere Modelle ein  
4. "Übersetzungsoptionen" - **"API-Schlüssel für SiliconFlow-Dienst"**: Fügen Sie Ihren API-Schlüssel ein  
5. Klicken Sie auf die Schaltfläche "Übersetzen" am unteren Rand der Seite, um die Übersetzung zu starten  
6. Nach Abschluss der Übersetzung finden Sie die übersetzte `PDF`-Datei im Abschnitt "Übersetzt" am unteren Rand der Seite.


## Danksagung

Danke an [SiliconFlow](https://siliconflow.cn) für die Bereitstellung des kostenlosen Übersetzungsdienstes für dieses Projekt.

<div align="right"> 
<h6><small>Ein Teil des Inhalts dieser Seite wurde von GPT übersetzt und kann Fehler enthalten.</small></h6>