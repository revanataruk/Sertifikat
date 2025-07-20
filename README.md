graph TD
    subgraph Sistem Prediksi Diabetes
        P1[1.0<br>Input Data Medis]
        P2[2.0<br>Lakukan Prediksi<br>Diabetes]
        P3[3.0<br>Tampilkan<br>Informasi Model]
    end

    EE1(Pengguna)
    DS1([D1<br>Model Decision Tree])
    DS2([D2<br>Dataset Diabetes])

    EE1 -- Data Form Medis --> P1
    P1 -- Data Pasien Baru --> P2
    DS1 -- Parameter Model --> P2
    P2 -- Hasil Prediksi --> EE1
    
    EE1 -- Permintaan Info Model --> P3
    P3 -- Informasi Detail Model --> EE1
    DS1 -- Detail Model --> P3
    DS2 -- Nama & Info Fitur --> P3
