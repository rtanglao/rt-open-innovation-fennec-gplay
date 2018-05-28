# rt-open-innovation-fennec-gplay
new version of https://github.com/rtanglao/rt-fennec-gplay with open innovation
# 2018-05-28
## 2018-05-28 Getting the reviews for November 14, 2017 - May 27, 2018
### 2018-05-28 November 2017
```bash
cd ~/Dropbox/GIT/rt-open-innovation-fennec-gplay
. setupDatabase
pushd ~/Documents/MONGO_DATABASES
mongod --config /usr/local/etc/mongod.conf --dbpath . &
popd
# for some bizarre reason google uses UTF-16 so convert to UTF-8
iconv -f UTF-16 -t UTF-8 27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201711.csv > utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201711.csv
wc -l utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201711.csv 
   27866 utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201711.csv
./read-reviews-replies.rb utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201711.csv 2>27may2018-nov2017-stderr.txt
# 27865 rows inserted
zip -e nov2017-ratings-reviews-archive.zip utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201711.csv
zip -e nov2017-stderr-archive.zip 27may2018-nov2017-stderr.txt
```

### 2018-05-28 December 2017

```bash
iconv -f UTF-16 -t UTF-8 27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201712.csv > utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201712.csv
wc -l utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201712.csv 
   22043 utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201712.csv
./read-reviews-replies.rb utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201712.csv 2>27may2018-dec2017-stderr.txt
# 22042 rows inserted
zip -e dec2017-ratings-reviews-archive.zip utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201712.csv
zip -e dec2017-stderr-archive.zip 27may2018-dec2017-stderr.txt
```

### 2018-05-28 January 2018

```bash
iconv -f UTF-16 -t UTF-8 27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201801.csv > utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201801.csv
wc -l utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201801.csv 
   22021 utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201801.csv
./read-reviews-replies.rb utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201801.csv 2>27may2018-jan2018-stderr.txt
# 22020 rows inserted
zip -e jan2018-ratings-reviews-archive.zip utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201801.csv
zip -e jan2018-stderr-archive.zip 27may2018-jan2018-stderr.txt
```

### 2018-05-28 February 2018

```bash
iconv -f UTF-16 -t UTF-8 27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201802.csv > utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201802.csv
wc -l utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201802.csv 
   16843 utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201802.csv
./read-reviews-replies.rb utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201802.csv 2>27may2018-feb2018-stderr.txt
# 16842 rows inserted
zip -e feb2018-ratings-reviews-archive.zip utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201802.csv
zip -e feb2018-stderr-archive.zip 27may2018-feb2018-stderr.txt
```

### 2018-05-28 March 2018

```bash
iconv -f UTF-16 -t UTF-8 27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201803.csv > utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201803.csv
wc -l utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201803.csv 
   17869 utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201803.csv
./read-reviews-replies.rb utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201803.csv 2>27may2018-mar2018-stderr.txt
# 17868 rows inserted
zip -e mar2018-ratings-reviews-archive.zip utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201803.csv
zip -e mar2018-stderr-archive.zip 27may2018-mar2018-stderr.txt
```

### 2018-05-28 April 2018

```bash
iconv -f UTF-16 -t UTF-8 27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201804.csv > utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201804.csv
wc -l utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201804.csv 
   16067 utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201804.csv
./read-reviews-replies.rb utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201804.csv 2>27may2018-apr2018-stderr.txt
# 16066 rows inserted
zip -e apr2018-ratings-reviews-archive.zip utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201804.csv
zip -e apr2018-stderr-archive.zip 27may2018-apr2018-stderr.txt
```

### 2018-05-28 May 2018

```bash
iconv -f UTF-16 -t UTF-8 27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201805.csv > utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201805.csv
wc -l utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201805.csv 
   16067 utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201805.csv
./read-reviews-replies.rb utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201805.csv 2>27may2018-may2018-stderr.txt
# 16066 rows inserted
zip -e may2018-ratings-reviews-archive.zip utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201805.csv
zip -e may2018-stderr-archive.zip 27may2018-may2018-stderr.txt
```
