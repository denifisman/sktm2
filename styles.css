function generateSurat() {
    var namaAnak = document.getElementById("namaAnak").value;
    var namaAyah = document.getElementById("namaAyah").value;
    var tempatTanggalLahirAyah = document.getElementById("tempatTanggalLahirAyah").value;
    var jenisKelaminAyah = document.getElementById("jenisKelaminAyah").value;
    var agamaAyah = document.getElementById("agamaAyah").value;
    var pekerjaanAyah = document.getElementById("pekerjaanAyah").value;

    var namaIbu = document.getElementById("namaIbu").value;
    var tempatTanggalLahirIbu = document.getElementById("tempatTanggalLahirIbu").value;
    var jenisKelaminIbu = document.getElementById("jenisKelaminIbu").value;
    var agamaIbu = document.getElementById("agamaIbu").value;
    var pekerjaanIbu = document.getElementById("pekerjaanIbu").value;

    // Update surat with values from the form
    document.getElementById("namaAnakSurat").innerText = namaAnak;
    document.getElementById("namaAyahSurat").innerText = namaAyah;
    document.getElementById("tempatTanggalLahirAyahSurat").innerText = tempatTanggalLahirAyah;
    document.getElementById("jenisKelaminAyahSurat").innerText = jenisKelaminAyah;
    document.getElementById("agamaAyahSurat").innerText = agamaAyah;
    document.getElementById("pekerjaanAyahSurat").innerText = pekerjaanAyah;

    document.getElementById("namaIbuSurat").innerText = namaIbu;
    document.getElementById("tempatTanggalLahirIbuSurat").innerText = tempatTanggalLahirIbu;
    document.getElementById("jenisKelaminIbuSurat").innerText = jenisKelaminIbu;
    document.getElementById("agamaIbuSurat").innerText = agamaIbu;
    document.getElementById("pekerjaanIbuSurat").innerText = pekerjaanIbu;

    // Update date
    var today = new Date();
    var date = today.getDate() + '-' + (today.getMonth() + 1) + '-' + today.getFullYear();
    document.getElementById("tanggalSurat").innerText = date;

    // Hide the form and show the surat
    document.getElementById("form").style.display = "none";
    document.getElementById("surat").style.display = "block";
}

function printSurat() {
    window.print();
}

function generatePDF() {
    const { jsPDF } = window.jspdf;

    var doc = new jsPDF();

    // Add logo
    const img = new Image();
    img.src = 'logo.png';
    img.onload = function() {
        doc.addImage(img, 'PNG', 10, 10, 30, 30);
        doc.setFontSize(16);
        doc.text("PEMERINTAH KABUPATEN BANGGAI KEPULAUAN", 50, 20);
        doc.setFontSize(14);
        doc.text("KECAMATAN LIANG DESA MAMULUSAN", 50, 30);
        doc.setFontSize(12);
        doc.text("A OBULUSAN NO 66 MAMULUSAN KODE POS 94783", 50, 40);
        doc.setLineWidth(1.0);
        doc.line(10, 60, 200, 60);
        doc.setFontSize(14);
        doc.text("SURAT KETERANGAN TIDAK MAMPU", 105, 70, null, null, 'center');
        doc.setFontSize(12);
        doc.text("Nomor: 140/354/PEMDES-MLS/IV/2022", 10, 80);
        doc.text("Yang bertanda tangan di bawah ini:", 10, 90);
        doc.text("Nama: LISNAWATI TABUPOK, S.Pd.K", 10, 100);
        doc.text("Jabatan: Kepala Desa", 10, 110);
        doc.text("Alamat: Desa Mamulusan, Kecamatan Liang, Kabupaten Banggai Kepulauan.", 10, 120);
        doc.text("Menerangkan dengan sebenarnya bahwa :", 10, 130);
        doc.text(`Nama Ayah: ${document.getElementById("namaAyahSurat").innerText}`, 10, 140);
        doc.text(`Tempat/Tanggal Lahir Ayah: ${document.getElementById("tempatTanggalLahirAyahSurat").innerText}`, 10, 150);
        doc.text(`Jenis Kelamin Ayah: ${document.getElementById("jenisKelaminAyahSurat").innerText}`, 10, 160);
        doc.text(`Agama Ayah: ${document.getElementById("agamaAyahSurat").innerText}`, 10, 170);
        doc.text(`Pekerjaan Ayah: ${document.getElementById("pekerjaanAyahSurat").innerText}`, 10, 180);
        doc.text(`Alamat Ayah: Desa Mamulusan, Kecamatan Liang, Kabupaten Banggai Kepulauan.`, 10, 190);
        doc.text(`Nama Ibu: ${document.getElementById("namaIbuSurat").innerText}`, 10, 200);
        doc.text(`Tempat/Tanggal Lahir Ibu: ${document.getElementById("tempatTanggalLahirIbuSurat").innerText}`, 10, 210);
        doc.text(`Jenis Kelamin Ibu: ${document.getElementById("jenisKelaminIbuSurat").innerText}`, 10, 220);
        doc.text(`Agama Ibu: ${document.getElementById("agamaIbuSurat").innerText}`, 10, 230);
        doc.text(`Pekerjaan Ibu: ${document.getElementById("pekerjaanIbuSurat").innerText}`, 10, 240);
        doc.text(`Alamat Ibu: Desa Mamulusan, Kecamatan Liang, Kabupaten Banggai Kepulauan.`, 10, 250);
        doc.text(`Bahwa yang bersangkutan tersebut diatas adalah benar orang tua dari ${document.getElementById("namaAnakSurat").innerText} yang Berpenghasilan Rendah (Ekonomi Lemah).`, 10, 260);
        doc.text("Demikian surat keterangan ini, dibuat dengan benar diberikan kepada yang bersangkutan, untuk dipergunakan dimana perlunya.", 10, 270);
        doc.text("Mengetahui", 10, 290);
        doc.text("CAMAT LIANG", 10, 300);
        doc.text("IRENODRATA ONENG, SH", 10, 310);
        doc.text("NIP. 19730817 200604 1 027", 10, 320);
        doc.text(`Mamulusan, ${document.getElementById("tanggalSurat").innerText}`, 10, 340);
        doc.text("KEPALA DESA MAMULUSAN", 10, 350);
        doc.text("LISNAWATI TABUPOK, S.Pd.K", 10, 380);

        doc.save("Surat_Keterangan_Tidak_Mampu.pdf");
    };
}
