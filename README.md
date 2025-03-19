# Informed Search

Informed Search, nu disebut ogé Heuristic Search, nyaéta algoritma nu make pangaweruh khusus (heuristic) pikeun manggihan solusi leuwih éfisién tibatan metode search nu teu make informasi tambahan (uninformed search). Ieu repository nembongkeun dua algoritma search informed anu kawentar:  

## 1. A* (A-Star) Search  
A* Search ngahijikeun kaunggulan tina Uniform Cost Search jeung Greedy Best-First Search. Algoritma ieu make:  
- **g(n)**: Biaya ti node awal ka node ayeuna  
- **h(n)**: Estimasi heuristic jarak ka tujuan  
- **f(n) = g(n) + h(n)**: Total biaya nu dipaké keur milih jalur  

### Fitur-fitur A* Search:  
- **Komplit**: Salawasna manggihan solusi mun aya jalanna  
- **Optimal**: Mastikeun jalur pangpondokna  
- **Leuwih éfisién** batan algoritma uninformed  

## 2. Greedy Best-First Search  
Greedy Best-First Search nyaeta algoritma nu make heuristic pikeun ngira-ngira jarak ka tujuan. Algoritma ieu:  
- Salawasna milih node nu pangdeukeutna ka tujuan  
- Nyokot kaputusan optimal dina tingkat lokal  
- Gancang, tapi teu salawasna manggihan jalur pangpondokna  

## Detil Implementasi  
Kadua algoritma ieu diimplementasikeun make:  
- **Priority Queue** pikeun ngatur frontier  
- **Dictionary/HashMap** pikeun ngawakilan graph  
- **Fungsi heuristic** pikeun estimasi jarak  

## Struktur Graph Conto  
Implementasi make graph nu diwangun ku:  
- **Node**: S (Mimitian), A, B, C, D, G (Tujuan)  
- **Nilai heuristic** keur tiap node  
- **Sambungan node** jeung biaya perjalanan (pikeun A*)  

## Pamakean  
Repository ieu ngandung notebook Jupyter pikeun tiap algoritma:  
- `a_star_search.ipynb`: Implementasi A* Search  
- `greedy_best_first_search.ipynb`: Implementasi Greedy Best-First Search  

Unggal notebook ngandung:  
- Implementasi algoritma  
- Representasi graph  
- Conto éksekusi jeung hasilna  
