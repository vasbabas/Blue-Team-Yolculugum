# Mavi Takım (Blue Team) Yolculuğu 🛡️

## Merhaba! 👋

Ben Muzaffer, Bilgisayar Programcılığı öğrencisiyim ve siber güvenlik dünyasına tutkuyla bağlıyım. 👨‍💻 Bu alana olan ilgim bir süredir devam etse de, öğrenme sürecimde daha yapılandırılmış ve disiplinli bir yaklaşıma ihtiyaç duyduğumu fark ettim.

## Bu Depo (Repository) Nedir? 🗺️

Bu depo, benim siber güvenlik serüvenimin canlı bir bir günlüğüdür. İnternette yaptığım detaylı araştırmalar sonucunda, "Daarin" tarafından Medium'da hazırlanan kapsamlı **[Blue Team Yol Haritası](https://medium.com/@daarin/roadmap-for-cyber-security-in-the-blue-team-ae9b25721ac2)** ile karşılaştım. Bu yol haritasının detay seviyesi ve mantıksal yapısı, kendimi geliştirmek için izlemek istediğim yolun tam olarak bu olduğuna karar vermemi sağladı. ✅

Bu GitHub deposunda, o yol haritasını takip ederken öğrendiğim her şeyi, karşılaştığım zorlukları 😱, bulduğum çözümleri 💡 ve kişisel notlarımı günlük olarak belgeleyeceğim. Amacım, hem kendi gelişimimi takip etmek hem de benim gibi bu yola baş koyan diğer insanlara bir kaynak ve rehber oluşturmaktır.

## Hedeflerim 🎯

Yol haritası oldukça uzun ve kapsamlı. Öncelikli hedefim, sağlam bir **IT (Bilgi Teknolojileri) temeli** oluşturmak. Meslek lisesi ve üniversitede aldığım bilgisayar eğitimleri sayesinde bazı temel konulara aşinayım, bu yüzden bu kısımları daha hızlı geçebilirim. Ancak bu deponun bir rehber niteliği taşımasını istediğim için, bildiğim konuları dahi atlamadan gerekli tüm bilgileri ve pratikleri ekleyeceğim. ✍️

IT temellerini sağlamlaştırdıktan sonra nihai hedefim, siber güvenlik alanına, özellikle **Mavi Takım (Blue Team)** rollerine geçiş yapmaktır.

## Kullandığım Araçlar ve Metodoloji 🛠️

Bu öğrenme sürecinde verimliliği artırmak adına modern araçlardan faydalanacağım. Özellikle karmaşık konuları araştırmak, ek bilgi edinmek ve farklı bakış açıları kazanmak için yapay zeka araçlarını 🤖 aktif olarak kullanacağım.

Bu yolculukta bana katılın! Her türlü geri bildirim, öneri ve tartışmaya açığım. 😊

---

## 📜 İçindekiler (Günlük Kayıtları)

Aşağıdaki listeden ilgili günün kaydına doğrudan atlayabilirsiniz.

