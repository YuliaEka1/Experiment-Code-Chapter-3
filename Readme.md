# Experiment Code Chapter 3

Nama : Yulia Eka Ardhani==========================================

Kelas : TI 3C / 20

NIM : 2041720054

## Langkah-langkah pengerjaan

### Uji Coba PySpark

Menjalankan service dari pyspark terlebih dahulu dengan perintah 

<code>cd spark-2.0.0-bin-hadoop2.7</code>

<code>bin/pyspark</code>

![](screenshots/pyspark.png)

1. Uji coba <code>Accumulator.py</code>

![](screenshots/accumulator.png)

Hasil : Berhasil. Fungsi accumulator (bertujuan akumulasi shared variable) berhasil dijalankan dengan output "4950".

2. Uji coba <code>BroadCast.py</code>

![](screenshots/broadcast.png)

Hasil : Berhasil. Fungsi Broadcast (Membuat variabel broadcast) sesuai range dan untuk mengakses nilai matriks / array menggunakan atribut broadcastVar.value

3. Uji coba <code>LogAnalytics.py</code>

![](screenshots/LogAnalytics.png)

Hasil : Berhasil. Fungsi filter untuk memfilter kata "Error" dan "product" pada log file. dan Count untuk menghitung jumlahnya.

4. Uji coba <code>PairRDD.py</code>

![](screenshots/PairRDD.png)

Hasil : Berhasil. fungsi dasar dari sebuah collection. 
- method maps digunakan untuk mapping sebuah collection 
    - key: variabel myList
    - value: jumlah huruf dari tiap" kata variabel myList
- myPairRDD.collect(): print collection
- myPairRDD.keys().collect(): print key pada collection
- myPairRDD.values().collect(): print values pada collection

5. Uji coba <code>UnderstandingRDD.py</code>

![](screenshots/rdd_1.png)
![](screenshots/rdd_2.png)

Hasil : Berhasil. Membuat sebuah list, dengan mempraktikan yaitu menghitung jumlah partisi, elemen, menampilkan data pada collection, dan memodifikasi collection (menambahkan atau mengurangi).


6. Uji coba <code>WordCount.py</code>

![](screenshots/wordcount.png)

Hasil : Berhasil. Menghitung jumlah kata yang ada suatu file (test.txt).

### Uji Coba Scala

Menjalankan service dari sparkshell terlebih dahulu dengan perintah 

<code>cd spark-2.0.0-bin-hadoop2.7</code>

<code>bin/spark-shell</code>


![](screenshots/spark-shell.png)

Jalankan juga service cloudera manager dengan perintah:

<code>sudo /home/cloudera/cloudera-manager --express --force</code>

kemudian login pada browser. Setelah itu, jalankan service HDFS


![](screenshots/hdfs.png)

1. Uji coba <code>SystemCommandsOutput.scala</code>

![](screenshots/scala_1.png)

Hasil : Berhasil. Menampilkan list file pada hdfs. Output 0 atau string "" karna belum terdapat file.

2. Uji coba <code>SystemCommandsReturnCode.scala</code>

![](screenshots/scala_2.png)

Hasil : Berhasil. Menampilkan list file pada folder /tmp (temporary file)
