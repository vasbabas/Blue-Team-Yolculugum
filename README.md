# Muzaffer'in Mavi Takım (Blue Team) Yolculuğu 🛡️

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
- *(Yeni günlük eklendiğinde buraya bir satır daha eklenecek...)*

---

## 🚀 Günlükler Başlıyor!
<a id="gun-2025-08-04"></a>
### 🗓️ 4 Ağustos 2025: Laboratuvar Kurulumu ve İlk Domain Macerası

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

---
<a id="gun-2025-08-05"></a>
### 🗓️ 5 Ağustos 2025: Active Directory'nin Kalbine İniyoruz: OU, Kullanıcılar ve İzinler

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

Yarınki hedefim, Windows Server serüvenini GPO (Grup İlke Nesneleri) ile daha derinlemesine inceleyerek tamamlamak. İyi akşamlar! 😊

---
<a id="gun-2025-08-06"></a>

### 🗓️ 6 Ağustos 2025: GPO ile İmparatorluğun Kurallarını Yazmak
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

Umarım yarın Windows Server ile ilgili son konuları da tamamlayıp bu ilk büyük adımı bitirebilirim. Bu yolculukta bana eşlik eden herkese bol çalışmalar dilerim! 😊

---
<a id="gun-2025-08-07"></a>

### 🗓️ 7 Ağustos 2025: Windows Server'da Ustalığa Son Adım: DNS, DHCP ve Ötesi
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

Sıradaki büyük macera, Linux yönetimi! İleriki çalışmalarda görüşmek üzere! 🚀
