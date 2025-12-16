## Erişim sağlanması

Keşif aşamasında FTP servisinin vsftpd 2.3.4 sürümünü kullandığını tespit ettikten sonra bu sürümün bilinen bir güvenlik açığı ile ilişkili olduğunu değerlendirdim.

Servis ve sürüm bilgisini doğruladıktan sonra zafiyeti değerlendirmeye karar verdim.

Bu aşamada exploit geliştirmek yerine, servis-zafiyet eşlemesini daha izlenebilir bir biçimde test edebilmek için Metasploit-Framework kullanmayı tercih ettim.

Metasploit, ilgili exploit modülünü ve payload sürecini entegre olarak sunduğu için test sürecini daha kontrollü yürütmemi sağladı.

Gerçekleştirdiğim test sonucunda hedef sistemde yetkisiz komut çalıştırma elde ettim ve erişim seviyesinde root yetkisi olduğunu doğruladım .

<img width="1574" height="792" alt="resim" src="https://github.com/user-attachments/assets/219fccae-bd46-4a17-8c4e-b54bf1f0aaa0" />

Bu test FTP servisinin güncel olmayan bir sürümle ve zayıf yapılandırma ile çalıştırılmasının tam sistem ele geçirilmesine kadar gidebilecek ciddi sonuçlar doğurabildiğini net şekilde gösterdi.
