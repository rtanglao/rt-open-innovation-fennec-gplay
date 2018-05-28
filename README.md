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
   27866 utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201712.csv
./read-reviews-replies.rb utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201712.csv 2>27may2018-dec2017-stderr.txt
# 27865 rows inserted
zip -e dec2017-ratings-reviews-archive.zip utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201712.csv
zip -e dec2017-stderr-archive.zip 27may2018-dec2017-stderr.txt
```
