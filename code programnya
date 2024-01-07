class Kuliner:
    def __init__(self, jenis, makanan, jumlah, harga, total):
        self.jenis = jenis
        self.makanan = makanan
        self.jumlah = jumlah
        self.harga = harga
        self.total = total
    
    def info(self):
        print("1. Restoran")
        print("2. Street Food")
    
    def hitung_biaya(self):
        self.total = self.harga * self.jumlah
        return self.total

class Restoran(Kuliner):
    def __init__(self, jenis, rating):
        super().__init__(jenis, 0, 0, 0, 0)         
        self.rating = rating

    def info(self):
        super().info()
        print("\t========= MENU MAKANAN =========")
        print("")
        print("\t1. Sushi \t\t Rp.115.000")
        print("\t2. Spageti Carbonara \t Rp.200.000")
        print("\t3. Kebab Turki \t\t Rp.220.000")
        print("\t4. Baked Salmon \t Rp.135.000")
        print("\t5. Chicken Teriyaki \t Rp.150.000")
        print("")
        print("\tRating: ", self.rating)
        print("\t========= MENU MAKANAN =========")
        print("")
        
class StreetFood(Kuliner):
    def __init__(self, jenis, lokasi):
        super().__init__(jenis, 0, 0, 0, 0)
        self.lokasi = lokasi
    
    def info(self):
        super().info()
        print("\t========= MENU MAKANAN =========")
        print("")
        print("\t1. Corndog \t Rp.15.000")   
        print("\t2. Kerak Telor \t Rp.20.000")
        print("\t3. Kebab Turki \t Rp.22.000")
        print("\t4. Crepes \t Rp.15.000")
        print("\t5. Bakso Pluto \t Rp.15.000")
        print("")
        print("\tLokasi: ", self.lokasi)
        print("\t========= MENU MAKANAN =========")
        print("")

print("1. Restoran")
print("2. Street Food")
while True:
    call = input("Masukkan pilihan Anda (1/2): ")
    if call == "1":
        restoran = Restoran("Restoran", "9/10")
        restoran.info()
        
        restoran.makanan = int(input("Masukkan Pilihan makanan: "))
        restoran.jumlah = int(input("Masukkan jumlah porsi: "))
        restoran.harga = int(input("Masukkan harga per porsi: "))
        total_biaya = restoran.hitung_biaya()
        print("Total harga yang harus dibayar : ", total_biaya)
        lanjut = (input("Jika ingin lanjut memesan ketik y jika tidak t : "))
        if lanjut == 't':
            break
    elif call == "2":
        streetfood = StreetFood("Street Food", "UTY kampus 1")
        streetfood.info()
        streetfood.makanan = int(input("Masukkan Pilihan makanan: "))
        streetfood.jumlah = int(input("Masukkan jumlah porsi: "))
        streetfood.harga = int(input("Masukkan harga per porsi: "))
        total_biaya = streetfood.hitung_biaya()
        print(f"Total biaya: Rp {total_biaya}")
        lanjut = (input("Jika ingin lanjut memesan ketik y jika tidak t : "))
        if lanjut == 't':
            break
    else:
        print("Pilihan tidak valid")
