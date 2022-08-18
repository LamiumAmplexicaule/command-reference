# コマンド一覧

Linuxにおけるコマンドを使用方法と共に紹介する．

- [コマンド一覧](#コマンド一覧)
    - [base64](#base64)
    - [cat](#cat)
    - [cp](#cp)
    - [head](#head)
    - [ls](#ls)
    - [mkdir](#mkdir)
    - [mv](#mv)
    - [rm](#rm)
    - [sort](#sort)
    - [tail](#tail)
    - [touch](#touch)
    - [uniq](#uniq)
    - [wc](#wc)

### base64

```base64```はファイルや標準入力から読みよったデータをbase64にエンコードやbase64からデコードする．faviconなどをhtmlに埋め込む際に使う．

```console
user@test ~/c/demo> base64 sample.png
iVBORw0KGgoAAAANSUhEUgAAACAAAAAgEAIAAACsiDHgAAAEsmlUWHRYTUw6Y29tLmFkb2JlLnhtcAAAAAAAPD94cGFja2V0IGJlZ2luPSLvu78iIGlkPSJXNU0wTXBDZWhpSHpyZVN6TlRjemtjOWQiPz4KPHg6eG1wbWV0YSB4bWxuczp4PSJhZG9iZTpuczptZXRhLyIgeDp4bXB0az0iWE1QIENvcmUgNS41LjAiPgogPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4KICA8cmRmOkRlc2NyaXB0aW9uIHJkZjphYm91dD0iIgogICAgeG1sbnM6ZXhpZj0iaHR0cDovL25zLmFkb2JlLmNvbS9leGlmLzEuMC8iCiAgICB4bWxuczp0aWZmPSJodHRwOi8vbnMuYWRvYmUuY29tL3RpZmYvMS4wLyIKICAgIHhtbG5zOnBob3Rvc2hvcD0iaHR0cDovL25zLmFkb2JlLmNvbS9waG90b3Nob3AvMS4wLyIKICAgIHhtbG5zOnhtcD0iaHR0cDovL25zLmFkb2JlLmNvbS94YXAvMS4wLyIKICAgIHhtbG5zOnhtcE1NPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvbW0vIgogICAgeG1sbnM6c3RFdnQ9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC9zVHlwZS9SZXNvdXJjZUV2ZW50IyIKICAgZXhpZjpQaXhlbFhEaW1lbnNpb249IjMyIgogICBleGlmOlBpeGVsWURpbWVuc2lvbj0iMzIiCiAgIGV4aWY6Q29sb3JTcGFjZT0iNjU1MzUiCiAgIHRpZmY6SW1hZ2VXaWR0aD0iMzIiCiAgIHRpZmY6SW1hZ2VMZW5ndGg9IjMyIgogICB0aWZmOlJlc29sdXRpb25Vbml0PSIyIgogICB0aWZmOlhSZXNvbHV0aW9uPSIzMDAvMSIKICAgdGlmZjpZUmVzb2x1dGlvbj0iMzAwLzEiCiAgIHBob3Rvc2hvcDpDb2xvck1vZGU9IjMiCiAgIHBob3Rvc2hvcDpJQ0NQcm9maWxlPSJEaXNwbGF5IFAzIgogICB4bXA6TW9kaWZ5RGF0ZT0iMjAyMi0wOC0xNFQxMTozNjo1MiswOTowMCIKICAgeG1wOk1ldGFkYXRhRGF0ZT0iMjAyMi0wOC0xNFQxMTozNjo1MiswOTowMCI+CiAgIDx4bXBNTTpIaXN0b3J5PgogICAgPHJkZjpTZXE+CiAgICAgPHJkZjpsaQogICAgICBzdEV2dDphY3Rpb249InByb2R1Y2VkIgogICAgICBzdEV2dDpzb2Z0d2FyZUFnZW50PSJBZmZpbml0eSBEZXNpZ25lciAxLjEwLjUiCiAgICAgIHN0RXZ0OndoZW49IjIwMjItMDgtMTRUMTE6MzY6NTIrMDk6MDAiLz4KICAgIDwvcmRmOlNlcT4KICAgPC94bXBNTTpIaXN0b3J5PgogIDwvcmRmOkRlc2NyaXB0aW9uPgogPC9yZGY6UkRGPgo8L3g6eG1wbWV0YT4KPD94cGFja2V0IGVuZD0iciI/Pma0/lcAAAFpaUNDUERpc3BsYXkgUDMAACiRdZC9S8NQFMVPq1LQOogOHRwyiUPU0gp2cWgrFEUwVAWrU/r6JTQxJClScRNXKfgfWMFZcLCIVHBxcBBEBxHdnDopuGh53pdU2iLex+X9OJxzuVzAGygyzeoFoOm2mUzEpLXUuuR7g4eeUyqzjKiiLAr+/bvr89H13k+IWY1m9SCyn7jWzi6Xdp4CU3/9XdWfyVqM/m/qIDNMG/DIxMq2bQjeJR4xaSniiuC8y8eC0y6fO56VZJz4llhiBTVD3CCW0x16voO1Yom1dhDb+7P66rKYQz2KOWzCgoEiVJQhQUH4H/+0449ji9xlmJTLowCbMlFSxIQs8Tx0MExCJg4hSB0Sd27d76F1P7mt7b0Cs3XO+UVbW6gDpzN0slpbG48AQwPATc1QTdWReqi9uRzwfgIMpoDhO8psWLlwyN3eHwP6Xjj/GAN8h0CzwvnXEefNKoWfgSv9Bx7dasBKz1nRAAAACXBIWXMAAC4jAAAuIwF4pT92AAAAS0lEQVRYhe3PMQ2AMAAAwdIF/2q6YgADKEAGIjpcSP4U/B/X/ZzvGr81dcCuBrQGtAa0BrQGtAa0BrQGtAa0BrQGtAa0BrQGtAa0D83GBE233FUrAAAAAElFTkSuQmCC
```

### cat

```cat```はファイルや標準入力を標準出力へコピーする．そのためファイルを見るときなどに使われる．

```console
user@test ~/c/demo> cat test.txt
Test Text File
```
<!-- ### chmod
### chown -->
### cp

```cp```はファイルやディレクトリをコピーする．

よく使うオプション

- ```r``` ディレクトリを再帰的にコピーする．

```console
user@test ~/c/demo> cat test.txt
Test Text File
user@test ~/c/demo> cp test.txt test_copied.txt
user@test ~/c/demo> cat test_copied.txt
Test Text File
user@test ~/c/demo> cat test_dir/test.txt 
Test Text File in Deep
user@test ~/c/demo> cp -r test_dir test_copied_dir
user@test ~/c/demo> cat test_copied_dir/test.txt 
Test Text File in Deep
```
<!-- ### cut
### dd
### fold -->
### head

```head```は各ファイルの先頭n行を表示する．デフォルトはn=10．

よく使うオプション

- ```n num``` 先頭からnum行表示する．-numであれば末尾からnum行除いて表示する．

```console
user@test ~/c/demo> head -n 3 sort.txt
a
g
d
user@test ~/c/demo> head -n -1 sort.txt
a
g
d
b
e
k
user@test ~/c/demo> last | head
user    pts/0        192.168.11.99    Tue Aug 16 17:21   still logged in
user    pts/0        192.168.11.99    Mon Aug 15 12:38 - 12:38  (00:00)
user    pts/0        192.168.11.99    Sun Aug 14 13:42 - 13:42  (00:00)
user    pts/0        192.168.11.99    Sun Aug 14 13:26 - 13:28  (00:02)
user    pts/0        192.168.11.99    Sun Aug 14 12:42 - 12:42  (00:00)
user    pts/0        192.168.11.99    Sun Aug 14 12:38 - 12:42  (00:03)
user    pts/0        192.168.11.99    Sun Aug 14 11:24 - 11:24  (00:00)
user    pts/0        192.168.11.99    Sun Aug 14 11:07 - 11:23  (00:16)
user    pts/0        192.168.11.99    Sun Aug 14 11:00 - 11:05  (00:04)
user    pts/0        192.168.11.99    Sun Aug 14 10:41 - 11:00  (00:19)
```

### ls

```ls```はファイルやディレクトリの情報を一覧表示する．

よく使うオプション

- ```a``` .から始まるファイルも表示する．
- ```l``` ファイル名以外の情報を表示する．
- ```h``` ファイルサイズなどに単位を付ける(SI接頭辞ではなく，2進接頭辞である)．

```console
user@test ~/c/demo> ls
sample.png       sort.txt         test.txt         test_copied.txt  test_copied_dir/ test_dir/
user@test ~/c/demo> ls -lah
total 20K
drwxr-xr-x 8 user user  256 Aug 14 02:47 .
drwxr-xr-x 3 user user 4.0K Aug 16 07:32 ..
-rw-r--r-- 1 user user 1.7K Aug 14 02:36 sample.png
-rw-r--r-- 1 user user   14 Aug 12 08:53 sort.txt
-rw-r--r-- 1 user user   15 Aug 12 08:50 test.txt
-rw-r--r-- 1 user user   15 Aug 14 02:42 test_copied.txt
drwxr-xr-x 3 user user   96 Aug 14 02:47 test_copied_dir
drwxr-xr-x 3 user user   96 Aug 14 02:47 test_dir
```

### mkdir

```mkdir```はディレクトリを作成する．

よく使うオプション

- ```p``` 存在していない親ディレクトリが存在すれば作成し，存在していれば何もしない．

```console
user@test ~/c/demo> ls
sample.png  sort.txt  test.txt  test_copied.txt  test_copied_dir  test_di
user@test ~/c/demo> mkdir test_dir2
user@test ~/c/demo> ls
sample.png  sort.txt  test.txt  test_copied.txt  test_copied_dir  test_dir  test_dir2
user@test ~/c/demo> mkdir test_dir
mkdir: cannot create directory 'test_dir': File exists
user@test ~/c/demo> mkdir -p test_dir
user@test ~/c/demo> 
```

### mv

```mv```はファイルの移動を行う．名前変更にも使われる．

よく使うオプション

- ```i``` 移動先にファイルが存在したとき，上書きするかをユーザに問い合わせる．
- ```n``` 存在するファイルを上書きしない．

```console
user@test ~/c/demo> ls
from             sample.png       sort.txt         test.txt         test_copied.txt  test_copied_dir/ test_dir/ to2
user@test ~/c/demo> mv from to
user@test ~/c/demo> ls
sample.png  sort.txt  test.txt  test_copied.txt  test_copied_dir  test_dir  to  to2
user@test ~/c/demo> mv -i to to2
mv: overwrite 'to2'? n
user@test ~/c/demo> ls
sample.png  sort.txt  test.txt  test_copied.txt  test_copied_dir  test_dir  to  to2
user@test ~/c/demo> mv -i to to2
mv: overwrite 'to2'? y
user@test ~/c/demo> ls
sample.png  sort.txt  test.txt  test_copied.txt  test_copied_dir  test_dir  to2
```

### rm

```rm```はファイルやディレクトリを削除する．

よく使うオプション

- ```f``` ユーザに問い合わせをせず，エラーを表示しない．
- ```r``` ディレクトリとその中身を再帰的に削除する．

```console
user@test ~/c/demo> ls
sample.png  sort.txt  test.txt  test_copied.txt  test_copied_dir  test_dir  to2
user@test ~/c/demo> rm to2
user@test ~/c/demo> ls
sample.png  sort.txt  test.txt  test_copied.txt  test_copied_dir  test_dir
user@test ~/c/demo> rm to2
rm: cannot remove 'to2': No such file or directory
user@test ~/c/demo> rm -f to2
user@test ~/c/demo>
```

### sort

```sort```はファイルから読み込んだ行に対してソートを行う．

```console
user@test ~/c/demo> cat sort.txt
a
g
d
b
e
k
c
user@test ~/c/demo> sort sort.txt 
a
b
c
d
e
g
k
```

### tail

```tail```は各ファイルの末尾n行を表示する．デフォルトはn=10．

よく使うオプション

- ```n num``` 末尾からnum行表示する．+numであれば先頭からnum-1行除いて表示する．

```console
user@test ~/c/demo> tail -n 3 sort.txt
e
k
c
user@test ~/c/demo> tail -n +2 sort.txt
g
d
b
e
k
c
user@test ~/c/demo> last | head
user    pts/0        192.168.11.99    Tue Aug 16 17:21   still logged in
user    pts/0        192.168.11.99    Mon Aug 15 12:38 - 12:38  (00:00)
user    pts/0        192.168.11.99    Sun Aug 14 13:42 - 13:42  (00:00)
user    pts/0        192.168.11.99    Sun Aug 14 13:26 - 13:28  (00:02)
user    pts/0        192.168.11.99    Sun Aug 14 12:42 - 12:42  (00:00)
user    pts/0        192.168.11.99    Sun Aug 14 12:38 - 12:42  (00:03)
user    pts/0        192.168.11.99    Sun Aug 14 11:24 - 11:24  (00:00)
user    pts/0        192.168.11.99    Sun Aug 14 11:07 - 11:23  (00:16)
user    pts/0        192.168.11.99    Sun Aug 14 11:00 - 11:05  (00:04)
user    pts/0        192.168.11.99    Sun Aug 14 10:41 - 11:00  (00:19)
```

### touch

```touch```はファイルのアクセス日時や更新日時を変更する．空ファイルを作成するときにも使われる．

```console
user@test ~/c/demo> ls
sample.png  sort.txt  test.txt  test_copied.txt  test_copied_dir  test_dir  test_dir2  uniq.txt
user@test ~/c/demo> touch touch
user@test ~/c/demo> ls
sample.png  sort.txt  test.txt  test_copied.txt  test_copied_dir  test_dir  test_dir2  touch  uniq.txt
```

### uniq

```uniq```はファイルから読み込んだ行の重複を除いて表示する．

```console
user@test ~/c/demo> cat uniq.txt 
u
u
n
n
i
i
i
q
q
q
q
q
user@test ~/c/demo> uniq uniq.txt 
u
n
i
q
```

### wc

```wc```は指定されたファイルのバイト数，文字数，ホワイトスペースで区切られた単語数，改行数をカウントする．ファイル数のカウントに使ったりする．

よく使うオプション

- ```w``` 単語数のみを表示する．
- ```l``` 改行数のみを表示する．

```console
user@test ~/c/demo> wc test.txt
1  3 15 test.txt
user@test ~/c/demo> ls
sample.png  sort.txt  test.txt  test_copied.txt  test_copied_dir  test_dir  test_dir2  touch  uniq.txt
user@test ~/c/demo> ls | wc -w
9
```
