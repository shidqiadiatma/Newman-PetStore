# Newman-PetStore

---

## **Install Newman**

Pastikan Node.js sudah terpasang:

```bash
node -v
npm -v
```

Install Newman dan reporter HTML Extra:

```bash
npm install -g newman newman-reporter-htmlextra
```

---

## **Menjalankan Collection**

Gunakan NPX untuk menjalankan collection tanpa instalasi lokal:

```bash
npx newman run petstore.postman_collection -e petstore.postman_environment -r htmlextra -n 5
```

---

## **Penjelasan Perintah**

* **npx newman run**: menjalankan Newman melalui NPX.
* **petstore.postman_collection**: file collection yang dieksekusi.
* **-e petstore.postman_environment**: environment berisi variable (mis. baseUrl).
* **-r htmlextra**: generate HTML report yang lebih lengkap.
* **-n 5**: menjalankan collection sebanyak 5 iterasi.

---
