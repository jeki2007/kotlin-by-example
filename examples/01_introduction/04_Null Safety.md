

override fun onNothingSelected(parent: AdapterView<*>) {}
when (operasi) {
    "Penjumlahan" -> soalText.text = "Berapakah $angka1 + $angka2?"
    "Pengurangan" -> soalText.text = "Berapakah $angka1 - $angka2?"
    "Perkalian" -> soalText.text = "Berapakah $angka1 × $angka2?"
    "Pembagian" -> {
        angka1 *= angka2  // agar hasilnya bilangan bulat
        soalText.text = "Berapakah $angka1 ÷ $angka2?"
    }
