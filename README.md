## Modifikasi
1. Mengganti warna background menjadi warna abu-abu yang deklarasinya dengan kode rgb.

   `setBackground(new Color(181, 181, 181));`
3. Mengganti warna walls dengan deklarasi kode rgb.

   `g.setColor(new Color(255, 255, 255));`
5. Mengganti foods menjadi icon tacoFood pixel.
   
    a) Menambahkan variabel dengan nama tacoFood

   	`private Image tacoFoodImage;`
   
    b)	Memuat gambar tacoFood

   `tacoFoodImage = new ImageIcon(getClass().getResource("./tacoFood.png")).getImage();`
   
    c)	Mengganti gambar dalam program

   `Block food = new Block(tacoFoodImage, x + 10, y + 10, 14, 14);`

7. Menambahkan panel score dan lives (nyawa) yang lebih jelas.

   Untuk menambahkan panel di atas board game yaitu dengan menambahkan deklarasi berikut ke dalam constructor PacMan()
	```
   	setLayout(new BorderLayout());
    JLabel scoreLabel = new JLabel("Score: 0   Lives: 3", SwingConstants.CENTER);
    scoreLabel.setFont(new Font("Arial", Font.BOLD, 20));
    scoreLabel.setForeground(Color.WHITE);
    scoreLabel.setBackground(Color.GRAY);
    scoreLabel.setOpaque(true); // Biar warna backgroundnya kelihatan
    add(scoreLabel, BorderLayout.NORTH);
 	```

### Output setelah modifikasi
![image](https://github.com/user-attachments/assets/951a4ea2-fa8b-4894-be0c-142de7ce8283)

