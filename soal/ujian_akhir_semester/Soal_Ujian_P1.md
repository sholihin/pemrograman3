## Soal Ujian Pemograman 1 ##

### Waktu Pengerjaan : ###
- 60 menit

### Sifat : ###

- Open Book
- Open PC/Laptop

### Soal ###

1. Buatlah program perpustakaan dengan 3 (tiga) buah judul buku dibawah ini !
	
	- Matematika
	- B. Indonesia
	- B. Inggris
	
2. Jika kita membuat program dengan `SourceCode` dibawah ini maka output apakah yang akan dihasilkan ? key : value is 6
	
``` java
public class Person {
	public static void main(String[] args){
		int a=4,b=6;
		int num=a|b;
		if(num==4)
			System.out.println("value is 4");

		else if(num==5)
			System.out.println("value is 5");

		else if(num==6)
			System.out.println("value is 6");

		else if(num==7)
			System.out.println("value is 7");
		}
}
```

3. Lengkapilah kekurangan pada `SourceCode` dibawah ini !

``` java
public class MahasiswaMain {

	1. .......................................... key : public static void main (String[] args) {
		File file = new File ("Mahasiswa.txt");
		FileInputStream fis = null;
		BufferedInputStream bis = null;
		DataInputStream dis = null;
		
		List<Mahasiswa> listMahasiswa = new ArrayList <Mahasiswa>();
			2. .......................................... key : try {
				fis = new FileInputStream(file);
				bis = new BufferedInputStream(fis);
				dis = new DataInputStream(bis);
					while (dis.available() !=0) {
						String line = dis.readLine ();
						String[] data = line.split(",");

						Mahasiswa m = new Mahasiswa ();
						m.setNpm (data[0]);
						m.setNama (data[1]);
						m.setAlamat (data[2]);
							listMahasiswa.add(m);
						}
				}
				
				
			3. .......................................... key : catch (IOException ex){
				System.out.println("File " + file.getName () + "tidak  ketemu !");
				System.out.println ("Exception : " + ex.getMessage());
			}
				
				for (Mahasiswa mhs : listMahasiswa) {
					System.out.println("==================================================");

						System.out.println ("NPM : " + mhs.getNpm ());
						System.out.println ("Nama : " + mhs.getNama ());
						System.out.println ("Alamat : " + mhs.getAlamat ());
				}
		}
}
```

4. Buatlah program pertambahan yang akan menampilkan output seperti dibawah ini!

a = 1000
b = 1000
a + b = 2000

key : 

``` java
public class Data {
	public static void main (String[] args) {
		int a;
		a = 1000;
		int b = 1000;

		System.out.println("a = " + a);
		System.out.println("b = " + b);
		System.out.println("a + b = " + (a + b));
	}
}
```

5. Pada soal nomor 3 ada beberapa library yang perlu diimport sebutkanlah satu-persatu dan jelaskan fungsinya !

key : 

``` java
import java.io.BufferedInputStream;
import java.io.DataInputStream;
import java.io.File;
import java.io.FileInputStream;
import java.io.IOException;
import java.util.ArrayList;
import java.util.List;
```
