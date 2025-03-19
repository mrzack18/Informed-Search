# Informed Search

Informed Search, atau dikenal juga sebagai Heuristic Search, adalah algoritma pencarian yang menggunakan pengetahuan khusus (heuristik) untuk menemukan solusi lebih efisien dibandingkan metode pencarian tanpa informasi tambahan (uninformed search). Repositori ini mendemonstrasikan dua algoritma pencarian berbasis heuristik yang populer:  

## 1. A* (A-Star) Search  
A* Search menggabungkan keunggulan dari Uniform Cost Search dan Greedy Best-First Search. Algoritma ini menggunakan:  
- **g(n)**: Biaya dari node awal ke node saat ini  
- **h(n)**: Estimasi heuristik jarak ke tujuan  
- **f(n) = g(n) + h(n)**: Total biaya yang digunakan untuk memilih jalur  

### Karakteristik A* Search:  
- **Komplet**: Selalu menemukan solusi jika jalurnya ada  
- **Optimal**: Menjamin jalur terpendek  
- **Lebih efisien** dibandingkan algoritma uninformed  

## 2. Greedy Best-First Search  
Greedy Best-First Search adalah algoritma yang menggunakan heuristik untuk memperkirakan jarak ke tujuan. Algoritma ini:  
- Selalu memilih node yang paling dekat dengan tujuan  
- Membuat keputusan optimal secara lokal  
- Lebih cepat, tetapi tidak selalu menemukan jalur terpendek  

## Detail Implementasi  
Kedua algoritma ini diimplementasikan dengan:  
- **Priority Queue** untuk manajemen frontier  
- **Dictionary/HashMap** untuk merepresentasikan graf  
- **Fungsi heuristik** untuk estimasi jarak  

## Struktur Graf Contoh  
Implementasi menggunakan graf yang terdiri dari:  
- **Node**: S (Start), A, B, C, D, G (Goal)  
- **Nilai heuristik** untuk setiap node  
- **Koneksi antar-node** dengan biaya perjalanan (untuk A*)  

## Penggunaan  
Repositori ini berisi notebook Jupyter untuk setiap algoritma:  
- `a_star_search.ipynb`: Implementasi A* Search  
- `greedy_best_first_search.ipynb`: Implementasi Greedy Best-First Search  

Setiap notebook mencakup:  
- Implementasi algoritma  
- Representasi graf  
- Contoh eksekusi dengan hasil  
