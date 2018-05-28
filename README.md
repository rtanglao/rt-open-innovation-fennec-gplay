# rt-open-innovation-fennec-gplay
new version of https://github.com/rtanglao/rt-fennec-gplay with open innovation
# 2018-05-28
## 2018-05-28 Getting the reviews for November 14, 2018 - May 27, 2018
```bash
cd ~/Dropbox/GIT/rt-open-innovation-fennec-gplay
. setupDatabase
pushd ~/Documents/MONGO_DATABASES
mongod --config /usr/local/etc/mongod.conf --dbpath . &
popd
wc -l 27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201711.csv 
   28043 27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201711.csv
iconv -f UTF-16 -t UTF-8 27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201711.csv > utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201711.csv
./read-reviews-replies.rb utf8-27may2018-downloaded-reviews_reviews_org.mozilla.firefox_201711.csv 2>27may2018-nov2017-stderr.txt
```
