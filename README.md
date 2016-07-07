```
sudo apt-get install libxslt-dev libxml2-dev libxml2
sudo pip install lxml
sudo pip install numpy
sudo pip install sumy
```

`find ./Samples -type f -print -exec sumy lex-rank --length=3 --file={} \;`

`for i in luhn edmundson lsa text-rank lex-rank sum-basic kl; do echo $i; find ./Samples -type f -print -exec sumy $i --length=3 --file={} \; ; done; > results.txt`
