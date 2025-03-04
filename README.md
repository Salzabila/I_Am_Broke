child: Column(
                crossAxisAlignment: CrossAxisAlignment.start, // Menyusun teks ke kiri
                children: const [
                  // Fakta humor tentang mahasiswa bokek
                  Text("💸 Saldo: Rp 0,00", style: TextStyle(fontSize: 18, fontWeight: FontWeight.bold)),
                  SizedBox(height: 8), // Spasi antara teks
                  Text("🍜 Makan Indomie tiap hari"),
                  Text("🏃‍♂ Menghindari ajakan nongkrong"),
                  Text("📅 Menunggu tanggal gajian seperti Lebaran"),
                ],
              ),
            ),

            const SizedBox(height: 20), // Spasi sebelum tombol

            // Tombol "Cek Saldo"
            ElevatedButton(
              onPressed: cekSaldo, // Memanggil fungsi cekSaldo saat ditekan
              style: ElevatedButton.styleFrom(
                backgroundColor: Colors.redAccent, // Warna tombol
                padding: const EdgeInsets.symmetric(horizontal: 20, vertical: 12), // Ukuran tombol
                textStyle: const TextStyle(fontSize: 16), // Ukuran teks pada tombol
              ),
              child: const Text("Cek Saldo"), // Label tombol
            ),

            const SizedBox(height: 10), // Spasi sebelum teks saldo
            // Menampilkan teks saldo yang bisa berubah
            Text(
              saldoText, // Menampilkan saldo terkini
              textAlign: TextAlign.center, // Menjadikan teks rata tengah
              style: const TextStyle(fontSize: 16, fontWeight: FontWeight.bold, color: Colors.redAccent), // Gaya teks saldo
            ),
          ],
        ),
      ),
    );
  }
}
