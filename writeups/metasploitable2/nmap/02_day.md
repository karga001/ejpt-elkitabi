## METASPLOİTABLE2
İlk keşif sırasında dikkatimi çeken 21/tcp ftp portunun servis ve sürüm bilgilerini doğrulamak amacıyla Nmap’in -A parametresi kullanılarak detaylı bir tarama gerçekleştirdim hedef sistemde FTP servisinin açık olduğunu vsftpd 2.3.4 sürümünün çalıştığını tespit ettim.
Ayrıca servis üzerinde anonymous FTP erişiminin aktif olduğu dikkatimi çekti. 

# Tarama çıktısı:

<img width="549" height="344" alt="resim" src="https://github.com/user-attachments/assets/89263fd2-f797-4cb8-beb1-1a313d24d478" />

Bu bulguyu hem servis sürümünün eski olması hem de yetkisiz erişime izin verilmesi nedeniyle kritik bir güvenlik riski olarak değerlendirdim.
