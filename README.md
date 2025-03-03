# Form.jsx
## quantityNum
  Menyediakan array yang berukuran n, kemudian menampilkan angka 1-n untuk menjadi pilihan item quantity.
  - Operator `spread (...)` mengubah array kosong tadi menjadi array dengan 20 elemen undefined.
  - `map()` adalah metode array yang digunakan untuk melakukan loop (perulangan) dan memproses setiap elemen dalam array.
  - Parameter `_` berarti bahwa kita tidak peduli dengan nilai elemen tersebut karena hanya butuh indeksnya (i).
## setQuantity()
  - `useState(1)` membuat state bernama quantity dengan nilai awal 1.
  - `onChange` untuk menghandle perubahan nilai quantity pada div select.
  - penambahan `(e) =>` untuk menangkap event yang terjadi saat pengguna berinteraksi dengan elemen.
  - `e.target.value` mengambil nilai yang dipilih/dimasukkan oleh pengguna.
## setname()
  -  `useState("")` membuat state bernama name dengan nilai awal string kosong ("").
  -  `onChange` untuk menghandle perubahan nilai quantity pada div input.
  -  penambahan `(e) =>` untuk menangkap event yang terjadi saat pengguna berinteraksi dengan elemen.
## onSubmit={handleSubmit}
  - `e` adalah event object yang diberikan otomatis oleh React saat event terjadi. `e` menyimpan informasi tentang event yang sedang berlangsung. Dalam konteks ini, e adalah event dari form submit.
  - Mencegah reload dengan `e.preventDefault()`.
  - Kemudian membuat object newItem dari data yang diterima dari event. Untuk id, dapat diakali dengan menggunakan `Date.now()` yaitu angka yan gmenunjukkan detik secara real-time.
  - `onAddItem(newItem)` untuk menambahkan objek baru ke dalam array.
  - `setname("")` dan `setQuantity(1)` untuk mereset data pada inputan.
