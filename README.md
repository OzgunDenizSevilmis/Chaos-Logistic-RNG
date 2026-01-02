graph TD
    A([BAŞLA]) --> B[/Girdi: Bit Sayısı N/]
    B --> C[Sabitler: r = 3.999999]
    C --> D[Tohum Al: x = Sistem Zamanı]
    D --> E[Sayaç: i = 0]
    E --> F{i < N mi?}
    F -- EVET --> G[Kaos Formülü: x = r * x * 1 - x]
    G --> H[Genişletme: deger = Tamsayı x * 10^14]
    H --> I[Bit Elde Et: bit = deger MOD 2]
    I --> J[/Listeye Ekle: bit/]
    J --> K[Sayaç Artır: i = i + 1]
    K --> F
    F -- HAYIR --> L[/Çıktı: Bit Listesini Yazdır/]
    L --> M([BİTİR])
    
    style A fill:#f9f,stroke:#333,stroke-width:2px
    style M fill:#f9f,stroke:#333,stroke-width:2px
    style F fill:#ff9,stroke:#333,stroke-width:2px
