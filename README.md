# Informed-Search-Algorithm

## Daftar Isi
- [Group Introduction](#group-introduction)
- [Description](#description)
- [Terminology](#terminology)
- [Greedy Best First Search](#greedy-best-first-search)
- [A* Search](#a*-search)
- [Comparative Analysis](#comparative-analysis)
- [Conclusion](#conclusion)


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
- f(n) adalah cost/jarak total dari current state ke goal state
- h(n) adalah hasil dari heuristic function

## A* Search

## Comparative Analysis

## Conclusion