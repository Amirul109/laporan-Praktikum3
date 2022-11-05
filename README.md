# laporan-Praktikum3
# Nama  : Amirul Mu'minin 
# Kelas : Ti.21.C2 
# Nim   : 312110109

# Tugas 1 menggunakan method setter dan getter
sours pscoudenya =

class Mahasiswa{
    private String nama;
    private int nim;

  // penggunaan method getter
    public String getNama(){
        return this.nama;
    }
    public String getNim(){
        return this.nim;
    }
 // penggunaan  method setter
    public void setNama(String nama){
        this.nama= nama;
    }
    public void setNim(int nim){
        this.nim= nim;
    
// membuat objek dari class Mahasiswa
Mahasiswa Amir = new Mahasiswa();

//menggunakan method setter
Amir.setNama("Amir");
Amir.setNim("32110109");
//menggunakan method getter
System.out.printlin("Nama: " + Amir.getNam());
System.out.printlin("Nim: " + Amir.setNim());
    }
}

# Tugas 2 Mengimplementasikan java 

#pegawai
public class Pegawai {
  private String nama;
  private double gajiPokok;

  public void setNama(String nama) {
    this.nama = nama;
  }

  public String getNama() {
    return this.nama;
  }

  public void setGajiPokok(double gajiPokok) {
    this.gajiPokok = gajiPokok;
  }

  public double getGajiPokok() {
    return this.gajiPokok;
  }

  public void cetakInfo() {
    System.out.println("NAMA\t\t: " + this.getNama());
    System.out.println("GAJI POKOK\t: " + this.getGajiPokok());

  }
}


#pegawaiBeraksi
public class PegawaiBeraksi {
  public static void main(String[] args) {
    // Membuat Object
    Manager indri = new Manager();
    Programmer yanto = new Programmer();

    /* Memberi attribute dan memberi nilai */
    indri.setNama("Indri lestari");
    indri.setGajiPokok(5500000);
    indri.setTunjangan(5000000);

    yanto.setNama("Yanto suyatno");
    yanto.setGajiPokok(5500000);
    yanto.setBonus(550000);

    /* Mengakses Method */
    indri.cetakInfo();
    System.out.println();
    yanto.cetakInfo();
  }
}

![Screenshot (41)](https://user-images.githubusercontent.com/116171779/200093147-a566843c-b635-4e2b-9191-c2150c559b12.png)

source pascoudenya =

public class Programmer extends Pegawai {
  private double bonus;

  public void setBonus(double bonus) {
    this.bonus = bonus;
  }

  public double getBonus() {
    return this.bonus;
  }

  public void cetakInfo() {
    super.cetakInfo();
    System.out.println("BONUS\t\t: " + this.getBonus());
  }
}
hasil Outputnya :
![Screenshot (40)](https://user-images.githubusercontent.com/116171779/200092935-ff41ea31-db60-493d-b6af-3c32dfc633b0.png)
