# Week Start Ops

## Main Office
- Buatkan semua orderan ke SDA
- Tawarkan customer lebih kecil dari 5jt untuk pengmbilan di SBY
	- Jika pengambilan di bawah 5jt, tawarkan customer untuk pengambilan di SBY
	- Jika pengambilan di atas 5jt, beri pemahaman bahwa di SBY stock terbatas
	- Jika customer tetap ingin ambil dari SBY
		- Jika stock mencukupi, layani sesuai permintaan customer (Tetap harus memudahkan kebutuhan customer terlebih dahulu)
		- Jika stock tidak mencukupi, beri pemahaman bahwa kita belum stock balancing, dan perkiraan barang ready di SBY bisa 2 sampai 3 hari 
- Untuk pindah orderan, pakai sistem pindah orderan di halaman Reset Order
- Kalau pindah mau di picker ulang ga? #Deliberate
- Posisi sdh picker harus reset order terlebih dahulu baru pindah cabang #Develop 
  (Kedepannya ubah jadi reset picker, jgn hrs reset order #Develop)

## Bagi Rute
- Login menggunakan akun bagi_rute
	- Kirim mobil
	- Pindah invoice2 ke cabang seharusnya
- jika pindah, pakai sistem pindah cabang di halaman Reset Order

## Proses Invoice
- @Team_Surabaya hanya proses ambil sendiri (offline). Orderan lainnya (otp, dst) hanya boleh diproses @Main_Office
- Customer checkout sendiri lalu datang langsung dan menunjukkan bukti transfer dianggap offline
- Customer datang langsung dan minta kirim kurir toko/gojek diarahkan ke @Main_Office

1. @Main_Office melakukan stock masuk stock keluar 
	1. Stock keluar: 
		1. Create invoice with HPP price to akun cabang
			- Note: Akun cabang supaya masuk di kategori cabang bukan sebagai Loss)
	2. Stock masuk: 
		1. Login ke cabang [^1] 
		2. Input di Spurcinv [^2]
2. Siap Pengiriman 
	- Same as [[#Half Loading Full Loading|Pengiriman]]

## Stock Balancing
Smaller_Branch ambil barang sesuai estimasi stock keluar selama 1 bulan  
(Limits: Not scalable after more than a single warehouse #Limits)

### Init
1. @Team_Surabaya create balancing request
2. Buka halaman Pergerakan Stock
3. Change kali_max_gdg_global to a qty that makes sense (min 0.3 - max 0.5)
	- Jika kali_max_gdg_global <= 0.3 masih muncul barang utk di order, mobil HARUS dijadwalkan utk kirim (stock di Smaller_Branch terlalu sedikit)
	- Jika kali_max_gdg_global > 0.3 normal
	- Jika kali_max_gdg_global > 0.5 barang sudah cukup di cabang
		- Limit: Barang keluar di Smaller_Branch terlalu banyak sehingga kali_max_gdg_global 0.5 sudah tidak mencukupi, maka max 0.5 harus diubah #Limits
	- Fix: Show kubikasi (HPP as fallback) on Pergerakan Stock #Action #Develop
4. Buka Simpo
5. Masukkan Volume Mobil ke Pergerakan Stock
6. Masukkan List ID Produk ke Simpo
	- (Note: Untuk pemahaman, anjurkan anak baru untuk mencoba kali_max_gdg_global terlalu besar/kecil. Perhatikan rasio n qty SKU fast moving dan SKU slow moving)
7. Copy List ID Produk
### Execute
1. @Main_Office melakukan stock masuk stock keluar 
	1. Stock keluar: 
		1. Create invoice with HPP price to akun cabang
			- Note: Akun cabang supaya masuk di kategori cabang bukan sebagai Loss)
	2. Stock masuk: 
		1. Login ke cabang [^1] 
		2. Input di Spurcinv [^2]
2. Siap Pengiriman 
	- Same as [[#Half Loading Full Loading|Pengiriman]]

## Half Loading Full Loading
1. Half loading or Full loading workflow remains the same 
2. Kirim Nomor Invoice ke @Team_Sidoarjo [^3]
3. @Team_Sidoarjo siapkan barang ke pallet
4. Mobil sampai dan muat pallet yang sudah disiapkan
	1. Jika Vol mobil ≥ 95%, Siapkan 1 SJ untuk dikorbankan  
	   
		??? info "Tidak Muat" 
			Lihat [[Tidak Muat#Tidak Muat]]


# Week Stable
## Stock Balancing - Stable
- Lihat [[SOP#Stock Balancing|Stock Balancing]]
### Init
1. Create Balancing request after the first wave of printing
	- Note: Exact timing is condition-dependent and will be refined through trial and error #Investigate_Minor
### Execute
- Lihat [[SOP#Stock Balancing|Stock Balancing]]

## Pengiriman
- Lihat [[SOP#Half Loading Full Loading|Pengiriman]]

[^1]: [[Deliberation#Cabang Setting]]

[^2]: [[Deliberation#Stock Masuk]]

[^3]: [[Deliberation#Shipping SJ Printing]]

