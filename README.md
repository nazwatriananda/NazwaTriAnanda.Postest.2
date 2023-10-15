print("Nama: Nazwa Tri Ananda")
print("NIM: 2309116018")
print("Kelas: Sistem Informasi A")
print("=====================================")

print("WELCOME TO KPOP STORE!")
print("Silahkan Login Sebagai: ")
print("1. Admin Toko")
print("2. Pelanggan")
print("=====================================")
Login_Menu = input('pilih Login Sebagai (1/2): ') 
print("=====================================")

if Login_Menu == '1':
    print("Hallo Admin!")
    print(input("Masukkan Password: "))
    print("Silahkan Pilih Menu Bantuan")

    print("=====================================")
    print("1. Menambahkan Barang pada List")
    print("2. Check List Barang")
    print("3. Mengubah Harga Barang")
    print("4. Menghapus Barang dari List")
    print("=====================================")

    Menu_Admin = input("Pilih Menu Yang Dibutuhkan(1/2/3/4): ")

    if Menu_Admin == "1" :
        Barang = ["Album Enhypen Manifesto Day 1 Reguler", "Album NCT DREAM Hello Future", "Album NCT DREAM Hot Sauce", "Album Seventeen Heng:garae", "Album NewJeans 2nd Ep - Get Up", "Lightstick Enhypen", "Lightstick NCT", "Lightstick WayV", "Lightstick Aespa", "Lightstick Seventeen ver. 3"]
        print(f"Barang Sebelum ditambahkan {Barang}")
        print("===========================")
        Barang.append("PhotoCard")
        print(f"Barang Setelah ditambahkan {Barang}")
    elif Menu_Admin == "2" :
        from prettytable import PrettyTable
        Barang = PrettyTable()
        Barang.field_names = ["Nomor", "Nama Barang", "Harga Barang"]
        Barang.add_row(["1.","Album Enhypen Manifesto Day 1 Reguler", "Rp 186.000"])
        Barang.add_row(["2.","Album NCT DREAM Hello Future", "Rp 275.000"])
        Barang.add_row(["3.","Album NCT DREAM Hot Sauce", "Rp 335.000"])
        Barang.add_row(["4.","Album Seventeen Heng:garae", "Rp 315.000"])
        Barang.add_row(["5.", "Album NewJeans 2nd Ep - Get Up", "Rp 450.000"])
        Barang.add_row(["6.","Lightstick Enhypen", "Rp 652.000"])
        Barang.add_row(["7.","Lightstick NewJeans", "Rp 745.000"])
        Barang.add_row(["8.","Lightstick NCT", "Rp 760.000"])
        Barang.add_row(["9.","Lightstick WayV", "Rp 770.000"])
        Barang.add_row(["10.","Lightstick Aespa", "Rp 779.000"])
        Barang.add_row(["11.","Lightstick Seventeen ver. 3", "Rp 795.000"])
        Barang.add_row(["12.","PhotoCard", "Rp 50.000"])
        print(Barang)
    elif Menu_Admin == "3" :
        Harga = ["Rp 186.000", "Rp 275.000", "Rp 335.000", "Rp 315.000", "Rp 400.000", "Rp 450. 000", "Rp 652.000", "Rp 652.000", "Rp 745.000", "Rp 760.000", "Rp 760.000", "Rp 770.000", "Rp 779.000", "Rp 795.000", "Rp 50.000"]
        print(f"Harga Barang Awal: {Harga}")
        print("===========================")
        Harga[0] = "Rp 175.000"
        print(f"Harga Barang Berhasil di Ubah: {Harga}")
    elif Menu_Admin == "4" :
        Barang = ["Album Enhypen Manifesto Day 1 Reguler", "Album NCT DREAM Hello Future", "Album NCT DREAM Hot Sauce", "Album Seventeen Heng:garae", "Album NewJeans 2nd Ep - Get Up", "Lightstick Enhypen", "Lightstick NewJeans", "Lightstick NCT",  "Lightstick WayV", "Lightstick Aespa", "Lightstick Seventeen ver. 3", "PhotoCard"]
        print(f"Barang Sebelum dihapus {Barang}")
        print("===========================")
        del Barang[4]
        print(f"Barang Setelah dihapus {Barang}")

