# GrokkingDeepLearning

Repository ini berisi ringkasan konsep, eksperimen kode, dan catatan pembelajaran per bab berdasarkan buku *Grokking Deep Learning* karya Andrew W. Trask.

> **Catatan:** notebook di repository ini merupakan materi belajar dan demonstrasi implementasi. Tidak semua notebook mereproduksi seluruh kode, dataset, atau hasil eksperimen buku secara persis. Perbedaan tersebut ditandai di notebook terkait.

## Identitas

- **Nama:** Omar Al Farizy Hutagalung
- **NIM:** 101032300034
- **Mata Kuliah:** Deep Learning

## Daftar Bab

| Bab | Judul/topik | Notebook |
|---:|---|---|
| 1 | Introducing Deep Learning: Why You Should Learn It | [Chapter 01](notebooks/Chapter_01.ipynb) |
| 2 | Fundamental Concepts | [Chapter 02](notebooks/Chapter_02.ipynb) |
| 3 | Introduction to Neural Prediction | [Chapter 03](notebooks/Chapter_03.ipynb) |
| 4 | Introduction to Neural Learning: Gradient Descent | [Chapter 04](notebooks/Chapter_04.ipynb) |
| 5 | Learning Multiple Weights at a Time | [Chapter 05](notebooks/Chapter_05.ipynb) |
| 6 | Building Your First Deep Neural Network | [Chapter 06](notebooks/Chapter_06.ipynb) |
| 7 | How to Picture Neural Networks: In Your Head and on Paper | [Chapter 07](notebooks/Chapter_07.ipynb) |
| 8 | Learning Signal and Ignoring Noise: Introduction to Regularization and Batching | [Chapter 08](notebooks/Chapter_08.ipynb) |
| 9 | Modeling Probabilities and Nonlinearities: Activation Functions | [Chapter 09](notebooks/Chapter_09.ipynb) |
| 10 | Neural Learning About Edges and Corners: Introduction to Convolutional Neural Networks | [Chapter 10](notebooks/Chapter_10.ipynb) |
| 11 | Neural Networks That Understand Language: King − Man + Woman ≈ ? | [Chapter 11](notebooks/Chapter_11.ipynb) |
| 12 | Neural Networks That Write Like Shakespeare: Recurrent Layers for Variable-Length Data | [Chapter 12](notebooks/Chapter_12.ipynb) |
| 13 | Introducing Automatic Optimization: Let’s Build a Deep Learning Framework | [Chapter 13](notebooks/Chapter_13.ipynb) |
| 14 | Learning to Write Like Shakespeare: Long Short-Term Memory | [Chapter 14](notebooks/Chapter_14.ipynb) |
| 15 | Deep Learning on Unseen Data: Introducing Federated Learning | [Chapter 15](notebooks/Chapter_15.ipynb) |

Judul Bab 1–15 mengikuti daftar isi buku. Penulisan kapitalisasi dapat berbeda dari judul yang tampil di buku.

## Isi notebook

Notebook dapat memuat:
- ringkasan konsep dan istilah penting;
- contoh kode yang dapat dijalankan;
- penjelasan keluaran dan interpretasi;
- rangkuman dan pertanyaan refleksi;
- catatan tentang batasan demonstrasi atau perbedaan dari eksperimen asli.

## Catatan metodologi dan batasan

1. Jalankan sel notebook dari atas ke bawah agar variabel dan fungsi sudah tersedia.
2. Beberapa contoh memakai data sintetis atau data kecil buatan untuk menjelaskan mekanisme tanpa mengunduh dataset besar.
3. Jika notebook menggunakan bobot acak, hasilnya adalah demonstrasi mekanisme dan **bukan** hasil pelatihan model yang sudah dipelajari.
4. Bab 8 pada buku membahas eksperimen klasifikasi MNIST, regularisasi, dropout, dan batching. Jika notebook menggunakan data sintetis, notebook tersebut hanya mengilustrasikan konsep dan tidak mereproduksi evaluasi MNIST pada buku.
5. Bab 11–12 memuat contoh pembelajaran bahasa dan representasi urutan. Contoh yang memakai data mainan tidak dapat dianggap sebagai model bahasa yang telah dilatih pada dataset asli.
6. Bab 13 berisi demonstrasi konsep tensor, computation graph, dan autograd. Implementasi sederhana dalam notebook tidak selalu mendukung semua operasi atau seluruh fitur framework deep learning.
7. Bab 14 membahas character language modeling, truncated backpropagation through time (BPTT), vanishing/exploding gradients, dan LSTM. Jika korpus Shakespeare asli tidak disertakan, notebook tidak mengklaim menghasilkan teks Shakespeare yang dipelajari.
8. Bab 15 membahas privasi, federated learning, secure aggregation, dan homomorphic encryption. Simulasi numerik atau contoh enkripsi dasar bukan protokol produksi yang telah diaudit.
9. Jika suatu notebook tidak menjalankan eksperimen asli buku, keterbatasan tersebut harus dinyatakan dengan jelas. Jangan menganggap angka atau keluaran demonstrasi sebagai hasil yang dilaporkan penulis.

## Menjalankan proyek

### Prasyarat

- Python 3
- Git
- Jupyter Notebook atau Visual Studio Code dengan ekstensi Jupyter
- Paket Python sesuai kebutuhan tiap notebook, misalnya `numpy`

### Clone repository

```bash
git clone https://github.com/omralfa/GrokkingDeepLearning.git
cd GrokkingDeepLearning
```

### Membuat virtual environment

**Windows PowerShell:**

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install numpy jupyter
```

Jika PowerShell memblokir aktivasi environment, notebook masih dapat dibuka dengan memilih interpreter `.venv` dari VS Code. Instal paket tambahan hanya jika diperlukan oleh notebook tertentu.

### Membuka notebook

```powershell
code .
```

Buka folder `notebooks/`, pilih bab yang ingin dipelajari, lalu jalankan sel secara berurutan. Jika sebuah notebook menggunakan paket tambahan, pasang paket yang disebutkan pada notebook tersebut.

## Struktur repository

```text
GrokkingDeepLearning/
├── notebooks/
│   ├── Chapter_01.ipynb
│   ├── Chapter_02.ipynb
│   ├── ...
│   └── Chapter_15.ipynb
└── README.md
```

## Referensi

- Andrew W. Trask, *Grokking Deep Learning*, Manning Publications.
- [Repository kode pendamping penulis](https://github.com/iamtrask/Grokking-Deep-Learning)

Materi dan kode di repository ini disusun untuk keperluan pembelajaran. Silakan merujuk ke buku untuk konteks lengkap, penurunan matematis, dataset, dan implementasi asli.
