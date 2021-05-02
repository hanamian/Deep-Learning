# MNIST (_Modified National Institute of Standards and Technology_)
---
MNIST bagus dipakai untuk digit recognition. Dataset MNIST berisi 70000 images angka dari 0 s/d 9 (10 kelas) yang ditulis tangan. Setiap gambar berukuran 28 x 28 pixels = 784 pixel persegi dan terlihat sebagai Matrix. MNIST sendiri lekat dengan penggunaan CNN.

![image](https://user-images.githubusercontent.com/49611937/116769586-6e12a080-aa67-11eb-9ac4-6e6b135a933c.png)

Matrix 28 x 28 pixels ini ditransformasi ke bentuk 784 x 1, sehingga semuanya menjadi input (784 pixels). Setiap pixels memiliki intensitas warna, 0=putih, 1=hitam.

Implementasi di dataset MNIST sendiri biasanya terdiri dari input layer, hidden layer, dan **Activation Function Softmax**. Fungsi Softmax ini akan menghasilkan output dengan cara menentukan probabilitas output. Index output yang dimiliki adalah 0, 1, 2, 3, 4, 5, 6, 7, 8, 9. Sedangkan contoh outputnya:
- [0.2, 0, 0, 0.1, 0, 0, 0, 0, 0.8, 0] = artinya model yakin 80% bahwa angkanya adalah 8
- [0, 0, 0, 0, 1, 0, 0, 0, 0, 0] = artinya model yakin 100% bahwa angkanya adalah 4
- [0, 0.9, 0, 0, 0, 1, 0, 0, 0, 0] = artinya model yakin 90% bahwa angkanya adalah 1

![image](https://user-images.githubusercontent.com/49611937/116800802-7d105600-ab2e-11eb-834e-8110a8b2e307.png)

