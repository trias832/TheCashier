## TheCashier
Aplikasi ini digunakan untuk menghitung jumlahdan harga dari  pembelian suatu barang/jasa
## Fungsionalitas
- User dapat menginputkan jasa atau barang yang dibeli,menginputkan jumlah dan harga
- Aplikasi dapat menampilkan barang yang di beli dan menampilkan total dari harga barang/jasa tersebut

## How Does it works?
Ketika user nenginputkan data dan mengklik button, maka data tersebut akan diolah oleh class Item untuk selanjutnya dimasukaan ke class Calculator untuk dilakukan perhitungan total harga dari barang.


    public void addItem(Item item)
        {
            this.listItem.Add(item);
            this.total += item.getSubTotal();
        }

Pada code diatas menerapkan Single Reponsibility.
Dimana item dimasukan kedalam list dan menghitung harga total semua barangnya


    public double getSubTotal()
        {
            subtotal = price * quantity;
            return subtotal;
        }

''
Pada code diatas digunakan untuk menghitung sub total harga dari setiap barang
