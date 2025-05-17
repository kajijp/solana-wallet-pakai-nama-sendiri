# Generate alamat wallet Solana pakai nama kita
ini adalah tutorial untuk generate alamat wallet solana dengan nama kita sendiri, sangat mudah sekali, cukup dengan beberapa perintah saja sudah jadi wallet dengan nama yang kalian inginkan

## Download Solana CLI di VPS Kalian
```
curl -LO https://github.com/solana-labs/solana/releases/latest/download/solana-release-x86_64-unknown-linux-gnu.tar.bz2
```
## Ekstrak file yang sudah didownload
```
tar -xvjf solana-release-x86_64-unknown-linux-gnu.tar.bz2
```
## Masuk ke folder Solana
```
cd solana-release
```
## Atur Path
```
echo 'export PATH="$PWD/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```
### Cek Versi Solana
```
solana --version
```
## Generate Wallet Solana
```
solana-keygen grind --starts-with kajijp:1 --ignore-case
```

### Keterangan
--starts-with = ini berfungsi untuk menentukan nama depan wallet<br>
--ends-with = ini berfungsi untuk menentukan nama belakang wallet<br>
kajijp:1 = Ganti "kajijp" dengan kata yang kalian inginkan dan angka 1 adalah jumlah wallet yang kalian inginkan<br>
--ignore-case = ini berfungsi untuk menghiraukan besar kecilnya kata, jika tanpa ini, maka wallet akan mencari yang sangat mirip dengan yang kalian inginkan<br>



