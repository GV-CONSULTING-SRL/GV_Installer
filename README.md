# GV IntegratorSystem - Installer

Repo pubblica per la distribuzione di GV IntegratorSystem (framework + moduli C#).

## Download

Scarica l'ultima versione dalla sezione [Releases](https://github.com/GV-CONSULTING-SRL/GV_Installer/releases/latest).

Nessun account GitHub richiesto — la repo e' pubblica.

## Asset disponibili nella release

| Asset | Contenuto |
|-------|-----------|
| `Setup_GV_IntegratorSystem_v*.exe` | Installer wizard completo (~220 MB) |
| `framework-v*-win-x64.zip` | Backend Node.js + frontend React pre-compilato |
| `{module_id}-v*-win-x64.zip` | Exe modulo C# pre-compilato (.NET 8) |
| `catalog.json` | Catalogo moduli (source of truth) |

## Moduli disponibili

| ID | Porta | Descrizione |
|----|-------|-------------|
| gv_integrator_acq | 5200 | Acquisti: RDA, ordini, lamiere |
| importcad3d | 5201 | Import distinte Excel/CAD |
| salvagnini_ops | 5202 | XML Salvagnini - OPS |
| speedcost | 5203 | Preventivazione carpenteria |
| officeautomation | 5204 | Processi documentali |
| connettorevision | 5205 | MOV_CON - Vision API |
| costupdater | 5206 | Aggiornamento costi cascade |
| gv_insighthub | 5207 | Cruscotto analitico BI |
| packinglistds | 5208 | Packing list spedizioni |

## Requisiti di sistema

- Windows 10/11 o Windows Server 2019+ (64-bit)
- SQL Server 2017+
- 4 GB RAM minimo
- 500 MB spazio disco (+ spazio per dati)
- Connessione Internet (per modalita "Download da Internet")

## Modalita di installazione

1. **Download da Internet** (consigliato) — l'installer scarica automaticamente i componenti necessari da questa repo. Nessun token o SDK richiesto.
2. **File locali** — per installazioni offline, fornire una cartella o ZIP con i file pre-compilati.

## Aggiornamento

- **Framework**: eseguire `aggiorna.ps1` (scarica automaticamente da questa repo)
- **Moduli**: eseguire `aggiorna-moduli.ps1 -UseRelease -ModuliIds "id1,id2"`
- **Console web**: Tab "Aggiornamenti" in `/sistema/console` (System Admin)

## Supporto

Per assistenza contattare GV Consulting srl.
