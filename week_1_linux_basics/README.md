# Week 1 - Linux Basics Homework

Bootcamp kapsamında verilen Linux temel komutlar ödevi.

## 1. `linux_basic` klasörü oluşturma

```bash
mkdir linux_basic
cd linux_basic
```

## 2. `dataops` klasörü ve dataset indirme

```bash
mkdir dataops
cd dataops
curl -O https://raw.githubusercontent.com/erkansirin78/datasets/master/Churn_Modelling.csv
```

## 3. `/etc` dizininde `.conf` ile biten dosyaları listeleme

```bash
ls /etc/*.conf
```

## 4. `dataops.txt` dosyası oluşturma ve okuma

```bash
echo "Hello! DataOps Bootcamp has started." > dataops.txt
cat dataops.txt
```

## 5. `yellow` klasörü işlemleri

```bash
mkdir yellow
cd yellow

echo "My Name is Red" > red.txt
echo "My Name is Blue" > blue.txt

cat red.txt >> blue.txt
cat blue.txt >> red.txt

cp red.txt ../red_copied.txt
cp blue.txt ../blue_copied.txt

brew install tree
tree yellow
```

## 6. Wine.csv işlemleri

```bash
mkdir -p ~/datasets
cd ~/datasets
curl -O https://raw.githubusercontent.com/erkansirin78/datasets/master/Wine.csv

head -15 Wine.csv

awk -F',' 'NR==1 || $1 > 14.0' Wine.csv
```
