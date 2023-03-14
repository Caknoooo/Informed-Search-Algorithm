# Informed-Search-Algorithm

## Daftar Isi
- [Group Introduction](#group-introduction)
- [Description](#description)
- [Terminology](#terminology)
- [Greedy Best First Search](#greedy-best-first-search)
- [A* Search](#a*-search)
- [Implementation Details](#implementation-details)
- [Comparative Analysis](#comparative-analysis)
- [Conclusion](#conclusion)
- [References](#references)


## Group Introduction
<b>Kelompok 06 Kecerdasan Buatan D</b> :
| Nama                      | NRP        |
|---------------------------|------------|
|Calvin Janitra             | 5025211020 |
|Kevin Nathanael Halim      | 5025211140 |
|M. Zhafran Dzaky           | 5025211142 |
|M. Naufal Badruttamam      | 5025211240 |

## Description
Pada repository ini, kami mengimplementasikan 2 Algoritma Informed Search yaitu <b>Greedy Best First Search Algorithm</b> dan <b>A* Algorithm</b> menggunakan bahasa Python ke dalam file dengan format <i>.ipynb</i> untuk menjalankan satu contoh kasus yang telah diberikan.<br>
Contoh kasus yang digunakan sendiri adalah contoh kasus pada powerpoint yakni Romania Problem yang merupakan permasalahan klasik untuk Informed Search. Pada permasalahan tersebut terdapat peta Romania yang terdiri dari beberapa kota dengan diberikan informasi jarak antar kota-kota yang ada. Tujuan pada kasus yang digunakan adalah untuk melakukan pencarian jalur terpendek untuk pergi dari satu kota ke yang lain, dalam hal ini adalah dari Aran ke Bucharest.<br>
Tujuan : Untuk mengetahui bagaimana performa kedua metode informed search tersebut dan perbandingannya antara yang satu dengan yang lain.

## Terminology
- Informed Search : Sebuah algoritma pencarian/search dimana terdapat informasi tambahan untuk mencapai goal state yang tentunya akan sangat membantu dalam proses pencarian secara efisien. Disebut juga dengan Heuristic Search.
- Start State : Keadaan/kondisi awal sebelum pencarian mulai dijalankan.
- Current State : Keadaan/kondisi terkini pada pencarian.
- Goal State : Keadaan/kondisi tujuan yang ingin dicari.
- Heuristic Functions : Fungsi pembantu yang digunakan dalam Informed Search untuk membantu mencari jalur pencarian yang paling menjanjikan dengan cara melakukan perkiraan jarak dari state terkini dengan goal state. Walaupun terdapat beberapa metode heuristik yang dapat digunakan dalam fungsi ini, tetapi semuanya akan membantu dalam membuat proses pencarian lebih efisien.

## Greedy Best First Search
Greedy Best First Search adalah salah satu algoritma Informed Search yang bekerja dengan memilih satu jalur pencarian yang terlihat menjanjikan atau terbaik saat itu. Merupakan hasil penggabungan dari algoritma Depth-First Search dan Breadth-First Search sehingga lebih efisien dari keduanya karena dapat bergerak dengan memilih mana yang lebih baik dari kedua algoritma tersebut sesuai dengan kondisi terkini.<br>
Cara kerja algoritma Greedy BFS ini sendiri adalah dengan memanfaatkan Heuristic Functions untuk menentukan jarak dari state terkini ke goal state dan memilih node yang terlihat paling baik (jaraknya paling dekat) pada setiap langkah pencarian hingga goal state tercapai. Algoritma ini dapat diimplementasikan menggunakan struktur data Priority Queue. Perumusan yang digunakan untuk menentukan cost terbaik dari node yang akan dilalui sendiri sebagai berikut,

    f(n) = h(n)
Dimana :
- f(n) adalah hasil dari fungsi yang berupa cost/jarak total dari current state ke goal state
- h(n) adalah heuristic function yang dipergunakan

## A* Search

## Implementation Details
1. Diawali dengan pembuatan class PriorityQueue yang merupakan implementasi dari struktur data Priority Queue untuk membantu simulasi implementasi algoritma Greedy BFS
2. Dibuat juga class CityNode yang merupakan class untuk melambangkan setiap node/kota yang ada pada peta Romania
3. Dibuat fungsi makeDict() yang digunakan untuk mengambil data kota-kota beserta dengan jarak antar tiap kota dari dalam file Jalan.txt yang akan dipergunakan untuk membangun graph untuk mewakili peta Romania pada kasus
4. Dibuat juga fungsi makeHeuristicDict() yang digunakan untuk mengambil data informasi tambahan yang terdapat pada file HeuristicJalan.txt yang nantinya akan dipergunakan sebagai fungsi heuristic untuk proses pencarian
5. Kemudian dibuat fungsi pencarian Greedy BFS dan A* yang akan melakukan pencarian dengan perbedaan dimana pada A* Search nilai yang diperoleh dari heuristic function ditambahkan dengan nilai distance atau cost dari start state ke current state, sementara pada Greedy BFS hanya digunakan nilai dari heuristic function saja
6. Setelah itu, dibuat fungsi PrintOutput yang akan mengeluarkan hasil dari proses pencarian dengan format sesuai yang telah dispesifikasikan. Yakni terdiri dari kota yang sempat terjelajahi saat proses searching dan juga jarak terpendek yang didapatkan sebagai hasil pencarian yang ditambah dengan jumlah kota serta jarak pencariannya (depth).
7. Terakhir, barulah dibuat fungsi main dimana semuanya dimulai, dengan masukkan start state adalah kota Aran dan goal statenya kota Bucharest.

## Comparative Analysis

## Conclusion

## References
- [https://www.javatpoint.com/ai-informed-search-algorithms](https://www.javatpoint.com/ai-informed-search-algorithms)
- [https://www.geeksforgeeks.org/difference-between-informed-and-uninformed-search-in-ai](https://www.geeksforgeeks.org/difference-between-informed-and-uninformed-search-in-ai)
- [https://socs.binus.ac.id/2013/04/23/uninformed-search-dan-informed-search](https://socs.binus.ac.id/2013/04/23/uninformed-search-dan-informed-search)