- [🗓️ 4 Ağustos 2025: Laboratuvar Kurulumu ve İlk Domain Macerası](#gun-2025-08-04)
- [🗓️ 5 Ağustos 2025: Active Directory'nin Kalbine İniyoruz: OU, Kullanıcılar ve İzinler](#gun-2025-08-05)
- [🗓️ 6 Ağustos 2025: GPO ile İmparatorluğun Kurallarını Yazmak](#gun-2025-08-06)
- [🗓️ 7 Ağustos 2025: Windows Server'da Ustalığa Son Adım: DNS, DHCP ve Ötesi](#gun-2025-08-07)
- [🗓️ 11 Ağustos 2025: Linux Yönetimi, Script Temelleri ve Sistem Loglarıyla Yolculuk Devam Ediyor](#gun-2025-08-11)
- [🗓️ 12 Ağustos 2025: Networking Deep Dive – Ağların Derinliklerine Yolculuk!](#gun-2025-08-12)
- [🗓️ 14 Ağustos 2025: Wireshark ile Trafik Analizi – Protokollerin Derinliklerine Yolculuk!](#gun-2025-08-14)
- [🗓️ 18 Ağustos 2025: Database Fundamentals ve Güvenlik – Temel Bilgiler, Pratikler ve Siber Güvenlik Bağlantısı](#gun-2025-08-18)
- [🗓️ 19 Ağustos 2025: Sahne Arkasına Bakış: Güvenlik Operasyon Merkezi (SOC) Nasıl Çalışır?](#gun-2025-08-19)
- [🗓️ 20 Ağustos 2025: Zararlı Yazılım (Malware) Türleri Rehberi](#gun-2025-08-20)
- *(Yeni günlük eklendiğinde buraya bir satır daha eklenecek...)*
---
## 🚀 Günlükler Başlıyor!
<a id="gun-2025-08-04"></a>
## 🗓️ 4 Ağustos 2025
### Laboratuvar Kurulumu ve İlk Domain Macerası 🧪

**Bugünkü Konu:** Blue Team laboratuvar ortamının hazırlanması. 🧪

#### Günün Özeti

Bugün, teorik bilgileri pratiğe dökebileceğim sanal laboratuvar ortamımı hazırlamaya odaklandım. Microsoft Learn koleksiyonuna başlamadan önce, üzerinde çalışacağım sistemlerin hazır ve birbirleriyle iletişim kurabilir halde olması kritikti. Bu süreç, beklediğimden daha fazla sorun giderme pratiği içerdi ve harika bir öğrenme deneyimi oldu! 💪

#### Yapılan İşlemler ve Öğrenilenler 🤓

1.  **Sanallaştırma Platformu: VirtualBox** 📦
    Her şeyden önce, izole ve güvenli bir çalışma alanı oluşturmak için Oracle VirtualBox'ı kurdum. Sanallaştırma, tek bir fiziksel makine üzerinde birden çok işletim sistemini aynı anda çalıştırmamızı sağlar. Bu, farklı sistemlerin birbiriyle nasıl etkileşime girdiğini görmek ve hata yapmaktan korkmadan denemeler yapmak için mükemmel bir yöntem.

2.  **Sanal Makinelerin Kurulumu** 🖥️
    -   **Windows Server 2019:** Laboratuvarımın merkezi olacak olan sunucu. Domain Controller (Etki Alanı Yöneticisi), DNS ve diğer temel servisleri bu sunucu üzerinde yapılandıracağım.
    -   **Windows 10:** Sunucu tarafından yönetilecek olan standart bir istemci (client) makinesi. Yaptığım politika değişikliklerinin ve güvenlik ayarlarının etkilerini bu makine üzerinden gözlemleyeceğim.

3.  **Ağ Yapılandırması: En Kritik Adım!** 🌐
    Sanal makinelerin birbiriyle konuşabilmesi için doğru ağ yapılandırması şarttır. Her iki sanal makine için de ikişer ağ bağdaştırıcısı tanımladım:
    -   **Bağdaştırıcı 1: NAT (Network Address Translation):** Bu bağdaştırıcı, sanal makinelerin ana makinem üzerinden internete çıkabilmesini sağlar. Bu sayede gerekli güncellemeleri ve indirmeleri yapabilirim. 🌍
    -   **Bağdaştırıcı 2: Dahili Ağ (Internal Network):** Bu bağdaştırıcı, iki sanal makinenin dış dünyadan izole, kendi özel ağlarında haberleşmesi için kullanıldı. İkisine de aynı "intnet" ismini verdim. Bu, gerçek bir şirket içi ağı simüle etmemi sağlıyor. 🔒

4.  **Statik IP Adreslemesi ve DNS** ✍️
    -   **Windows Server 2016 IP Ayarları:**
        -   IP Adresi: `192.168.100.10`
        -   Alt Ağ Maskesi: `255.255.255.0`
        -   DNS Sunucusu: `192.168.100.10` (Kendisi)
        -   **Öğrenilen Bilgi 💡:** Bir Domain Controller, aynı zamanda DNS sunucusu olarak da hizmet verir. Bu yüzden DNS olarak kendi IP adresini göstermesi gerekir ki ağdaki diğer makineler domain'i ve diğer kaynakları ismiyle bulabilsin.
    -   **Windows 10 IP Ayarları:**
        -   IP Adresi: `192.168.100.20`
        -   Alt Ağ Maskesi: `255.255.255.0`
        -   DNS Sunucusu: `192.168.100.10` (Server'ın IP'si)
        -   **Öğrenilen Bilgi 💡:** İstemci makinenin domain'e katılabilmesi için DNS sunucusu olarak Domain Controller'ın IP adresini bilmesi zorunludur. Aksi takdirde, "contoso.local" gibi bir domain isminin hangi IP adresine karşılık geldiğini çözemez.

#### Karşılaşılan Sorun ve Çözüm: "AD DC Could Not Be Contacted" 🤯
Her şey hazır gibiydi. Windows 10 makinesini `CLIENT01` olarak yeniden adlandırdım ve domain'e dahil etmeye çalıştığımda o meşhur hatayı aldım: **"An Active Directory Domain Controller for the domain could not be contacted."**

Ping testinde Windows 10'dan sunucuya ping gidebiliyorken, sunucudan Windows 10'a ping gitmemesi ilk ipucuydu. Kısa bir araştırma ve yapay zekaya danışma sonucunda suçlunun **Windows Güvenlik Duvarı (Firewall)** 🔥 olduğunu anladım.

**Çözüm (Geçici) ✅:** Sorunu hızlıca aşmak için Windows Server üzerindeki güvenlik duvarını geçici olarak tamamen kapattım. Ve BINGO! 🎉 Windows 10 makinesi sorunsuz bir şekilde domain'e katıldı.

**Profesyonel İpucu ve Gelecek Notu 📝:** Gerçek bir ortamda güvenlik duvarını tamamen kapatmak **asla** yapılmaması gereken bir şeydir. Doğru yöntem, domain'e katılım için gerekli olan spesifik portlara (DNS, RPC, SMB vb.) güvenlik duvarı üzerinden izin vermektir. Bu konuyu ilerleyen günlerde detaylıca araştırıp doğru kural setini oluşturacağım.

#### Günün Sonucu ve Sonraki Adımlar 🏁
Laboratuvarım artık hazır! Bu temel kurulum, yol haritamdaki pratik uygulamalar için sağlam bir zemin oluşturdu. Artık gönül rahatlığıyla başlayabilirim!

Herkese bol çalışmalar, sağlıklı günler diliyorum  esenlikle kalın ! 🌟

---
<a id="gun-2025-08-05"></a>
## 🗓️ 5 Ağustos 2025
### Active Directory'nin Kalbine İniyoruz: OU, Kullanıcılar ve İzinler 💙

**Bugünkü Konu:** Active Directory'nin kalbine yolculuk ve ilk pratik uygulamalar. 💙

#### Günün Özeti
Bugün, dün kurduğum laboratuvarı daha işlevsel hale getirmekle başladım ve ardından Active Directory'nin temel yapı taşlarını hem teoride hem de pratikte öğrenmeye odaklandım. Sunucu güncellemelerinin ne kadar sabır gerektirdiğini bir kez daha anladıktan sonra, bir şirketin dijital iskeletini oluşturan OU, kullanıcı ve grup yönetiminin ne kadar keyifli olduğunu gördüm. Emeklerimin karşılığını almak harikaydı! 💪

#### Hazırlık Aşaması 🛠️
Pratiğe geçmeden önce birkaç temel adımı tamamladım:
1.  **VirtualBox Guest Additions Kurulumu:** Hem sunucu hem de istemci makinesine bu eklentileri kurdum.
    - **💡 Neden Önemli?** Bu eklentiler, sanal makine ile ana makine arasında daha iyi entegrasyon sağlar. Ekran çözünürlüğünü otomatik ayarlar, fare geçişlerini pürüzsüzleştirir ve en önemlisi, kopyala-yapıştır gibi özellikleri aktif hale getirir. Kısacası, hayat kurtarır!
2.  **Windows Server Güncellemeleri:** Sunucumun güncel olmadığını fark ettim ve tüm güncellemeleri yükledim. Bu işlem biraz uzun sürse de, siber güvenlikte ilk kural şudur: **Sistemlerini her zaman güncel tut!** Patch atılmamış sistemler, saldırganlar için açık bir davetiyedir. 🛡️

#### 🧠 Teorik Köşe: Active Directory'nin Kalbine İniyoruz
Pratiğe dalmadan önce bu kavramları sıfırdan öğrenelim:
-   **Active Directory Domain Services (AD DS) Nedir?:** Bu, bir Windows Server'a kurduğumuz bir **roldür**. Bu rolü kurduğumuzda, o sunucu artık sıradan bir sunucu olmaktan çıkar ve **Domain Controller (DC)** yani "Etki Alanı Yöneticisi" olur. AD DS, kullanıcı hesapları, parolalar, bilgisayarlar, izinler gibi tüm kritik bilgileri tutan merkezi bir veritabanı sağlar ve yönetir.
-   **Domain, Tree, Forest Hiyerarşisi:**
    -   **Domain (Etki Alanı):** Senin kurduğun `muzafferdomain.local` bir Domain'dir. Bunu bir krallık 🏰 olarak düşün. Bu krallığın kendi vatandaşları (kullanıcılar), binaları (bilgisayarlar) ve kanunları (Grup İlkeleri) vardır. Her şey bu krallığın kralı olan DC tarafından yönetilir.
    -   **Tree (Ağaç):** Ortak bir kök ismini paylaşan birden çok domain'in oluşturduğu yapıdır. Örneğin, ileride `satis.muzafferdomain.local` adında ikinci bir domain kurarsan, bu ikisi aynı ağacı 🌳 oluşturur.
    -   **Forest (Orman):** En üst yapıdır. Bir şirketin sahip olduğu tüm ağaçları içerir. Senin `muzafferdomain.local` ile kurduğun yapı, şu an tek bir ağaçtan oluşan bir ormandır. 🌲
-   **Organizational Unit (OU - Organizasyonel Birim):** Bir krallığın içindeki şehirler veya mahalleler gibidir. Domain'deki nesneleri (kullanıcı, grup, bilgisayar) düzenli tutmak için kullandığımız klasörlerdir 📁. Asıl gücü, farklı departmanlara farklı kurallar (GPO'lar) uygulamayı sağlamasıdır. Örneğin, "Muhasebe" OU'sundaki herkesin yazıcılara erişimi varken, "Stajyerler" OU'sundakilerin olmayabilir.
-   **Kullanıcılar ve Gruplar:**
    -   **Kullanıcı Hesabı (User Account):** Her bir bireyin ağa giriş yapmak için kullandığı dijital kimliğidir 👤.
    -   **Grup (Group):** Benzer ihtiyaçları olan kullanıcıları bir araya getiren bir listedir. İki ana türü vardır:
        -   **Security (Güvenlik) Grubu:** En yaygın olanıdır. Klasörlere, yazıcılara, kaynaklara **izin vermek** için kullanılır. Bunlar, bir odanın anahtarını 🔑 taşıyan gruplardır. Bizim `ITDepartmani` grubumuz bir güvenlik grubudur.
        -   **Distribution (Dağıtım) Grubu:** Sadece e-posta göndermek için kullanılır. Örneğin, `herkes@muzafferdomain.local` gibi bir e-posta listesi oluşturmak için. Bunların kaynaklara erişim izni olamaz.
    -   **Altın Kural 🏆:** İzinler **ASLA** tek tek kullanıcılara verilmez. Her zaman bir Güvenlik Grubu oluşturulur, izinler o gruba verilir ve kullanıcılar o gruba üye yapılır.

#### 💻 Pratik Zamanı: Teoriyi Eyleme Dökmek
1.  **OU Yapısını Oluşturma:** "Active Directory Users and Computers" konsolunu açarak, `muzafferdomain.local` domain'im altında `IT`, `HR` (İnsan Kaynakları) ve `Security` adında üç adet OU oluşturdum.
2.  **Kullanıcıları ve Grupları Oluşturma:**
    -   Her OU'nun içine, o departmanı temsil eden test kullanıcıları oluşturdum (`jamesdaniel.it`, `katecole.hr` vb.).
    -   **🔑 Şifre Mücadelesi:** Windows Server'ın varsayılan şifre karmaşıklığı ilkesi (büyük/küçük harf, rakam vb.) yüzünden şifre oluşturmakta zorlandım. Bu aslında iyi bir şey! Güvenliğin işlediğini gösterir. Çözüm olarak güçlü bir şifre oluşturucu kullandım.
    -   `ITDepartmani` adında bir **Global Güvenlik Grubu** oluşturdum ve `jamesdaniel.it` kullanıcısını bu gruba üye yaptım.
3.  **Dosya Paylaşımının İki Anahtarı: Paylaşım ve NTFS İzinleri:**
    -   Sunucumda "OrtakBelgeler" adında bir klasör açtım ve bu klasöre `ITDepartmani` grubunun erişmesini sağladım.
    -   **Paylaşım İzinleri (Binanın Giriş Kapısı):** Klasöre ağ üzerinden erişilip erişilemeyeceğini kontrol eder. Buradan `ITDepartmani` grubuna "Değiştirme (Change)" izni verdim.
    -   **NTFS Güvenlik İzinleri (Odaların Kilitleri):** Ağdan veya yerelden, klasöre erişildiğinde içinde ne yapılabileceğini (okuma, yazma, silme vb.) kontrol eder. Buradan `ITDepartmani` grubuna "Tam Denetim (Full Control)" verdim.
    -   **Unutma:** Kullanıcının nihai izni, bu ikisinden **en kısıtlayıcı olanıdır!**

#### 😱 Karşılaşılan Sorun ve "Aha!" Anı
Her şeyi ayarladıktan sonra `CLIENT01` makinesine `jamesdaniel.it` olarak giriş yaptım. Ağ'a tıklayıp sunucuma erişmeye çalıştığımda benden tekrar kimlik bilgisi istedi ve bir türlü bağlanamadım.
**Çözüm ve Öğrenilen Ders 💡:** Sorun, Windows'a hangi `administrator` hesabını kullanmak istediğimi söylemememdi. `CLIENT01` makinesinin kendi yerel `administrator` hesabı var, bir de benim domain'imin `administrator` hesabı var.
Doğru formatı kullandığımda sorun çözüldü:
`muzafferdomain\administrator`
Bu komut, Windows'a "Hayır, yerel yöneticiyi değil, `muzafferdomain` krallığının yöneticisini kullanarak bu işlemi yap!" demek anlamına geliyor. Bu, yeni başlayanların sıkça takıldığı çok değerli bir dersti.

#### 🏁 Günün Sonucu ve Kapanış Düşünceleri
Bugün, Active Directory'nin teorik derinliklerine inip bunu kendi laboratuvarımda hayata geçirdim. Hatalar yapmak ve bu hataların nedenini anlayarak çözmek, öğrenme sürecinin en kalıcı parçası. Bu rehberi günlük tutar gibi yazıyorum çünkü amacım sadece "şunu yapın" demek değil, aynı zamanda bu yolda yürürken başınıza gelebilecek gerçekçi senaryoları ve hisleri de paylaşmak. Umarım hep birlikte gelişiriz.

Yarınki hedefim, Windows Server serüvenini GPO (Grup İlke Nesneleri) ile daha derinlemesine inceleyerek tamamlamak.

Herkese bol çalışmalar, sağlıklı günler diliyorum  esenlikle kalın ! 🌟

---
<a id="gun-2025-08-06"></a>
## 🗓️ 6 Ağustos 2025
### GPO ile İmparatorluğun Kurallarını Yazmak ⚖️
Bugünkü Konu: Grup İlke Nesneleri (Group Policy Objects - GPO) ile merkezi yönetim. ⚖️

#### Günün Özeti
Bugün benim için hem yorucu hem de öğretici bir gündü. Beklenmedik bir aksilik yüzünden tüm laboratuvar ortamımı sıfırdan kurmak zorunda kalmak, planlarımı yavaşlatsa da pes etmedim ve günün hedefine, yani Active Directory'nin en güçlü silahlarından biri olan GPO'lara odaklandım. Zorluklara rağmen, bir domain'deki binlerce kullanıcı ve bilgisayar için kuralları tek bir yerden nasıl koyabileceğimizi görmek inanılmaz bir tatmin duygusu yaşattı.

#### 😱 Zorlu Başlangıç: Laboratuvarı Yeniden İnşa Etmek
Güne başlarken karşılaştığım bilgisayar değişikliği, tüm sanal makinelerimi, OU yapımı, kullanıcılarımı ve paylaşımlarımı en baştan kurmam gerektiği anlamına geliyordu. Bu gerçekten moral bozucu ve zaman alıcı bir süreçti. Ancak bu zorunlu tekrarın, önceki günlerde öğrendiğim temel bilgileri ne kadar pekiştirdiğini de fark ettim. Bazen en iyi öğrenme, beklenmedik tekrarlarla gelir. 💪

#### 🧠 Teorik Köşe: GPO (Group Policy Object) Nedir?
GPO, bir domain yöneticisinin sahip olduğu en güçlü araçtır. Onu, krallığımızın (muzafferdomain.local) Anayasa ve Kanun Kitabı 📜 olarak düşünebiliriz. GPO'lar sayesinde, binlerce bilgisayar ve kullanıcı için ayarları tek tek yapmak yerine, merkezi kurallar belirleyip bunları otomatik olarak uygulayabiliriz.

#### Nasıl Çalışır?: Bir GPO oluşturur ve onu bir OU'ya (Organizasyonel Birim) bağlarsınız. O andan itibaren, o GPO içindeki tüm kurallar, o OU içindeki tüm kullanıcılara ve/veya bilgisayarlara uygulanır.

İşlem Sırası (LSDOU): GPO'lar belirli bir hiyerarşide işlenir: Local (Yerel Bilgisayar) -> Site (Fiziksel Lokasyon) -> Domain (Tüm Etki Alanı) -> OU (Organizasyonel Birim). Bu, en son uygulanan (genellikle OU'ya bağlanan) polisin en geçerli olduğu anlamına gelir. Bu yüzden OU'lar bu kadar önemlidir!

Kullanıcı ve Bilgisayar Yapılandırması: Her GPO'nun içinde iki ana bölüm vardır:

Computer Configuration: Bilgisayar açıldığında uygulanan ayarlardır. Kimin oturum açtığından bağımsızdır. (Örn: Windows Güvenlik Duvarı ayarları)

User Configuration: Bir kullanıcı oturum açtığında uygulanan ayarlardır. Hangi bilgisayarda oturum açtığından bağımsızdır. (Örn: Masaüstü arkaplanını değiştirmek)

#### 💻 Pratik Zamanı: IT Departmanına Özel Kurallar
Teoriyi öğrendikten sonra, IT OU'suna özel bir GPO oluşturarak aşağıdaki kuralları uyguladım:

1. Özel Parola Politikası Oluşturma
IT departmanının daha güvenli parolalar kullanmasını sağlamak için, domain genelindeki politikadan daha sıkı bir politika belirledim. Bu politika, şifrelerin en az 12 karakter olmasını, karmaşıklık kurallarına uymasını ve son 5 şifrenin tekrar kullanılamamasını zorunlu kıldı.

<img width="1906" height="1024" alt="password" src="https://github.com/user-attachments/assets/60dc68f3-be0a-4370-bdfb-73f14e9b7e4c" />


2. CMD ve PowerShell'e Erişimi Engellemek
Güvenlik nedeniyle, standart IT kullanıcılarının Komut İstemi'ne (CMD) ve PowerShell'e erişimini engellemek istedim. "User Configuration" altında, kullanıcıların belirli uygulamaları çalıştırmasını engelleyen politikayı bularak cmd.exe ve powershell.exe'yi listeye ekledim.

<img width="1903" height="1025" alt="Prevent access to the command prompt" src="https://github.com/user-attachments/assets/23dc5b90-9fe9-420e-b51e-8a6c2f43b914" />


3. İnteraktif Giriş Mesajı Eklemek
Kullanıcılar oturum açmadan önce onlara bir uyarı veya bilgilendirme metni göstermek, güvenlik farkındalığı için harika bir yöntemdir. IT OU'sundaki kullanıcılar için, oturum açma ekranında "Bu sistem sadece yetkili IT personeli içindir. Tüm aktiviteler kayıt altına alınmaktadır." gibi bir başlık ve mesaj belirledim.

<img width="1910" height="1006" alt="Do not display last user name" src="https://github.com/user-attachments/assets/189d2b05-93cb-4eb8-a6d3-0252afe13175" />


🏁 Günün Sonucu ve Kapanış Düşünceleri
Bugün, başlangıçtaki tüm aksiliklere rağmen GPO'nun temel mantığını ve gücünü kavramakla geçti. Birkaç tıklama ile tüm bir departmanın çalışma ortamını nasıl şekillendirebildiğini görmek müthiş bir deneyimdi. Çok yorucu bir gün oldu ama değdi.

Umarım yarın Windows Server ile ilgili son konuları da tamamlayıp bu ilk büyük adımı bitirebilirim. Herkese bol çalışmalar, sağlıklı günler diliyorum  esenlikle kalın ! 🌟

---
<a id="gun-2025-08-07"></a>
## 🗓️ 7 Ağustos 2025
### Windows Server'da Ustalığa Son Adım: DNS, DHCP ve Ötesi 🎉
Bugünkü Konu: Windows Server yönetiminin temel taşları ve yol haritasının ilk büyük bölümünün tamamlanışı! 🎉

#### Günün Özeti
Bugün, Windows Server serüvenimde son ve en kritik konulara dalarak uzun ama inanılmaz keyifli bir çalışma seansı gerçekleştirdim. Ağın görünmez kahramanları olan DNS ve DHCP'den başlayıp, veri depolamanın kalbi olan Dosya Sunucusu'na, oradan da sistemin sağlığını izlemeye kadar geniş bir yelpazeyi ele aldım. Her bir konu, bir sistem yöneticisinin ve bir Blue Teamer'ın bilmesi gereken temel yetenekleri içeriyordu. Günün sonunda, yol haritamdaki ilk büyük bölümü tamamlamanın gururunu yaşıyorum!

#### 🌐 1. DNS ve DHCP: Ağın Posta Adresi ve Otomatik Kapı Numarası
🧠 Teorik Köşe
DNS (Domain Name System) Nedir?: İnternetin ve yerel ağların "telefon rehberidir" 📖. www.google.com gibi insanların anladığı isimleri, 172.217.16.196 gibi bilgisayarların anladığı IP adreslerine çevirir. Onsuz, her site için IP adresi ezberlemek zorunda kalırdık!

Temel Kayıt Türleri: A (İsmi IPv4'e çevirir), AAAA (İsmi IPv6'ya çevirir), CNAME (Bir isme başka bir isim takma - alias), MX (Mail sunucusunu belirtir), PTR (IP'yi isme çevirir - Reverse DNS).

Zone Türleri: Forward Lookup Zone (isimden IP'ye) ve Reverse Lookup Zone (IP'den isme) en temel iki bölgedir.

DHCP (Dynamic Host Configuration Protocol) Nedir?: Ağa yeni katılan cihazlara otomatik olarak IP adresi, alt ağ maskesi, ağ geçidi ve DNS sunucusu gibi bilgileri atayan servistir. Ağa her yeni cihaz bağlandığında manuel IP vermenin kabusunu ortadan kaldırır. 🤖

İlişkileri: DHCP, bir cihaza IP verdiğinde, bu bilgiyi otomatik olarak DNS'e kaydettirebilir (Dynamic DNS). Böylece CLIENT01 bilgisayarı 192.168.100.125 IP'sini aldığında, bu bilgi DNS'e anında işlenir.

#### 💻 Pratik Zamanı
Önce Server Manager üzerinden DNS ve DHCP rollerini kurdum.

DNS Yapılandırması:

muzafferdomain.local için bir Forward Lookup Zone oluşturdum.

192.168.100.x ağı için bir Reverse Lookup Zone oluşturdum. Burada bir ders aldım: İlk denememde "Secondary Zone" olarak oluşturduğum için IP-isim eşleşmesinde sürekli hata aldım. Araştırınca, bu ana sunucuda bölgenin "Primary Zone" olması gerektiğini öğrendim.

nslookup komutu ile test ettiğimde muzafferdomain.local'in çözümlenmediğini gördüm. Sebebi, sunucunun kendi A kaydının otomatik oluşmamasıydı. Manuel olarak SERVER01 -> 192.168.100.10 şeklinde bir A kaydı oluşturunca sorun düzeldi. ✅

DHCP Yapılandırması:

LAN_SCOPE adında yeni bir Scope (kapsam) oluşturdum ve dağıtılacak IP aralığını 192.168.100.100 - 192.168.100.200 olarak belirledim.

Sunucu, router gibi sabit IP'li cihazların bu aralıktan IP almaması için 192.168.100.1 - 10 arasını Exclusion (Hariç Tutma) olarak ekledim.

Scope Options'da DNS sunucusu olarak sunucumun IP'sini (192.168.100.10) girdim.

CLIENT01 makinesine geçip yönetici CMD'sinde ipconfig /release ve ipconfig /renew komutlarını çalıştırdım. ipconfig /all ile kontrol ettiğimde, istemcimin belirlediğim aralıktan (100'lü bir IP) başarılı bir şekilde IP aldığını gördüm!

Tavsiye: VirtualBox'ın kendi DHCP ve ağ yapıları bazen kafa karıştırabiliyor. Bu tür testlerde VirtualBox'ın ağ ayarlarını (NAT, Internal Network vb.) doğru yapılandırdığınızdan emin olun.

#### 📁 2. Dosya Sunucusu ve Depolama Yönetimi: Verinin Kalesi
#### 🧠 Teorik Köşe
File Server Rolü: Kullanıcıların dosyalarını merkezi bir sunucuda depolamasını, paylaşmasını ve yönetmesini sağlar. Bu, veri güvenliği, yedekleme ve yetkilendirme için kritiktir.

Auditing (Denetim) ve Effective Access (Etkin Erişim): Blue Team için hayati iki kavram!

Auditing: Kimin, hangi dosyaya, ne zaman eriştiğini, ne yaptığını (okudu, sildi, değiştirdi) kaydeden bir güvenlik günlüğü oluşturur. Bir olay anında "suçluyu" bulmak için bu loglara bakarız.

Effective Access: Bir kullanıcının bir dosya veya klasör üzerinde sahip olduğu nihai izni gösterir. Bazen bir kullanıcı birden çok gruba üye olur ve izinleri karmaşıklaşır. Bu araç, "Ahmet bu dosyayı neden silemiyor?" sorusunun net cevabını verir.

#### 💻 Pratik Zamanı
File Server rolünü kurdum.

SMB Share - Quick sihirbazı ile C sürücüsünde OrtakAlan adında yeni bir paylaşılan klasör oluşturdum.

İzinlerini ITDepartmani grubunun tam yetkili olacağı şekilde ayarladım.

Blue Team Adımı: Paylaşılan klasörün denetim (Auditing) ayarlarını açtım. Fakat logların yazılması için önce GPO üzerinden "Audit object access" politikasını hem başarılı hem de başarısız denemeler için aktif hale getirdim. Artık bu klasöre yapılan her erişim, Security Event Log'una yazılacak!

CLIENT01 üzerinden \\192.168.100.10\OrtakAlan UNC yolu ile klasöre başarıyla eriştim.

#### 💾 3. Yedekleme, 📊 Performans ve 🌐 Uzak Erişim
Özet
Günün sonuna doğru bu konuları ele aldım. Eski bir bilgisayarla çalışıyorsanız yedekleme ve sanallaştırma işlemleri bir işkenceye dönüşebiliyor, bu yüzden bazı adımları sadece teorik ve pratik adımlarını izleyerek geçtim.

Windows Server Backup: Yedekleme sihirbazını çalıştırdım ve adımları takip ettim.

<img width="1914" height="973" alt="backup" src="https://github.com/user-attachments/assets/df3544bd-da1f-4ac8-a367-c7cf806af171" />


VSS ve Görev Zamanlayıcı: Veriler kullanılırken bile tutarlı bir yedeğini alan Volume Shadow Copy Service (VSS)'in ne kadar önemli olduğunu ve Task Scheduler ile yedeklemelerin nasıl otomatikleştirileceğini öğrendim.

<img width="1907" height="970" alt="shadow copies" src="https://github.com/user-attachments/assets/16b749a4-0098-4e2b-8113-9df7a856d2db" />


Performans İzleme: perfmon aracını açarak CPU, Memory ve Disk kullanımı gibi sayaçları ekleyip sunucunun nabzını canlı olarak izledim. Bu verileri daha sonra analiz etmek için bir Data Collector Set oluşturdum.

<img width="1919" height="1029" alt="performance collector" src="https://github.com/user-attachments/assets/1cecec7e-b7b8-4a71-8e8e-751847bebdd1" />

<img width="1915" height="977" alt="create collector" src="https://github.com/user-attachments/assets/08df4ab1-a46e-4883-9046-23ddfc379096" />

Remote Access ve Hyper-V: Performans sorunları nedeniyle bu konuları (RDP, VPN, Hyper-V Kurulumu, Sanal Makine oluşturma, Nested Virtualization vb.) maalesef sadece teorik ve videolar üzerinden çalışarak tamamladım.

🏁 Günün Sonucu ve Büyük Başarı: Windows Server Bölümü Tamamlandı!
Bugün, yol haritamızdaki "Operating System Mastery" bölümünün Windows Server kısmını ve hatta AD/GPO temellerini tamamen bitirmiş oldum! Çok sayıda konuyu bir güne sığdırmak yorucuydu ama her bir parçanın birbiriyle nasıl konuştuğunu görmek paha biçilmezdi. Artık sağlam bir Windows altyapısına sahibim.

Sıradaki büyük macera, Linux yönetimi! Herkese bol çalışmalar, sağlıklı günler diliyorum  esenlikle kalın ! 🌟

---
<a id="gun-2025-08-11"></a>
## 🗓️ 11 Ağustos 2025
### Linux Yönetimi, Script Temelleri ve Sistem Loglarıyla Yolculuk Devam Ediyor 🐧

**Bugünkü Konu:** Linux administration (Ubuntu, CentOS, RHEL), PowerShell ve Bash scripting basics, System logging and event management. Artık bir sonraki büyük adım olan Network Deep Dive ünitesine geçmeye hazırım! 🚀

#### Günün Özeti
Bugün, siber güvenlik yolculuğumda Windows dünyasından çıkıp Linux evrenine adım attım. Ardından hem PowerShell hem de Bash script temellerini keşfettim ve sistem loglarının nasıl yönetildiğine dair önemli bilgiler edindim. Tüm bu konular, ileride daha derinlemesine çalışmak için sağlam bir temel oluşturdu. 💪

#### 🐧 Linux Nedir? Temeller ve Dağıtımlar
Öncelikle Linux'un ne olduğuna baktım. Linux, topluluklar ve şirketler tarafından geliştirilen, açık kaynaklı bir işletim sistemidir. Temelinde "kernel" (çekirdek) bulunur ve bu çekirdek üzerine farklı "dağıtımlar" (distributions) inşa edilir. Kernel, donanım ile yazılım arasındaki köprüdür. Dağıtımlar ise kernel + ek yazılımlar + araçlar + paket yöneticisi gibi bileşenlerden oluşur.

Windows ile Linux'un çekirdek yapısını karşılaştırdım. Linux, modüler ve açık kaynaklı bir çekirdeğe sahipken, Windows daha kapalı ve monolitik bir yapıya sahip. Popüler Linux dağıtımlarına göz attım: Ubuntu, CentOS, RHEL ve tabii ki daha önce kullandığım Arch Linux! Arch bana tanıdık geldiği için bu kısımlar hatırlatıcı oldu. 😊

#### 📁 Linux Dosya Sistemi ve Dizinler
Linux'ta dosya sistemi mantığını öğrendim. Kök dizin (/) her şeyin başlangıcı. Temel dizinlerin ne işe yaradığını tabloyla özetledim:

| Dizin        |  Açıklama                                      |
|--------------|------------------------------------------------|
| /            | Kök dizin, tüm dosya ve klasörlerin başlangıcı |
| /bin         | Temel komutlar (ls, cp, mv, rm, vb.)           |
| /sbin        | Sistem yönetim komutları                       |
| /etc         | Sistem yapılandırma dosyaları                  |
| /home        | Kullanıcıların kişisel dizinleri               |
| /var         | Değişken veriler (loglar, spool, vb.)          |
| /tmp         | Geçici dosyalar                                |
| /usr         | Kullanıcı programları ve kütüphaneler          |
| /opt         | Ek yazılımlar                                  |
| /root        | Root kullanıcısının ana dizini                 |

#### 📦 Paket Yönetimi ve Temel Komutlar
Paket yönetimine geçtim. Ubuntu'da `apt`, CentOS/RHEL'de `yum` ve `dnf` kullanılıyor. Temel kavramlar:
- `update`, `upgrade`, `install`, `remove` gibi işlemler
- `sudo` ile yönetici yetkisi kazanma

#### 👤 Kullanıcı ve Yetki Yönetimi
Kullanıcı ekleme, parola atama, kullanıcı silme, grup ekleme ve kullanıcıyı gruba dahil etme işlemlerini öğrendim. Dosya/dizin izinlerinde `r` (okuma), `w` (yazma), `x` (çalıştırma) tiplerini ve chmod/chown komutlarını pratik ettim.

#### ⚙️ Servis ve Process Yönetimi
Process (işlem) ve service (hizmet) kavramlarını öğrendim. `ps`, `top`, `systemctl`, `service` gibi komutlarla uygulamalı denemeler yaptım. Bu tarz komutlar, aktif kullanıldıkça daha kalıcı oluyor; o yüzden ileride Linux'u daha fazla kullanarak pekiştireceğim.

#### 🌐 Ağ Yönetimi
Ağ birimlerini ve IP yapılandırmasını inceledim. `ip a`, `ifconfig`, `route`, `ping`, `nslookup`, `cat /etc/resolv.conf` gibi komutlarla ağ yapılandırması ve DNS testleri yaptım.

#### 📝 Log Yönetimi
Logların nerede tutulduğunu ve canlı log takibini öğrendim. Özellikle `/var/log/syslog` ve hata içeren loglara bakmak için kullanılan komutları pratik ettim. Log yönetimi, sistemde neler olup bittiğini anlamak için çok önemli!

#### 💾 Yedekleme
Linux'ta 3 tip yedekleme yöntemini inceledim (tam, artımlı, diferansiyel). Temel mantıklarını kavradım.

#### ⚡ PowerShell ve Bash Scripting Temelleri
Script nedir, ne işe yarar sorusuyla başladım. PowerShell ve Bash'te temel script yazımını ve farklarını öğrendim. PowerShell'de komutlar nesne tabanlıdır, çıktılar metin değil nesnedir. Komutlar pipeline (|) ile bağlanır. Değişkenler `$` ile başlar. Dosya uzantısı `.ps1`.

PowerShell temel komutları:
- `Get-Help <komut>` — Komut hakkında yardım al
- `Get-Process` — Çalışan işlemleri listeler
- `Get-Service` — Hizmetleri gösterir
- `Set-ExecutionPolicy RemoteSigned` — Script çalıştırma izinlerini ayarlar
- `Write-Output "Merhaba Dünya"` — Ekrana çıktı verir

Bash temel komutları:
- `echo "Merhaba Dünya"` — Yazdırır
- `ls` — Dosya listesi
- `pwd` — Bulunduğun dizin
- `chmod +x script.sh` — Çalıştırılabilir yapar
- `./script.sh` — Scripti çalıştırır

Değişkenler ve veri tipleri:
- PowerShell'de dinamik tipli, tür belirtilmez
- Bash'te tüm değerler string olarak kabul edilir, tip dönüşümleri manuel yapılır

Koşullar, döngüler ve fonksiyonları temel olarak inceledim. Ancak bu konuların daha kalıcı olması için ileride Python ile birlikte tekrar çalışacağım.

#### 📝 System Logging & Event Management
Sistem loglarının ne olduğunu, log türlerini ve Windows Event Log sistemini öğrendim. Event Viewer'a göz attım. Linux'ta ise `/var/log/syslog` ve diğer log dosyalarını inceledim.

---

#### 🏁 Günün Sonucu ve Sonraki Adım
Bugün, Linux yönetimi ve script temelleriyle ilgili önemli bir aşamayı tamamladım. Konuların çoğu daha önce bildiğim için hızlıca ilerledim, odak noktam hatırlatıcı ve rehber niteliğinde çalışmak oldu. Bundan sonraki ünitede "Network Deep Dive" ile ağ dünyasına daha derinlemesine dalacağım!

Herkese bol çalışmalar, sağlıklı günler diliyorum  esenlikle kalın ! 🌟

---
<a id="gun-2025-08-12"></a>
## 🗓️ 12 Ağustos 2025
### Networking Deep Dive – Ağların Derinliklerine Yolculuk! 🌐

**Bugünkü Konu:** TCP/IP stack ve OSI modeli, ağ protokolleri (HTTP/HTTPS, DNS, DHCP, SMTP), ağ cihazları (switch, router, firewall), ağ segmentasyonu ve VLAN’lar. Wireshark’ı ise pratik gerektirdiği için yarına bırakıyorum! 🕵️‍♂️

#### Günün Özeti
Bugün, siber güvenlik yolculuğumda yepyeni bir üniteye, Networking Deep Dive’a başladım. Ağların temellerini, protokolleri, cihazları ve segmentasyon kavramlarını derinlemesine inceledim. Bu konular, Blue Team için olmazsa olmaz teorik bilgiler! Her başlıkta hem temel kavramları hem de pratikte karşılaşabileceğim detayları öğrenmeye odaklandım. Şimdi adım adım ilerleyelim:

---

#### 1️⃣ Temel Ağ Kavramları
- **Ağ (Network):** İki veya daha fazla cihazın veri iletişimi yapabilmesi için birbirine bağlanmasıdır. Modern dünyada, bilgisayarlar, telefonlar, yazıcılar ve hatta IoT cihazları bile ağlara bağlıdır.
- **Host:** Ağa bağlı herhangi bir cihaz (PC, sunucu, yazıcı, kamera vb.).
- **Node:** Ağ üzerinde veri gönderebilen veya alabilen her cihaz. Her host bir node’dur, ama her node host olmayabilir (ör: switch).
- **Interface:** Cihazın ağa bağlandığı fiziksel ya da sanal bağlantı noktasıdır. Genellikle NIC (Network Interface Card) olarak adlandırılır. Bir cihazda birden fazla interface olabilir (ör: Ethernet, Wi-Fi).

---

#### 2️⃣ OSI Modeli ve TCP/IP Stack
- **OSI Modeli (7 Katman):** Ağ iletişimini anlamak için geliştirilmiş teorik bir modeldir. Her katman, belirli bir işlevi yerine getirir:
    1. **Physical (Fiziksel):** Kablolar, elektrik sinyalleri, fiber optik, radyo dalgaları. Donanım seviyesidir.
    2. **Data Link (Veri Bağlantı):** MAC adresleri, çerçeveler, Ethernet. Switch’ler bu katmanda çalışır.
    3. **Network:** IP adresleme, yönlendirme. Router’lar burada çalışır.
    4. **Transport:** TCP/UDP, port numaraları, hata kontrolü, veri akışı.
    5. **Session:** Oturum yönetimi, bağlantıların kurulması ve sonlandırılması.
    6. **Presentation:** Veri formatı, şifreleme, sıkıştırma. Farklı sistemler arası veri dönüşümü.
    7. **Application:** Kullanıcıya görünen servisler (HTTP, FTP, DNS, e-posta vb.).

- **TCP/IP Modeli (4 Katman):** Gerçek dünyada daha çok kullanılan, pratik bir modeldir:
    1. **Network Access (Physical + Data Link):** Donanım ve bağlantı protokolleri.
    2. **Internet (Network):** IP adresleme ve yönlendirme.
    3. **Transport:** TCP/UDP, portlar.
    4. **Application (Session + Presentation + Application):** Uygulama protokolleri.

> 📌 **Not:** OSI modeli daha çok öğretici ve teoriktir, TCP/IP ise gerçek ağlarda uygulanan modeldir.

---

#### 3️⃣ TCP/IP Temelleri ve IP Adresleme
- **IPv4:** 32-bit adresleme, 4 oktet (ör: 192.168.1.1). Sınırlı adres alanı nedeniyle günümüzde IPv6’ya geçiş hızlanıyor.
- **IPv6:** 128-bit adresleme, çok daha geniş adres alanı (ör: 2001:0db8::1). Geleceğin interneti için kritik.
- **Subnet Mask:** IP adresinin ağ ve host kısmını ayırır (ör: 255.255.255.0). Alt ağlar oluşturmak için kullanılır.
- **Default Gateway:** Ağdan dış dünyaya (ör: internete) çıkış noktasıdır. Genellikle router’ın IP’sidir.
- **Port Numaraları:**
    - 0–1023: Well-known ports (HTTP: 80, HTTPS: 443, DNS: 53, SSH: 22)
    - 1024–49151: Registered ports
    - 49152–65535: Dynamic/Ephemeral ports
- **CIDR Notasyonu:** IP adresi + “/” ile subnet mask gösterimi (ör: 192.168.1.0/24). Daha esnek ağ tasarımı sağlar.
- **Özel IP Aralıkları (RFC 1918):**
    - 10.0.0.0/8
    - 172.16.0.0/12
    - 192.168.0.0/16
  Bu adresler internette yönlendirilmez, yerel ağlarda kullanılır.

---

#### 4️⃣ Yaygın Ağ Protokolleri
- **HTTP/HTTPS:** Web trafiği (80/443). HTTPS, SSL/TLS ile şifrelenmiş güvenli iletişim sağlar.
- **DNS:** Alan adlarını IP adresine çevirir (53 UDP/TCP). İnternetin telefon rehberi gibidir.
- **DHCP:** Otomatik IP adresi, ağ geçidi, DNS gibi bilgileri dağıtır (67/68 UDP). Ağ yönetimini kolaylaştırır.
- **SMTP / IMAP / POP3:** E-posta gönderme ve alma protokolleri. SMTP (25), IMAP (143/993), POP3 (110/995).
- **FTP / SFTP:** Dosya transferi. FTP (21) şifresiz, SFTP (22) SSH üzerinden güvenli.
- **SNMP:** Ağ cihazlarının izlenmesi ve yönetimi için kullanılır.
- **SSH:** Güvenli uzaktan bağlantı (22). Özellikle sunucu yönetiminde vazgeçilmezdir.

> 🔎 **Ekstra:** Protokollerin çoğu hem TCP hem UDP kullanabilir. UDP hızlı ama güvenilmez, TCP ise bağlantı odaklı ve güvenilirdir.

---

#### 5️⃣ Ağ Cihazları ve Görevleri
- **Switch:** Layer 2 cihazıdır, MAC adreslerine göre veri iletir. VLAN desteği ile ağları mantıksal olarak bölebilir. Modern switch’ler yönetilebilir (managed) veya yönetilemez (unmanaged) olabilir.
- **Router:** Layer 3 cihazıdır, IP adreslerine göre yönlendirme yapar. Farklı ağlar arasında veri iletimini sağlar. Evdeki modemler genellikle router’dır.
- **Firewall:** Trafiği filtreler, güvenlik politikaları uygular. Donanım (hardware) veya yazılım (software) tabanlı olabilir. Paket filtreleme, stateful inspection ve proxy gibi farklı türleri vardır.
- **Access Point:** Kablosuz ağ erişimi sağlar. Genellikle switch veya router’a bağlıdır.
- **Load Balancer:** Trafiği birden fazla sunucuya dağıtarak yükü dengeler, yüksek erişilebilirlik sağlar.

> 🛡️ **Not:** Blue Team için firewall ve IDS/IPS cihazlarının doğru yapılandırılması kritik önemdedir.

---

#### 6️⃣ Ağ Segmentasyonu ve VLAN’lar
- **Ağ Segmentasyonu:** Büyük bir ağı, daha küçük mantıksal parçalara ayırmak. Broadcast domain’leri küçültür, performansı ve güvenliği artırır.
- **VLAN (Virtual LAN):** Layer 2 üzerinde mantıksal ağlar oluşturur. Farklı VLAN’lar, aynı fiziksel switch üzerinde bile birbirinden izole olabilir. VLAN’lar arası iletişim için router veya Layer 3 switch gerekir.
- **Faydaları:**
    - Performans artışı (daha az broadcast)
    - Güvenliğin artması (farklı departmanlar izole edilir)
    - Yönetim kolaylığı

> 🧩 **Ekstra:** VLAN’lar, özellikle büyük şirketlerde departman bazlı ağ ayrımı için kullanılır. Örneğin, IT, HR ve Guest VLAN’ları.

---

#### 7️⃣ Paket Akışı (Packet Flow) ve Ağda Veri Yolculuğu
- Uygulama katmanında veri oluşur (ör: bir web sayfası isteği).
- Transport katmanında TCP/UDP portu eklenir.
- Network katmanında IP adresi eklenir.
- Data Link katmanında MAC adresi eklenir.
- Fiziksel katmanda veri, kablo veya Wi-Fi üzerinden iletilir.
- Karşı tarafta bu süreç tersine çözülür ve veri uygulamaya ulaşır.

> 📦 **Not:** Paketlerin ağda nasıl yol aldığını anlamak, sorun giderme ve güvenlik için çok önemlidir.

---

#### 8️⃣ Ağ Güvenliği Temelleri
- **ACL (Access Control List):** Hangi trafiğin geçeceğini veya engelleneceğini belirler. Router ve firewall’larda kullanılır.
- **NAT (Network Address Translation):** Yerel (özel) IP’leri internete çıkarken tek bir genel IP’ye çevirir. Ev ağlarında yaygındır.
- **VPN (Virtual Private Network):** Uzak ağlara güvenli tünel ile erişim sağlar. Şirketler için uzaktan çalışma çözümüdür.
- **IDS/IPS:** Saldırı tespit (Intrusion Detection System) ve önleme (Intrusion Prevention System) sistemleri. Ağ trafiğini analiz ederek şüpheli aktiviteleri tespit eder.

---

#### 9️⃣ İzleme ve Sorun Giderme Araçları
- **ping:** Hedefe erişilebilir mi test eder.
- **traceroute / tracert:** Paketlerin geçtiği yolları listeler, ağdaki gecikme ve kopuklukları bulmak için kullanılır.
- **nslookup / dig:** DNS sorguları yapar, alan adlarının IP karşılığını bulur.
- **netstat / ss:** Aktif bağlantıları ve portları listeler.
- **tcpdump / Wireshark:** Ağ trafiğini analiz eder. Wireshark, görsel arayüzüyle paketleri detaylı incelemek için çok güçlüdür (bunu yarın detaylıca çalışacağım!).

> 🛠️ **Ekstra:** Bu araçlar, ağda sorun giderme ve güvenlik analizi için Blue Team’in vazgeçilmezidir.

---

#### 🏁 Günün Sonucu ve Sonraki Adım
Bugün, ağların temellerinden başlayıp, protokoller, cihazlar, segmentasyon ve güvenlik konularına kadar kapsamlı bir teorik altyapı oluşturdum. Wireshark gibi pratik gerektiren araçları ise yarına bırakıyorum. Networking bilgisi, siber güvenliğin temel taşlarından biri ve Blue Team için vazgeçilmez! Yarın daha fazla pratik ve uygulama ile devam edeceğim.

Herkese bol çalışmalar, sağlıklı günler diliyorum  esenlikle kalın ! 🌟

---
<a id="gun-2025-08-14"></a>
## 🗓️ 14 Ağustos 2025
### Wireshark ile Trafik Analizi – Protokollerin Derinliklerine Yolculuk! 🕵️‍♂️🌐

**Bugünkü Konu:** Wireshark ile ağ trafiği analizi ve internet protokollerinin detaylı incelenmesi. Bugün hem teorik hem pratik olarak protokolleri ve Wireshark'ın temel özelliklerini keşfettim! 🚦

#### Günün Özeti
Bugün, siber güvenlik yolculuğumda Wireshark programını kullanarak ağ trafiği analizine odaklandım. Hacker Joe'nun Wireshark tanıtım videosunu izledim ve videoda vurgulanan internet protokollerini tekrar gözden geçirdim. Daha önce bu konuları çalışmış olsam da, bazı detayları kaçırmış olabileceğimi fark ettim ve eksik kalan noktaları tamamlamak için tekrar ettim. Gerçekten de bazı protokolleri yüzeysel geçtiğimi fark ettim! 🔍

---

#### 🌐 İnternet Protokolleri: Teorik Bilgiler ve Örnekler
Bugün üzerinde durduğum protokolleri ve kavramları tek tek açıklayacağım. Her birinin ne işe yaradığını, nasıl çalıştığını ve pratikte nerede karşılaşabileceğimizi örneklerle anlatacağım. 👨‍🏫

- **IP Adresi:** Bir cihazın ağdaki kimliğidir. Örneğin, evdeki bilgisayarın IP'si `192.168.1.5` olabilir. Her cihazın benzersiz bir IP adresi olmalı ki veri doğru yere ulaşsın.
- **Public ve Private IP Adresi:**
    - *Public IP* (Genel IP): İnternete çıkarken kullandığımız, ISP tarafından verilen IP'dir. Örneğin, evdeki modeminizin dış dünyaya görünen IP'si.
    - *Private IP* (Yerel IP): Ev veya iş ağında kullanılan, internette yönlendirilmez. Örneğin, `192.168.1.10`.
- **LAN (Local Area Network):** Ev, okul veya ofis gibi küçük bir alanda cihazların birbirine bağlandığı ağdır. Örneğin, evdeki bilgisayarlar ve yazıcılar aynı LAN'da olabilir.
- **NAT (Network Address Translation):** Birden fazla cihazın internete tek bir public IP ile çıkmasını sağlar. Evdeki tüm cihazlar, modem sayesinde NAT ile internete çıkar. 🏠➡️🌍
- **DHCP (Dynamic Host Configuration Protocol):** Cihazlara otomatik IP adresi, ağ geçidi ve DNS bilgisi dağıtır. Örneğin, yeni bir telefon Wi-Fi'ya bağlandığında IP'sini DHCP ile alır.
- **IP Paketi ve İçeriği:** Bir IP paketi, verinin ağda taşınan birimidir. İçinde kaynak/destinasyon IP, protokol bilgisi ve veri bulunur.
- **TCP (Transmission Control Protocol):** Güvenilir veri iletimi sağlar. Bağlantı kurmak için "3-way handshake" (SYN, SYN-ACK, ACK) kullanır. Örneğin, bir web sitesine bağlanırken TCP ile iletişim kurarsın.
    - *SYN, FIN, RST, URG, PSH, ACK bayrakları:* TCP paketlerinde bağlantı yönetimi için kullanılır. Mesela SYN ile bağlantı başlatılır, FIN ile sonlandırılır.
    - *Acknowledgement Number:* Gönderilen verinin alındığını onaylayan numaradır. Pizza siparişi örneği: Sipariş verirsin (SYN), restoran onaylar (SYN-ACK), sen de onayladığını bildirirsin (ACK).
- **UDP (User Datagram Protocol):** Hızlı ama güvenilir olmayan veri iletimi sağlar. Örneğin, canlı yayın veya oyunlarda UDP kullanılır.
- **DNS (Domain Name System):** Alan adlarını IP'ye çevirir. "www.google.com" yazınca, DNS sunucusu IP adresini bulur.
- **SNMP (Simple Network Management Protocol):** Ağ cihazlarını izlemek ve yönetmek için kullanılır. Örneğin, bir switch'in durumunu SNMP ile takip edebilirsin.
- **NTP (Network Time Protocol):** Ağdaki cihazların saatlerini senkronize eder. Tüm sunucuların aynı zamanı kullanması için gereklidir.
- **ARP (Address Resolution Protocol):** IP adresini MAC adresine çevirir. Bir bilgisayar, aynı ağdaki başka bir cihaza veri göndereceğinde ARP ile MAC adresini bulur.
- **Router:** Farklı ağlar arasında veri ileten cihazdır. Evdeki modem genellikle router işlevi görür.
- **Gateway:** Ağdan dış dünyaya çıkış noktasıdır. Genellikle router'ın IP'si gateway olur.
- **Switch:** Aynı ağdaki cihazları birbirine bağlar. Switch, MAC adreslerine göre veri iletir.
- **FTP (File Transfer Protocol):** Dosya transferi için kullanılır. Genellikle port 21 üzerinden çalışır.
- **SMB (Server Message Block):** Windows ağlarında dosya ve yazıcı paylaşımı için kullanılır.
- **Telnet:** Uzak cihazlara komut satırı üzerinden bağlanmak için kullanılır. Güvensizdir, şifreler açık gider.
- **HTTP (Hypertext Transfer Protocol):** Web trafiği için kullanılır. "http://" ile başlayan siteler bu protokolü kullanır.

Her protokolün Wireshark'ta nasıl göründüğünü test ettim ve pratikte karşılaştığım örnekleri inceledim. 🍕💻

---

#### 🦈 Wireshark ile Pratik: Temel Özellikler ve İpuçları
Videoda öğrendiklerimi Wireshark üzerinde denedim. Program düşündüğümden daha kolay ve kullanıcı dostu geldi! 👀

- **Ağ Seçimi ve Filtreleme:** Wireshark'ta analiz etmek istediğin ağı seçiyorsun. En üstteki arama çubuğu ile filtreleme yapmak çok kolay. Örneğin, sadece TCP paketlerini görmek için `tcp` yazmak yeterli.
- **Filtre Operatörleri:** Arama çubuğunda `or`, `and`, `not` gibi operatörlerle filtreleri özelleştirebiliyorsun. Mesela, hem TCP hem UDP paketlerini görmek için `tcp or udp` yazabilirsin.
- **Renk Kodlama:** Paketleri daha kolay ayırt etmek için filtrelere özel renkler atayabiliyorsun. Örneğin, DNS paketlerini mavi, HTTP paketlerini yeşil yapabilirsin. Bu görsel olarak analiz sürecini hızlandırıyor! 🎨
- **Profil Sistemi:** Sağ altta "Profile" kısmı var. Buradan farklı analiz profilleri oluşturup ayarlarını dışa aktarabiliyor veya profiller arasında geçiş yapabiliyorsun. Hedefe göre özel profil oluşturmak çok kullanışlı! 🎯
- **İstatistikler:** Wireshark'ın istatistik bölümü çok detaylı. Trafiğin yoğun olduğu durumlarda buradan genel bir bakış alabilirsin. Ancak bugün çok derinlemesine incelemedim, ileride daha detaylı çalışacağım.

---

#### 📝 Kapanış ve Gelecek Planı
Wireshark ve protokollerle ilgili bugün bolca pratik yaptım. Programın temel mantığını kavradım ama daha karmaşık analizler için ileride daha fazla çalışmam gerekecek. SIEM araçlarında da benzer analizler yapacağımı düşünüyorum. Bu ünite oldukça teorik olsa da, tekrar etmek ve örneklerle çalışmak bilgilerin kalıcı olmasını sağlıyor. Bazen en temel kavramları bile unutabiliyoruz; o yüzden sık sık tekrar etmek çok önemli! 🔄

Bugünkü çalışmam böyle geçti. Herkese bol çalışmalar, sağlıklı günler diliyorum. Esenlikle kalın! 🌟

---
<a id="gun-2025-08-18"></a>
# 🗓️ 18 Ağustos 2025
## Database Fundamentals ve Güvenlik – Temel Bilgiler, Pratikler ve Siber Güvenlik Bağlantısı 🗄️🔒

**Bugünkü Konu:** Veritabanı temelleri (SQL/NoSQL), veritabanı güvenliği, normalizasyon, indeksleme ve sorgu optimizasyonu. Hem teorik hem pratik olarak çalıştım, öğrendiklerimi özetliyorum!

---

### 1️⃣ SQL ve NoSQL Temelleri
- **SQL (Structured Query Language):** İlişkisel veritabanlarında veriler tablo, satır ve sütun şeklinde saklanır. Veri bütünlüğü, tutarlılık ve karmaşık sorgular için idealdir. ACID (Atomicity, Consistency, Isolation, Durability) prensipleriyle çalışır. Büyük şirket uygulamalarında, finans ve ERP sistemlerinde yaygındır.
- **NoSQL:** Esnek şema, yatay ölçeklenebilirlik ve büyük veri işleme için uygundur. JSON belgeler, anahtar-değer, grafik ve sütun tabanlı yapılar sunar. Eventual consistency (zamanla tutarlılık) yaklaşımıyla çalışır. Log analizi, IoT ve gerçek zamanlı uygulamalarda tercih edilir.

**Temel SQL Komutları:**
- `SELECT`: Veri sorgulama
- `WHERE`: Filtreleme
- `AND/OR`: Koşul birleştirme
- `LIKE`: Desen eşleşmesi
- `GROUP BY`: Gruplama
- `COUNT`, `SUM`, `AVG`: Toplama fonksiyonları
- `INSERT`, `UPDATE`, `DELETE`: Veri ekleme, güncelleme, silme

**Pratik:**
SQLite ile örnek bir tablo oluşturdum ve temel komutları çalıştırdım:
```sql
CREATE TABLE ogrenciler (
  id INTEGER PRIMARY KEY,
  ad TEXT,
  soyad TEXT,
  yas INTEGER
);
INSERT INTO ogrenciler (ad, soyad, yas) VALUES ('Ali', 'Yılmaz', 21);
SELECT * FROM ogrenciler WHERE yas > 20;
```
---

### 2️⃣ Database Security Concepts
- **CIA Üçlüsü:**
  - **Confidentiality (Gizlilik):** Verinin yetkisiz erişime karşı korunması. Şifreleme, erişim kontrolleri ve güvenlik duvarları ile sağlanır.
  - **Integrity (Bütünlük):** Verinin doğruluğu ve değişmezliği. Hash algoritmaları, dijital imzalar ve denetim mekanizmaları kullanılır.
  - **Availability (Erişilebilirlik):** Verinin ihtiyaç duyulduğunda erişilebilir olması. Yedekleme, felaket kurtarma ve yüksek erişilebilirlik çözümleri ile sağlanır.
- **Authentication (Kimlik Doğrulama):** Kullanıcıların kimliğinin doğrulanması. Parola, çok faktörlü kimlik doğrulama (MFA), sertifika tabanlı girişler.
- **Authorization (Yetkilendirme):** Kullanıcıya hangi işlemlerin izinli olduğunun belirlenmesi. Rol tabanlı erişim kontrolü (RBAC), yetki matrisleri.
- **SQL Injection:** Zararlı sorgularla veritabanına sızma saldırısı. Parametreli sorgular, input validation ve web uygulama güvenlik duvarı (WAF) ile korunma.
- **Veri Şifreleme:**
  - **At Rest Encryption:** Verinin disk üzerinde şifrelenmesi. AES, TDE gibi teknolojiler.
  - **In Transit Encryption:** Veri aktarımı sırasında şifreleme (ör: TLS/SSL).
  - **Column/Field Encryption:** Hassas alanların ayrı şifrelenmesi. Kredi kartı, kimlik numarası gibi veriler için kullanılır.
- **Backup & Recovery:** Düzenli yedekleme ve acil durumlarda geri yükleme. Tam, artımlı ve diferansiyel yedekleme yöntemleri.
- **Logging & Auditing:** Erişim ve değişikliklerin kaydedilmesi, izlenmesi. Güvenlik olaylarının tespiti ve adli analiz için kritik.
---

### 3️⃣ NoSQL Pratiği ve Farkları
MongoDB ile temel işlemler:
```js
// Belge ekleme
 db.ogrenciler.insertOne({ ad: "Ayşe", soyad: "Kara", yas: 22 })
// Sorgulama
 db.ogrenciler.find({ yas: { $gt: 20 } })
```
NoSQL'de veri genellikle JSON formatında tutulur, şema esnektir. SIEM ve log analizi gibi büyük veri uygulamalarında yaygındır. Yüksek performans, esneklik ve ölçeklenebilirlik sağlar. SQL'den farklı olarak JOIN işlemleri sınırlı veya yoktur, veri genellikle denormalize edilir.



**SQL vs NoSQL Tablosu:**
| Özellik         | SQL (RDBMS)         | NoSQL (MongoDB, Elasticsearch) |
|-----------------|---------------------|-------------------------------|
| Veri Yapısı     | Tablo, satır, sütun | JSON belge, key-value, graph  |
| Şema            | Sabit               | Esnek, dinamik                |
| Ölçeklenebilirlik| Dikey               | Yatay, dağıtık                |
| Tutarlılık      | ACID                | Eventual consistency          |
| Sorgu Dili      | SQL                 | API/JSON                      |
| Kullanım        | Finans, ERP         | Büyük veri, log, IoT          |
---

### 4️⃣ Data Normalization & Indexing
- **Normalizasyon:** Verinin tekrarını azaltmak, tutarlılığı artırmak için tabloyu bölme işlemi. Temel formlar:
  - **1NF (Birinci Normal Form):** Her alan atomik olmalı. Yani bir hücrede birden fazla veri olmamalı.
  - **2NF (İkinci Normal Form):** Tüm alanlar tam anahtara bağlı olmalı. Kısmi bağımlılıklar kaldırılır.
  - **3NF (Üçüncü Normal Form):** Tüm alanlar sadece anahtara bağlı olmalı. Transitif bağımlılıklar kaldırılır.

<img width="721" height="244" alt="normalizyasyon" src="https://github.com/user-attachments/assets/0c4fe5af-02ac-4331-8289-9f33978a3f16" />

- **İndeksleme:** Sorguları hızlandırmak için kullanılır. Büyük tablolarda arama ve sıralama işlemlerini optimize eder.
  - **Primary Index:** Anahtar alan, genellikle benzersizdir.
  - **Unique Index:** Tekil değerler, tekrar eden veri engellenir.
  - **Composite Index:** Birden fazla alanı kapsar, karmaşık sorgularda kullanılır.
  - **Full-text Index:** Metin aramalarında kullanılır, özellikle büyük metin alanlarında hızlı arama sağlar.
SQLite üzerinde test ettim:
---

### 5️⃣ Query Optimization (Sorgu Optimizasyonu)
- Amaç: Sorguların hızlı ve verimli çalışmasını sağlamak. Büyük veri tabanlarında performans kritik önemdedir.
- Yöntemler:
  - İndeks kullanımı ile arama hızlandırılır.
  - `SELECT *` yerine sadece gerekli alanları seçmek, gereksiz veri transferini önler.
  - `WHERE` ile filtreleme, gereksiz satırların sorguya dahil edilmesini engeller.
  - JOIN'leri dikkatli kullanmak, karmaşık sorgularda performans kaybını önler.
  - `LIMIT` ile veri miktarını sınırlamak, özellikle raporlama ve analizde gereksiz yükü azaltır.
  - Normalizasyon/denormalizasyon dengesini kurmak, veri tekrarını ve karmaşıklığı azaltır.
---

### 🏁 Günün Sonucu ve Kapanış
Bugün veritabanı temellerini, güvenlik kavramlarını, SQL ve NoSQL farklarını, normalizasyon ve indeksleme tekniklerini hem teorik hem pratik olarak çalıştım. İleride SIEM ve log analizi gibi konularda bu bilgiler çok işime yarayacak. Pratiklerimi artıracağım!

Herkese bol çalışmalar, sağlıklı günler diliyorum  esenlikle kalın ! 🌟
---

<a id="gun-2025-08-19"></a>
# 🗓️ 19 Ağustos 2025
## Security Operations Center (SOC) – Roller, Süreçler, Senaryolar ve Sürekli İyileştirme 🛡️🔍

Bugün yeni üniteye başladım: Security Operations Center (SOC). Bu ünitede SOC ekiplerinin işleyiş biçimini, rollerini, vardiya ve iletişim prosedürlerini, metrik ve KPI’ları, sürekli iyileştirme süreçlerini senaryolarla ve örneklerle çalıştım. Pratik yapmaya uygun bir konu olmadığı için, teorik bilgileri akılda kalıcı hale getirmek için senaryolaştırdım. 📝

---

### 1️⃣ SOC Roles and Responsibilities (L1, L2, L3) 👨‍💻👩‍💻
- **SOC Nedir?** Bir kurumun siber güvenlik olaylarını merkezi olarak izleyen, analiz eden ve müdahale eden ekip. 🏢
- **Seviye Seviyelendirmesi:**
  - **L1 (Tier 1 – Alert Analyst):** İlk savunma hattı. SIEM ekranını 7/24 izler, gelen alarmları inceler, false positive olup olmadığını kontrol eder. Basit olaylarda ilk aksiyonu alır. 🛡️
    - *Senaryo:* "Failed Login Attempts from Turkey IP" alarmı. L1 kullanıcıya sorar, gerekirse hesabı kilitler ve L2’ye yükseltir. 🔒
  - **L2 (Tier 2 – Incident Responder):** L1’den gelen olayları detaylı araştırır. Network trafiği, endpoint logları inceler, olayın gerçek tehdit olup olmadığını belirler, gerekirse saldırıyı durdurur. 🌐
    - *Senaryo:* L1’den gelen şüpheli login. L2 Wireshark/EDR ile analiz yapar, anormal erişimi tespit eder, hesabı devre dışı bırakır. 🚨
  - **L3 (Tier 3 – Threat Hunter / Expert):** En tecrübeli ekip. Malware analizi, reverse engineering, APT araştırmaları, threat hunting, SIEM kural optimizasyonu, diğer ekipleri eğitme. 🧑‍🔬
    - *Senaryo:* L2 şüpheli dosya bulur, L3 sandbox’ta analiz eder, ransomware olduğunu tespit eder, IOC çıkarır ve SIEM’e kural yazar. 🦠

**📊 Özet Tablo:**
| Seviye |           Görev               |           Örnek Senaryo              |
|--------|-------------------------------|--------------------------------------|
| L1     | Alarm izleme, ilk kontrol     | Anormal login alarmlarını incelemek  |
| L2     | Derin analiz, olay müdahalesi | Tor IP’den login girişini engellemek |
| L3     | İleri analiz, threat hunting  | Ransomware analizi ve IOC çıkarmak   |

---

### 2️⃣ Shift Operations and Handover Procedures 🔄🕒
- **Vardiya Operasyonları:** SOC operasyonları 7/24 devam eder. Analist gelen alarmları izler, yanlış pozitifleri ayıklar, olaylara müdahale eder, dokümantasyon tutar. 📋
- **Handover (Devir Teslim):** Vardiya değişiminde bilgi kaybı olmaması için açık olaylar, alınan ve beklenen aksiyonlar, kritik alarmlar ve iletişim bilgileri yazılı olarak devredilir. 🔗
  - *Senaryo:* Gece analisti, şüpheli login aktivitesi tespit eder, hesabı disable eder, AD logları inceleniyor. Handover’da not bırakır, sabah analisti olayı devralır ve brute-force saldırısını tespit eder. 🌙➡️🌞
- **Ekstra Bilgiler:**
  - Runbook/Playbook: Standart prosedürler. 📑
  - Ticketing System: Jira, ServiceNow, TheHive. 🎫
  - Shift Handover Meeting: Kısa toplantı ile kritik olaylar aktarılır. 👥

---

### 3️⃣ Escalation Procedures and Communication 🚦📞
- **Escalation Nedir?** Olayın mevcut seviyedeki analistin çözüm yetkisini aştığında üst seviyeye veya ilgili ekibe aktarılması. ⬆️
- **Amaç:** Yanlış alarm ile vakit kaybetmemek, kritik olayların doğru kişilere ulaşmasını sağlamak. ⏱️
- **Türler:**
  - Technical Escalation: L1 → L2 → L3. 🧑‍💻➡️🧑‍🔬
  - Hierarchical Escalation: Operasyonel sınır aşıldığında yöneticilere raporlama. 🏢
- **Süreç:** Olayı belirle, ön analiz yap, çözülemiyorsa yükselt, dokümante et, iletişim kurallarına uy. 🗂️
- **İletişim:**
  - Net, sade dil. 🗣️
  - Kanallar: Ticketing, telefon, acil chat. 📱💬
  - Zincir: Önce ilgili seviye, sonra yöneticiler, gerekirse dış ekipler. 🔗
- *Senaryo:* L1, web sunucusunda şüpheli trafik tespit eder, L2’ye escalate eder, L2 credential stuffing bulur, CISO’ya raporlanır. 🌐🚨
- **Ek Bilgiler:**
  - Runbook & Playbook, SLA, iletişim matriksi. 📑⏳

---

### 4️⃣ SOC Metrics & KPIs 📈📊
- **Metric:** Genel ölçüm değeri. Örn: Toplam olay sayısı. 🔢
- **KPI:** Performans göstergesi. Örn: Olay tespit süresi (MTTD), çözüm süresi (MTTR). ⏱️
- **Başlıca Metrics:** Incident count, false positive rate, alarm türleri, detection time, resolution time. 🧮
- **Başlıca KPIs:** MTTD, MTTR, false positive ratio, SLA uyum oranı, incident escalation rate. 🎯
- *Senaryo 1:* MTTD – Saldırı 09:00’da başlıyor, 10:00’da tespit ediliyor → tespit süresi 1 saat. ⏰
- *Senaryo 2:* MTTR – Phishing mail olayı 1 saatte çözülüyor. 📧
- *Senaryo 3:* False Positive – 100 alarmdan 40’ı yanlış, oran %40. 🚫

---

### 5️⃣ Continuous Improvement in SOC Operations 🔁🚀
- **Sürekli İyileştirme:** SOC süreçleri PDCA döngüsüyle sürekli geliştirilir. 🔄
  - Plan: Risk analizi, yeni tehditler, hedef KPI/SLA belirleme. 📝
  - Do: Süreçleri uygula, olaylara müdahale et, yeni playbook ekle. 🛠️
  - Check: KPI/metrik analizi, red/purple team testleri. 📊
  - Act: Eksikleri düzelt, yeni teknik/araç entegre et, eğitim ver. 🎓
- **Yöntemler:** Lessons learned meetings, threat hunting, red/purple team egzersizleri, tool optimization, training & knowledge sharing. 🧑‍🏫🔬

---

Bugünkü bilgileri senaryolarla ve örneklerle aktardım. Teorik bir ünite olduğu için pratik yapma imkanı olmadı, ama senaryolarla akılda kalıcı olmasını sağladım. Umarım faydalı olmuştur.

Herkese bol çalışmalar, sağlıklı günler diliyorum. Esenlikle kalın! 🌟

---

# 🗓️ 20 Ağustos 2025
## Zararlı Yazılım (Malware) Türleri Rehberi 🛡️

Merhaba! Bugün log inceleme ünitesine geçmeden önce, loglarda zararlı yazılımları tespit edebilmek için öncelikle virüs türlerini ve temel malware çeşitlerini öğrenmemiz gerektiğini düşündüm. Çünkü bir zararlının davranışını ve izini bilmeden, loglarda ne arayacağımızı da bilemeyiz. Bu rehberde, siber güvenlik dünyasında en sık karşılaşılan zararlı yazılım türlerini, çalışma prensiplerini, tespit ve korunma yöntemlerini, gerçek hayattan örneklerle birlikte detaylıca ele aldım.

---
<a id="gun-2025-08-20"></a>
## 🦠 Virüsler (Viruses)
### 🧐 Nedir ve Nasıl Çalışır?
Virüsler, adlarını biyolojik benzerlerinden alırlar. Tıpkı bir hücreye sızan biyolojik bir virüs gibi, bilgisayar virüsleri de kendilerini meşru bir programa veya dosyaya "eklerler". Bu "konak" dosya çalıştırıldığında, virüs de aktif hale gelir, kendini kopyalar ve diğer dosyalara bulaşmaya çalışır. Yayılmak için insan etkileşimine (örneğin, bir dosyayı çalıştırmak, bir e-posta ekini açmak) ihtiyaç duyarlar. Virüsler, makro virüsleri (Office belgelerindeki makrolara bulaşır), boot sector virüsleri (bilgisayarın başlangıç disk bölümünü hedef alır) veya polimorfik virüsler (antivirüslerden saklanmak için kodunu sürekli değiştiren gelişmiş virüsler) gibi farklı türlere ayrılabilir.

### 🎬 Gerçek Hayattan Bir Örnek
ILOVEYOU Virüsü (2000): "ILOVEYOU" konu başlığı ve "LOVE-LETTER-FOR-YOU.txt.vbs" adlı bir ek içeren bir e-posta ile yayıldı. Milyonlarca insan merak edip eki açtığında, virüs aktif hale gelerek kullanıcının Outlook adres defterindeki herkese kendini gönderdi ve bilgisayardaki .jpg, .mp3 gibi dosyaları sildi. Bu saldırı, sosyal mühendisliğin ne kadar güçlü olduğunu ve basit bir merak duygusunun küresel bir salgına nasıl yol açabileceğini göstermiştir.

### 🕵️‍♂️ Nasıl Tespit Edilir?
- **İmza Tabanlı Tespit:** Antivirüs yazılımları, bilinen virüslerin benzersiz "parmak izlerini" (imzalarını) içeren bir veritabanına sahiptir. Bir dosyayı taradığında, bu imzalarla eşleşip eşleşmediğini kontrol eder. Bu yöntem hızlı ve etkilidir ancak sadece bilinen tehditleri yakalayabilir.

- **Davranış Analizi (Heuristics):** Bu daha proaktif bir yöntemdir. Antivirüs, bir programın şüpheli davranışlar sergileyip sergilemediğini izler. Örneğin, bir Word belgesinin aniden ağ bağlantısı kurmaya veya sistem dosyalarını değiştirmeye çalışması gibi anormal eylemler, bir makro virüsünün işareti olabilir ve program tarafından engellenir.

- **Belirtiler:** Bilgisayarın belirgin şekilde yavaşlaması, sık sık kilitlenmesi, beklenmedik pop-up'lar, dosyaların bozulması, kaybolması veya dosya boyutlarının anlamsız bir şekilde artması.

### 🛡️ Nasıl Durdurulur ve Korunulur?
- **Antivirüs ve Anti-Malware Yazılımı:** Her zaman güncel bir antivirüs programı kullanın ve düzenli tam sistem taramaları yapın. "Gerçek zamanlı koruma" özelliğinin açık olduğundan emin olun.

- **Şüpheli Ekler ve İndirmeler:** Tanımadığınız kişilerden gelen e-posta eklerini veya güvenilmeyen sitelerden indirilen dosyaları asla açmayın. Dosya uzantılarına dikkat edin; .exe, .vbs, .scr gibi uzantılar özellikle tehlikelidir.

- **İşletim Sistemi ve Yazılım Güncellemeleri:** Yazılımlardaki güvenlik açıklarını kapatmak için tüm güncellemeleri zamanında yapın. Bu, virüslerin sömürebileceği potansiyel giriş noktalarını kapatır.

## 🐛 Solucanlar (Worms)
### 🧐 Nedir ve Nasıl Çalışır?
Solucanlar, virüslerin aksine yayılmak için bir konak dosyaya veya insan etkileşimine ihtiyaç duymazlar. Kendi kendilerine çoğalır ve ağdaki güvenlik açıklarını (örneğin, güncellenmemiş bir yazılım servisi) kullanarak bir bilgisayardan diğerine otomatik olarak yayılırlar. Genellikle ağdaki diğer zayıf makineleri bulmak için port taraması yaparlar. Amaçları genellikle mümkün olduğunca çok sisteme bulaşarak bir botnet oluşturmak, ağ trafiğini felç etmek veya fidye yazılımı gibi başka zararlıları indirmektir.

### 🎬 Gerçek Hayattan Bir Örnek
Stuxnet (2010): Sadece yayılmakla kalmayıp, fiziksel altyapıyı hedef alan ilk siber silahlardan biri olarak kabul edilir. İran'ın nükleer programını hedef alan bu solucan, USB bellekler ve ağ açıkları üzerinden yayılarak, spesifik endüstriyel kontrol sistemlerini (SCADA) aradı. Bu sistemleri bulduğunda, uranyum zenginleştirmede kullanılan santrifüjlerin hızını tehlikeli seviyelerde değiştirerek fiziksel hasara yol açtı.

### 🕵️‍♂️ Nasıl Tespit Edilir?
- **Ağ Trafiği Analizi:** Ağda beklenmedik ve yoğun bir trafik (özellikle SMB portu 445 gibi belirli portlarda) solucan belirtisi olabilir. Güvenlik duvarı (firewall) ve IDS/IPS (Saldırı Tespit/Önleme Sistemleri), bilinen solucanların yayılma modellerini tanıyan imzalara sahiptir ve bu tür anormal trafiği tespit edip engelleyebilir.

- **Davranış Analizi:** Bir sistemin, ağdaki diğer sistemlere sürekli olarak belirli portlardan bağlanmaya çalışması veya rastgele IP adreslerini taraması şüphelidir. EDR çözümleri bu tür davranışları tespit edebilir.

- **Belirtiler:** İnternet bağlantısının ve yerel ağın aşırı yavaşlaması, bilgisayarın fanlarının sürekli yüksek hızda çalışması, güvenlik duvarınızdan gelen çok sayıda giden bağlantı uyarısı.

### 🛡️ Nasıl Durdurulur ve Korunulur?
- **Güvenlik Duvarı (Firewall):** Doğru yapılandırılmış bir güvenlik duvarı, solucanların kullandığı portları kapatarak veya anormal tarama aktivitelerini engelleyerek yayılmasını yavaşlatabilir.

- **Yama Yönetimi (Patch Management):** Solucanlar en çok bilinen ve yaması yayınlanmış güvenlik açıklarını kullandığı için, tüm sistem ve yazılım yamalarını anında uygulamak en etkili korunma yöntemidir. "Yama Salı"larını (Patch Tuesday) takip etmek kritiktir.

- **Ağ Segmentasyonu:** Ağı farklı segmentlere (VLAN'lar gibi) ayırmak, bir solucanın bir segmente bulaşması durumunda diğer kritik segmentlere (örneğin, sunucu ağına) yayılmasını engeller.

## 🐴 Truva Atları (Trojans)
### 🧐 Nedir ve Nasıl Çalışır?
Adını, içine askerlerin gizlendiği ünlü Truva Atı'ndan alır. Truva atları, meşru ve zararsız bir yazılım (örneğin, bir oyun, bir PDF okuyucu, bir sistem temizleme aracı) gibi görünen ancak arka planda kötü amaçlı işler yapan yazılımlardır. Kendi kendilerine yayılmazlar; kullanıcının sosyal mühendislik teknikleriyle kandırılarak onları isteyerek indirip çalıştırması gerekir. Bir kez çalıştığında, saldırgana sisteme bir arka kapı (backdoor) açabilir, onu bir botnet'e dahil edebilir veya fidye yazılımı gibi başka zararlıları indirebilir. RAT (Remote Access Trojan) en tehlikeli türlerinden biridir ve saldırgana kurbanın bilgisayarı üzerinde tam kontrol (kamerasını açma, dosyalarını yönetme vb.) sağlar.

### 🎬 Gerçek Hayattan Bir Örnek
Zeus Trojanı: Bankacılık bilgilerini çalmak için tasarlanmış en ünlü Truva atlarından biridir. Kullanıcılar meşru görünümlü bir yazılım indirdiğinde, Zeus arka planda çalışarak kullanıcı banka sitesine girdiğinde tuş vuruşlarını kaydeder (keylogging) veya tarayıcıya sahte bir giriş ekranı enjekte ederek kimlik bilgilerini çalar. Bu, "Man-in-the-Browser" saldırısının klasik bir örneğidir.

### 🕵️‍♂️ Nasıl Tespit Edilir?
- **Antivirüs Taramaları:** İyi bir antivirüs, bilinen Truva atlarının imzalarını tanıyabilir.

- **Ağ İzleme:** Bilgisayarınızın, siz farkında olmadan bilinmeyen veya şüpheli bir sunucuya (Komuta & Kontrol sunucusu) sürekli veri gönderdiğini fark ederseniz, bu bir Truva atı belirtisi olabilir. Wireshark gibi araçlarla bu trafik incelenebilir.

- **Endpoint Detection and Response (EDR):** EDR çözümleri, bir programın normal davranışının dışına çıktığını (örneğin, svchost.exe gibi meşru bir Windows işleminin içine kod enjekte etmesi) tespit edebilir.

### 🛡️ Nasıl Durdurulur ve Korunulur?
- **Güvenilir Kaynaklar:** Sadece resmi ve güvenilir web sitelerinden veya uygulama mağazalarından yazılım indirin. Korsan yazılımlar ve "crack" dosyaları en yaygın Truva atı kaynaklarıdır.

- **E-posta Dikkat:** "Faturanız ektedir" veya "Kargo takip numaranız" gibi görünen sahte e-postalardaki eklere karşı son derece dikkatli olun.

- **Kullanıcı Hesabı Denetimi (UAC):** Windows'taki UAC gibi mekanizmalar, bir program yönetici hakları istediğinde sizi uyarır. Ne kurduğunuzdan emin değilseniz asla izin vermeyin.

## 💸 Fidye Yazılımları (Ransomware)
### 🧐 Nedir ve Nasıl Çalışır?
Fidye yazılımları, günümüzün en tehlikeli ve en kârlı zararlı yazılım türüdür. Bir sisteme bulaştığında, kullanıcının kişisel dosyalarını (fotoğraflar, belgeler, veritabanları) güçlü bir şifreleme algoritmasıyla (genellikle AES veya RSA) şifreler ve dosyaları açamaz hale getirir. Ardından, dosyaları geri getirecek olan şifre çözme anahtarı (decryption key) için kullanıcıdan genellikle kripto para (Bitcoin vb.) ile fidye talep eder. Modern saldırganlar artık "çifte şantaj" (double extortion) taktiğini kullanmaktadır: Dosyaları şifrelemeden önce hassas verileri kendi sunucularına kopyalarlar ve kurban fidyeyi ödemezse verileri internette yayınlamakla tehdit ederler.

### 🎬 Gerçek Hayattan Bir Örnek
WannaCry (2017): Windows'taki EternalBlue adlı bir güvenlik açığını kullanarak (solucan gibi) yayıldı ve dünya çapında yüz binlerce bilgisayarı etkiledi. Hastaneler, şirketler ve kamu kurumları dahil olmak üzere birçok sistemi kilitledi ve dosya başına 300-600 dolar fidye talep etti. Bu saldırı, yamanın yayınlanmış olmasına rağmen uygulanmamasının ne kadar yıkıcı sonuçlara yol açabileceğini acı bir şekilde göstermiştir.

### 🕵️‍♂️ Nasıl Tespit Edilir?
- **Davranış Analizi:** Bir işlemin kısa sürede binlerce dosyayı okuyup, şifreleyip, yeniden yazması tipik bir fidye yazılımı davranışıdır. Modern güvenlik yazılımları (EDR, XDR) bu anormal dosya aktivitesini tespit ederek işlemi anında sonlandırabilir.

- **"Canary" Dosyaları / Honeypot'lar:** Sistemin belirli yerlerine, içinde anlamsız veriler olan "kanarya" dosyaları veya sahte ağ paylaşımları yerleştirilir. Eğer bu dosyalarda bir değişiklik (şifrelenme) tespit edilirse, fidye yazılımı saldırısı olduğu anlaşılır ve süreç otomatik olarak durdurulur.

- **Fidye Notu:** En bariz belirti, masaüstünde beliren ve dosyalarınızın şifrelendiğini, fidyeyi nasıl ödeyeceğinizi anlatan bir metin dosyası (DECRYPT_ME.txt gibi) veya duvar kağıdıdır.

### 🛡️ Nasıl Durdurulur ve Korunulur?
- **YEDEKLEME (3-2-1 Kuralı)!** En etkili savunma budur. Verilerinizin 3 kopyasını, 2 farklı medya türünde saklayın ve bu kopyalardan 1 tanesi mutlaka çevrimdışı (ağa bağlı olmayan) veya değiştirilemez (immutable) bir ortamda olsun. Böylece dosyalarınız şifrelense bile yedeğinizden geri dönebilirsiniz.

- **E-posta Güvenliği:** Fidye yazılımlarının en yaygın bulaşma yolu phishing e-postalarıdır. Gelişmiş e-posta güvenlik çözümleri kullanın ve kullanıcıları şüpheli eklere ve linklere asla tıklamamaları konusunda eğitin.

- **En Az Yetki Prensibi (Principle of Least Privilege):** Günlük işlerinizi yönetici (admin) hesabıyla yapmayın. Standart bir kullanıcı hesabı, fidye yazılımının tüm sisteme yayılmasını ve kritik sistem dosyalarını şifrelemesini zorlaştırabilir.

## 🕵️‍♂️ Casus Yazılımlar (Spyware) ve Keylogger'lar
### 🧐 Nedir ve Nasıl Çalışır?
Casus yazılımlar, adından da anlaşılacağı gibi, kullanıcının haberi olmadan sisteme sızar ve gizlice bilgi toplar. Topladığı bilgiler arasında internet gezinti alışkanlıkları, e-posta adresleri, kullanıcı adları ve parolalar olabilir. Keylogger'lar ise casus yazılımların özel bir türüdür ve klavyede bastığınız her tuşu kaydederek kredi kartı bilgileri, şifreler gibi en hassas verileri çalmayı hedefler. Adware ise genellikle casus yazılımlarla birlikte gelir ve amacı sürekli olarak istenmeyen reklamlar göstermektir.

### 🎬 Gerçek Hayattan Bir Örnek
CoolWebSearch (CWS): Bir tarayıcı eklentisi veya küçük bir program gibi görünen bu casus yazılım, kullanıcının tarayıcı anasayfasını değiştirir, arama sonuçlarını kendi sitelerine yönlendirir ve sürekli olarak rahatsız edici pop-up'lar çıkarırdı. Amacı, reklam geliri elde etmek ve kullanıcı verilerini toplamaktı. Bu tür yazılımlar genellikle "Potansiyel Olarak İstenmeyen Programlar" (PUPs) olarak sınıflandırılır.

### 🕵️‍♂️ Nasıl Tespit Edilir?
- **Anti-Spyware Araçları:** Birçok modern antivirüs, casus yazılımları da tespit edebilen modüllere sahiptir. Malwarebytes gibi özel araçlar bu konuda oldukça etkilidir.

- **Ağ Trafiği:** Bilgisayarınızın siz bir şey yapmazken bile sürekli olarak şüpheli bir reklam sunucusuna veya veri toplama sunucusuna veri gönderdiğini görmek bir belirtidir.

- **Belirtiler:** Tarayıcı anasayfanızın veya arama motorunuzun kendi kendine değişmesi ve bunu düzeltememeniz, sistem performansında ani düşüşler, internette gezinirken her yerde karşınıza çıkan beklenmedik reklam pencereleri.

### 🛡️ Nasıl Durdurulur ve Korunulur?
- **Dikkatli Kurulum:** Ücretsiz yazılımlar kurarken "Hızlı Kurulum" yerine "Özel Kurulum" seçeneğini tercih edin. Bu sırada size "ekstra" olarak sunulan tarayıcı araç çubuklarını veya istenmeyen programları kurmayı reddeden kutucukların işaretini kaldırın.

- **Pop-up Engelleyiciler:** Tarayıcınızın pop-up engelleyicisini aktif tutun ve güvenilir bir reklam engelleyici (ad-blocker) eklentisi kullanın.

- **Güvenlik Yazılımı:** Düzenli olarak güncel bir güvenlik yazılımıyla tarama yapın ve şüpheli tarayıcı eklentilerini kaldırın.

## 🤖 Botnet'ler
### 🧐 Nedir ve Nasıl Çalışır?
Botnet, "robot" ve "network" kelimelerinin birleşimidir. Bir saldırgan (botmaster), genellikle solucanlar veya Truva atları aracılığıyla binlerce, hatta milyonlarca bilgisayara sızar. Bu ele geçirilmiş bilgisayarlara "zombi" denir ve hepsi, saldırganın merkezi bir Komuta ve Kontrol (C&C veya C2) sunucusundan gönderdiği komutları bekler. Saldırgan, bu devasa zombi ordusunu DDoS saldırıları, spam e-posta kampanyaları, kripto para madenciliği veya tıklama sahtekarlığı (click fraud) gibi büyük çaplı ve yasa dışı faaliyetler için kullanır.

### 🎬 Gerçek Hayattan Bir Örnek
Mirai Botneti (2016): Güvenliği zayıf olan IoT (Nesnerin İnterneti) cihazlarını (güvenlik kameraları, modemler, DVR'lar vb.) hedef aldı. Fabrika ayarı şifrelerini ("admin/admin" gibi) deneyerek yüz binlerce cihaza sızdı ve devasa bir botnet oluşturdu. Bu botnet, tarihin en büyük DDoS (Distributed Denial of Service) saldırılarından bazılarını gerçekleştirmek için kullanıldı ve Twitter, Netflix, Reddit gibi büyük siteleri saatlerce erişilmez hale getirdi.

### 🕵️‍♂️ Nasıl Tespit Edilir?
- **Ağ Anormallikleri:** Cihazınızın, bilginiz dışında şüpheli bir C&C sunucusuna bağlanmaya çalışması (genellikle IRC portları 6667, özel portlar veya bazen gizlenmek için DNS portu 53 üzerinden) en önemli belirtidir. Güvenlik duvarı logları ve NetFlow verileri bu tespitte yardımcı olabilir.

- **DDoS Trafiği:** Bilgisayarınızın veya ağınızın, belirli bir hedefe doğru anlamsız ve yoğun bir ağ trafiği (UDP/ICMP flood) göndermesi, bir DDoS saldırısının parçası olduğunuzu gösterir.

- **Anti-Malware Taramaları:** Botnet'e dahil olmanızı sağlayan zararlı yazılımı (bot istemcisini) tespit edebilir.

### 🛡️ Nasıl Durdurulur ve Korunulur?
- **Güçlü ve Benzersiz Şifreler:** Özellikle modem, kamera gibi IoT cihazlarınızın varsayılan şifrelerini mutlaka değiştirin. Her cihaz için farklı ve karmaşık bir şifre kullanın.

- **Yazılım ve Firmware Güncellemeleri:** Cihazlarınızın firmware (donanım yazılımı) güncellemelerini düzenli olarak yapın. Üreticiler genellikle bilinen güvenlik açıklarını bu güncellemelerle kapatır.

- **Genel Korunma Yöntemleri:** Bir botnet'e dahil olmanızı sağlayan şey genellikle bir solucan veya Truva atıdır. Dolayısıyla onlardan korunma yöntemleri botnet'lerden de korunmanızı sağlar.

---

Bugünkü rehberde, en çok karşılaşabileceğimiz ve loglarda tespit etmemiz gereken zararlı yazılım türlerini özetledim. İleride daha az bilinen veya özel malware türleriyle ilgili kısa bilgiler de ekleyebilirim. Umarım bu rehber, hem log analizlerinde hem de genel siber güvenlik çalışmalarında size yol gösterici olur. Herkese bol çalışmalar, sağlıklı günler dilerim. Esenlikle kalın! 🌟

---