elif Login_Menu == '2':
    print("Selamat Datang Di Toko Kami!")
    
    from prettytable import PrettyTable
    Barang = PrettyTable()
    Barang.field_names = ["Nomor", "Nama Barang", "Harga Barang"]
    Barang.add_row(["1.","Album Enhypen Manifesto Day 1 Reguler", "Rp 175.000"])
    Barang.add_row(["2.","Album NCT DREAM Hello Future", "Rp 275.000"])
    Barang.add_row(["3.","Album NCT DREAM Hot Sauce", "Rp 335.000"])
    Barang.add_row(["4.","Album Seventeen Heng:garae", "Rp 315.000"])
    Barang.add_row(["5.","Lightstick Enhypen", "Rp 652.000"])
    Barang.add_row(["6.","Lightstick NewJeans", "Rp 745.000"])
    Barang.add_row(["7.","Lightstick NCT", "Rp 760.000"])
    Barang.add_row(["8.","Lightstick WayV", "Rp 770.000"])
    Barang.add_row(["9.","Lightstick Aespa", "Rp 779.000"])
    Barang.add_row(["10.","Lightstick Seventeen ver. 3", "Rp 795.000"])
    Barang.add_row(["11.","PhotoCard", "Rp 50.000"])
    print(Barang)
    
    Barang = (input("Masukkan nomor Barang yang ingin Dibeli (1/2/3/4/5/6/7/8/9/10/11): "))

    if Barang == "1":
        Jumlah_Barang = int(input("Anda Ingin Membeli Album Enhypen Manifesto Day 1 Reguler sebanyak: "))
        Total = 175000 * Jumlah_Barang   
        print("Total Belanjaan Anda sebesar: ")                      
        print(Total)
        print("Terimakasih Telah Berbelanja di Toko Kami")
    elif Barang == "2":
        Jumlah_Barang = int(input("Anda Ingin Membeli Album NCT DREAM Hello Future sebanyak: "))
        Total = 275000 * Jumlah_Barang
        print("Total Belanjaan Anda sebesar: ")                         
        print(Total)
        print("Terimakasih Telah Berbelanja di Toko Kami")
    elif Barang == "3":
        Jumlah_Barang = int(input("Anda Ingin Membeli Album NCT DREAM Hot Sauce sebanyak: "))
        Total = 335000 * Jumlah_Barang   
        print("Total Belanjaan Anda sebesar: ")                      
        print(Total)
        print("Terimakasih Telah Berbelanja di Toko Kami")
    elif Barang == "4":
        Jumlah_Barang = int(input("Anda Ingin Membeli Album Seventeen Heng:garae sebanyak: "))
        Total = 315000 * Jumlah_Barang   
        print("Total Belanjaan Anda sebesar: ")                      
        print(Total)
        print("Terimakasih Telah Berbelanja di Toko Kami")
    elif Barang == "5":
        Jumlah_Barang = int(input("Anda Ingin Membeli Lightstick Enhypen sebanyak: "))
        Total = 652000 * Jumlah_Barang   
        print("Total Belanjaan Anda sebesar: ")                      
        print(Total)
        print("Terimakasih Telah Berbelanja di Toko Kami")
    elif Barang == "6":
        Jumlah_Barang = int(input("Anda Ingin Membeli Lightstick NewJeans sebanyak: "))
        Total = 745000 * Jumlah_Barang     
        print("Total Belanjaan Anda sebesar: ")                    
        print(Total)
        print("Terimakasih Telah Berbelanja di Toko Kami")
    elif Barang == "7":
        Jumlah_Barang = int(input("Anda Ingin Membeli Lightstick NCT sebanyak: "))
        Total = 760000 * Jumlah_Barang     
        print("Total Belanjaan Anda sebesar: ")                    
        print(Total)
        print("Terimakasih Telah Berbelanja di Toko Kami")
    elif Barang == "8":
        Jumlah_Barang = int(input("Anda Ingin Membeli Lightstick WayV sebanyak: "))
        Total = 770000 * Jumlah_Barang      
        print("Total Belanjaan Anda sebesar: ")                   
        print(Total)
        print("Terimakasih Telah Berbelanja di Toko Kami")
    elif Barang == "9":
        Jumlah_Barang = int(input("Anda Ingin Membeli Lightstick Aespa sebanyak: "))
        Total = 779000 * Jumlah_Barang        
        print("Total Belanjaan Anda sebesar: ")                 
        print(Total)
        print("Terimakasih Telah Berbelanja di Toko Kami")
    elif Barang == "10":
        Jumlah_Barang = int(input("Anda Ingin Membeli Lightstick Seventeen ver. 3 sebanyak: "))
        Total = 795000 * Jumlah_Barang   
        print("Total Belanjaan Anda sebesar: ")                      
        print(Total)
        print("Terimakasih Telah Berbelanja di Toko Kami")
    elif Barang == "11":
        Jumlah_Barang = int(input("Anda Ingin Membeli PhotoCard sebanyak: "))
        Total = 50000 * Jumlah_Barang        
        print("Total Belanjaan Anda sebesar: ")                 
        print(Total)
        print("Terimakasih Telah Berbelanja di Toko Kami")
else:
    print("Data Tidak Valid")
