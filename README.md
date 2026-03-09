# PasteShare 🚀

A **PasteShare** egy ultra-minimalista, nyílt forráskódú, kliensoldali titkosítással működő szövegmegosztó alkalmazás. A projekt célja, hogy a privát jegyzetek megosztása során az adat soha ne érintse a szervert olvasható formában.

## 🌟 Főbb jellemzők

- **Zéró Backend:** Nincs szükség adatbázisra vagy szerveroldali nyelvre (PHP, Node.js, stb.).
- **Kliensoldali Titkosítás:** Az adatok tömörítése és kódolása az `LZ-String` algoritmus segítségével a böngésződben történik.
- **URL-alapú Tárolás:** Minden adat a böngésző címsorában (hash) tárolódik. Ha nincs meg a link, az adat sem létezik.
- **Önvédelmi Funkció:** Beépített integritás-ellenőrzés, amely megakadályozza a branding eltávolítását.

## 🛠️ Telepítés és használat

A PasteShare egyik legnagyobb előnye a **"Plug and Play"** működés.

1. **Klónozd a tárolót:**
   git clone https://github.com/Olcsa123Dev/PasteShare.git

2. **Testreszabás:**
   Nyisd meg az index.html fájlt és írd át a címet a sajátodra:
   <title>Saját PasteShare Editor</title>

3. **Publikálás:**
   Töltsd fel bármilyen statikus tárhelyre (GitHub Pages, Netlify, Vercel vagy saját szerver).

## 🔒 Technikai működés

Az alkalmazás az LZString metódust használja. Mentéskor a rendszer összefűzi a hitelesítő szöveget a tartalommal, majd kódolja azt. Visszatöltéskor a script ellenőrzi az hitelesítő szöveg meglétét; ha a kódolt adat sérült vagy módosított, a tartalom nem kerül megjelenítésre.

## 📄 Licenc

Ez a projekt nyílt forráskódú. Felhasználható és módosítható, feltéve, hogy a "Powered by PasteShare" branding megjelölés látható marad a kliensoldali script előírásai szerint.

---
**Fejlesztette:** [Olcsa123Dev](https://github.com/Olcsa123Dev)
