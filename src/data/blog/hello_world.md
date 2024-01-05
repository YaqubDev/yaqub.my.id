---
banner_alt: A photo of a forest overlooking the bright white sky in the background
banner: https://images.unsplash.com/photo-1494825514961-674db1ac2700?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8
title_prefix: Introducing
title: 👋🏻 Hello World
description: Situs di buat oleh Farizal M. Yaqub , Class 8D
date: '2023-14-24'
---

## :face_with_raised_eyebrow: What is this?

---

Ini adalah Situs Web baru saya! Dibangun dari awal dengan tumpukan teknologi baru yang saya pilih berdasarkan apa yang belum saya pelajari & gunakan selama beberapa bulan/tahun terakhir.

Jadi, dengan banyaknya pekerjaan yang dilakukan untuk membangun kembali situs web saya saat ini tetapi dengan tampilan yang benar-benar baru & sejumlah fitur & opsi baru, saya pikir sekarang ini akan menjadi perubahan yang baik untuk memamerkan beberapa di antaranya

## :question: Why

---

Portofolio adalah kumpulan karya atau hasil kerja yang pernah kamu buat. Portofolio karya dapat memberikan gambaran tentang kemampuan dan keahlian yang dimiliki oleh seseorang. Oleh karena itu, Portofolio dapat meningkatkan peluang karir setiap orang yang sedang bekerja maupun yang masih mencari pekerjaan.

## :hammer: Tech Stack

---

Pembelajaraan project](https://github.com/yaqubvocalid) pribadi saya & portofolio:

-   :atom_symbol: [React](https://reactjs.org/) / [Preact](https://preactjs.com/) (For Production)
-   :muscle: [Next.js](https://nextjs.org/)
    -   :mag: [next-seo](https://github.com/garmeeh/next-seo)
    -   :crescent_moon: [next-themes](https://github.com/pacocoursey/next-themes)
-   :female-singer: [EmotionCSS](https://emotion.sh)
-   :lipstick: [Twin.macro](https://github.com/ben-rogerson/twin.macro) (For [Tailwind CSS](https://tailwindcss.com/))
-   :tokyo_tower: [Tailwind UI](https://tailwindui.com/)
-   :feather: [Feather Icons](https://feathericons.com/)
-   :file_cabinet: [Hookstate](https://hookstate.js.org/)
-   :+1: [react-use](https://github.com/streamich/react-use)

## :pinching_hand: Vite

---

Tidak ada (404)

## :sparkles: Features

 UI UX / Tailwind / NextJS

---

With this new ground up re-build comes a whole host of new features & improvements.

### :atom_symbol: Preact

---

fitur kecil yang sering saya lupa saya tambahkan tetapi sangat membantu dengan ukuran bundel adalah [Preact](https://preactjs.com/).

Lihat

```js:next.config.js
webpack: (config, { dev, isServer }) => {
    if (!dev && !isServer) {
        Object.assign(config.resolve.alias, {
            'react': 'preact/compat',
            'react-dom/test-utils': 'preact/test-utils',
            'react-dom': 'preact/compat',
        });
    }

    return config;
},
```

### :book: Blog

---

Seperti yang bisa Anda ketahui dari fakta bahwa Anda sedang membaca ini, saya sekarang punya blog! :tada:

Artinya, saya akhirnya memiliki tempat untuk membuat artikel panjang yang bisa membahas topik yang sangat saya minati secara lebih mendalam. Semuanya, mulai dari tulisan teknis tentang teknologi baru yang saya coba, hingga tulisan pribadi lainnya tentang hobi yang saya sukai, seperti keyboard mekanis.

<XButton href="/blog" icon="feather:external-link" label="Vist my Blog" />

### :clipboard: Projects

---

My new [projects page](/projects) telah didesain ulang untuk memanfaatkan rendering sisi server untuk tujuan yang sangat unik. Halaman ini akan menampilkan sejumlah proyek terpilih yang tersedia untuk umum di repositori GitHub saya. Namun cara pemilihannya sangat unik. Setiap permintaan yang dibuat untuk halaman tersebut (Yang belum di-cache) akan mengembalikan halaman yang baru dirender di sisi server yang kemudian dihidrasi di klien (Seperti yang dilakukan semua SSR). Saat melakukan render, server akan keluar dan mengambil semua repositori GitHub saya yang tersedia & kemudian memfilter semuanya berdasarkan sejumlah filter. Ini termasuk yang berikut: - Repositori tidak diarsipkan - Berisi topik `portofolio` dalam meta data repositori Dari sana kami kemudian menghapus akhiran emoji yang digunakan dalam deskripsi repositori (Ini adalah praktik umum yang saya lakukan untuk menambahkan sentuhan warna :rainbow:) sehingga dapat digunakan sebagai ikon proyek, dengan deskripsi kemudian dikembalikan dengan yang menghapus emoji. Data lainnya yang dikembalikan cukup standar (URL Beranda, URL repositori GitHub, dll). Dengan ini saya dapat memperbarui konten halaman proyek saya dengan menggunakan GitHub sebagai bentuk CMS. Yang perlu saya lakukan untuk menambahkan proyek ke halaman halaman proyek saya adalah menambahkan tag `portofolio` ke salah satu repositori saya.

![Screenshot of the projects page](/blog/hello_world/projects.png 'Screenshot of the projects page')

<XButton href="/projects" icon="feather:external-link" label="Go to Projects" />

Terima kasih, @Yaqub