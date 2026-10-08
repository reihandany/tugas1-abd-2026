# Data Tugas 1

## Dataset yang Dipilih

| Item | Isi |
|---|---|
| Nama dataset | APBD Pemda Indonesia (`apbd-pemda-indonesia`) |
| Sumber | Hugging Face Datasets (`https://huggingface.co/datasets/pohonmaple/apbd-pemda-indonesia`) |
| Format lokal | CSV |
| Ukuran lokal | ±123 MB |
| Jumlah baris | 1.155.181 |
| Periode data | 2011–2025 |
| Unit analisis | Data rincian akun APBD per Pemerintah Daerah (Provinsi/Kabupaten/Kota) berdasarkan tahun dan bulan |

Dataset memenuhi persyaratan dataset skala besar pada Milestone 1
karena memiliki lebih dari 1 juta baris.

## Sumber Dataset

Dataset diperoleh melalui Hugging Face Datasets:

https://huggingface.co/datasets/pohonmaple/apbd-pemda-indonesia

Dataset memiliki 1.155.181 baris dan memuat informasi antara lain tahun,
bulan, provinsi, pemerintah daerah, akun APBD, anggaran, realisasi,
dan persentase.

## Cara Memperoleh Data

Dataset dapat diperoleh menggunakan library `datasets` dari Hugging Face
atau melalui halaman dataset pada sumber resmi.

Contoh menggunakan Python:

```python
from datasets import load_dataset

dataset = load_dataset(
    "pohonmaple/apbd-pemda-indonesia",
    split="train"
)