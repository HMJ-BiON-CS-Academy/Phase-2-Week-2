# Phase-2-Week-2

# JavaScript Week 2: React.js

## 1. Pengenalan React.js

### Penjelasan
React.js adalah pustaka JavaScript yang digunakan untuk membangun antarmuka pengguna (UI) berbasis komponen. React dikembangkan oleh Facebook dan banyak digunakan dalam pengembangan aplikasi web modern karena kecepatan, fleksibilitas, dan efisiensinya dalam mengelola perubahan data.

### Fitur Utama React:
- **Komponen**: UI dibangun dengan komponen yang dapat digunakan kembali.
- **Virtual DOM**: React memperbarui tampilan secara efisien tanpa perlu merender ulang seluruh halaman.
- **State dan Props**: Untuk mengelola data dalam komponen.
- **Hooks**: Fungsi khusus untuk menangani state dan lifecycle dalam komponen fungsi.

---

## 2. Contoh Penggunaan

### Instalasi React
Untuk memulai proyek React, kita bisa menggunakan **Create React App**:
```sh
npx create-react-app my-app
cd my-app
npm start
```

### Membuat Komponen Sederhana
Buat file `Hello.js` di dalam folder `src/components`:
```jsx
import React from 'react';

function Hello() {
    return <h1>Hello, React!</h1>;
}

export default Hello;
```

Gunakan komponen `Hello` di `App.js`:
```jsx
import React from 'react';
import Hello from './components/Hello';

function App() {
    return (
        <div>
            <Hello />
        </div>
    );
}

export default App;
```

### Menggunakan State dengan Hooks
```jsx
import React, { useState } from 'react';

function Counter() {
    const [count, setCount] = useState(0);
    
    return (
        <div>
            <p>Count: {count}</p>
            <button onClick={() => setCount(count + 1)}>Tambah</button>
        </div>
    );
}

export default Counter;
```

Tambahkan komponen `Counter` ke dalam `App.js`.

---

## 3. Assignment

### Tugas 1: Membuat Komponen
1. Buat komponen `Welcome.js` yang menerima `name` sebagai prop dan menampilkan "Hello, [name]!".
2. Gunakan komponen ini di dalam `App.js` dengan mengirimkan nama berbeda.

### Tugas 2: State dan Event Handling
1. Buat komponen `Toggle.js` dengan tombol untuk menampilkan atau menyembunyikan teks saat diklik.
2. Gunakan `useState` untuk mengelola visibilitas teks.

Selamat belajar React! 🚀

