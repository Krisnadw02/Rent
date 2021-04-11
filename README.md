# Rent
compilasi code
#data mobil

mobilkecil=("ayla","brio","agya")
mobilsedan=("camry","vios","city")
mobilminibus=("avanza","xenia","apv")

print (mobilkecil)
print (mobilsedan)
print (mobilminibus)

def menu ():
    print (" Selamat Datang")
    print ("menu sewa")
    print ("1. mobil kecil")
    print ("2. mobil sedan")
    print ("3. mobil minibus")
    print ("4. pencarian")
    print ("5. keluar")
    
username = "admin"
password = "admin"

username_input=input("masukan username  ")
password_input=input("masukan password  ")

if (username_input == username and password_input == password):
    menu ()
else:
    username_input=input("masukan username  ")
    password_input=input("masukan password  ")
    while "admin" not in username_input and password_input:
        username_input=input("masukan username  ")
        password_input=input("masukan password  ")
        if("admin" in username_input and password_input):
            break
#jarak tab harus di perhatikan karna sering kali kita gabisa dappet output kalo tabnya terlalu jauh
def menu2 ():
    print ("Unit Tersedia")
    print (mobilkecil)
def menu3 ():
    print ("Unit Tersedia")
    print (mobilsedan) 
def menu4 ():
    print ("Unit Tersedia")
    print (mobilminibus)

menu_input=input("masukan unit:  ")
if menu_input=="1":
    menu2 ()
    print ("Harga per jam 25000")
    x=int(input("Lama Sewa  "))
print ("Harga Sewa  ",x*25000)
if menu_input=="2":
    menu3 ()
    print ("Harga per jam 30000")
    y=int(input("Lama Sewa  "))
    print ("Harga Sewa  ",(y)*30000)
if menu_input=="3":
    menu4 ()
    print ("Harga per jam 35000")
    b=int(input("Lama Sewa  "))
    print ("Harga Sewa  ",b*35000)

ulang = input("Apakah anda akan mengulang sewa ?  ")
if ulang == "Yes" or "No":
        menu ();
    else;
        exit()
    
