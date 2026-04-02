# spanec
# 🌙 Sleep Program Data Logger v3.2

Sistem za spremljanje spanca in dnevnih navad strank v okviru 21-dnevnega programa.

## 🚀 Hitre povezave
- **Spletni dnevnik:** `https://<tvoj-uporabnik>.github.io/<ime-projekta>/`
- **Google Sheet Baza:** [Tukaj prilepi povezavo do svoje tabele]

## 🛠 Nastavitve za nove kliente
Za vsakega novega klienta generiraj unikatno povezavo, da mu ni treba vpisovati podatkov:
`https://<tvoj-uporabnik>.github.io/<ime-projekta>/?ime=Ime_Priimek&email=naslov@email.com`

## 📂 Struktura projekta
* **`index.html`**: Mobilno prilagojen vmesnik z avtomatskim izračunom povprečja (Stats Card).
* **`EmailParser.gs`**: Bere e-pošto in izlušči podatke (vključno z datumom in številko dneva).
* **`SheetWriter.gs`**: Piše v tabelo, preprečuje podvajanje vrstic in računa statistiko za "PREGLED VSEH".
* **`WebApi.gs`**: Omogoča vmesniku na GitHubu branje preteklih podatkov iz tabele.

## ⚠️ Pomembna navodila za vzdrževanje
1.  **Osveževanje podatkov:** Če želiš, da se vsi prejeti emaili takoj zapišejo v tabelo, mora biti nastavljen "Trigger" v Google Apps Scriptu na funkcijo `processInbox`.
2.  **Povprečja:** Tabela "PREGLED VSEH" se posodobi vsakič, ko se izvede zapis novega dneva za posameznega klienta.
3.  **Logotip:** Logo se vleče iz naslova: `https://info.hypno-transformations.com/wp-content/uploads/2024/01/logo-header.png`.

