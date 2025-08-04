# Muzaffer'in Mavi Takım (Blue Team) Yolculuğu 🛡️

## Merhaba! 👋

Ben Muzaffer, Bilgisayar Programcılığı öğrencisiyim ve siber güvenlik dünyasına tutkuyla bağlıyım. 👨‍💻 Bu alana olan ilgim bir süredir devam etse de, öğrenme sürecimde daha yapılandırılmış ve disiplinli bir yaklaşıma ihtiyaç duyduğumu fark ettim.

## Bu Depo (Repository) Nedir? 🗺️

Bu depo, benim siber güvenlik serüvenimin canlı bir günlüğüdür. İnternette yaptığım detaylı araştırmalar sonucunda, "Daarin" tarafından Medium'da hazırlanan kapsamlı **[Blue Team Yol Haritası](https://medium.com/@daarin/roadmap-for-cyber-security-in-the-blue-team-ae9b25721ac2)** ile karşılaştım. Bu yol haritasının detay seviyesi ve mantıksal yapısı, kendimi geliştirmek için izlemek istediğim yolun tam olarak bu olduğuna karar vermemi sağladı. ✅

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

- [4 Ağustos 2025: Laboratuvar Kurulumu ve İlk Domain Macerası](#️-4-ağustos-2025-laboratuvar-kurulumu-ve-ilk-domain-macerası)
- *(Yeni günlük eklendiğinde buraya bir satır daha eklenecek...)*

---

## 🚀 Günlükler Başlıyor!

### 4 Ağustos 2025: Laboratuvar Kurulumu ve İlk Domain Macerası

**Bugünkü Konu:** Blue Team laboratuvar ortamının hazırlanması. 🧪

#### Günün Özeti

Bugün, teorik bilgileri pratiğe dökebileceğim sanal laboratuvar ortamımı hazırlamaya odaklandım. Microsoft Learn koleksiyonuna başlamadan önce, üzerinde çalışacağım sistemlerin hazır ve birbirleriyle iletişim kurabilir halde olması kritikti. Bu süreç, beklediğimden daha fazla sorun giderme pratiği içerdi ve harika bir öğrenme deneyimi oldu! 💪

#### Yapılan İşlemler ve Öğrenilenler 🤓

1.  **Sanallaştırma Platformu: VirtualBox** 📦
    Her şeyden önce, izole ve güvenli bir çalışma alanı oluşturmak için Oracle VirtualBox'ı kurdum. Sanallaştırma, tek bir fiziksel makine üzerinde birden çok işletim sistemini aynı anda çalıştırmamızı sağlar. Bu, farklı sistemlerin birbiriyle nasıl etkileşime girdiğini görmek ve hata yapmaktan korkmadan denemeler yapmak için mükemmel bir yöntem.

2.  **Sanal Makinelerin Kurulumu** 🖥️
    - **Windows Server 2016:** Laboratuvarımın merkezi olacak olan sunucu. Domain Controller (Etki Alanı Yöneticisi), DNS ve diğer temel servisleri bu sunucu üzerinde yapılandıracağım.
    - **Windows 10:** Sunucu tarafından yönetilecek olan standart bir istemci (client) makinesi. Yaptığım politika değişikliklerinin ve güvenlik ayarlarının etkilerini bu makine üzerinden gözlemleyeceğim.

3.  **Ağ Yapılandırması: En Kritik Adım!** 🌐
    Sanal makinelerin birbiriyle konuşabilmesi için doğru ağ yapılandırması şarttır. Her iki sanal makine için de ikişer ağ bağdaştırıcısı tanımladım:
    - **Bağdaştırıcı 1: NAT (Network Address Translation):** Bu bağdaştırıcı, sanal makinelerin ana makinem üzerinden internete çıkabilmesini sağlar. Bu sayede gerekli güncellemeleri ve indirmeleri yapabilirim. 🌍
    - **Bağdaştırıcı 2: Dahili Ağ (Internal Network):** Bu bağdaştırıcı, iki sanal makinenin dış dünyadan izole, kendi özel ağlarında haberleşmesi için kullanıldı. İkisine de aynı "intnet" ismini verdim. Bu, gerçek bir şirket içi ağı simüle etmemi sağlıyor. 🔒

4.  **Statik IP Adreslemesi ve DNS** ✍️
    - **Windows Server 2016 IP Ayarları:**
        - IP Adresi: `192.168.100.10`
        - Alt Ağ Maskesi: `255.255.255.0`
        - DNS Sunucusu: `192.168.100.10` (Kendisi)
        - **Öğrenilen Bilgi 💡:** Bir Domain Controller, aynı zamanda DNS sunucusu olarak da hizmet verir. Bu yüzden DNS olarak kendi IP adresini göstermesi gerekir ki ağdaki diğer makineler domain'i ve diğer kaynakları ismiyle bulabilsin.
    - **Windows 10 IP Ayarları:**
        - IP Adresi: `192.168.100.20`
        - Alt Ağ Maskesi: `255.255.255.0`
        - DNS Sunucusu: `192.168.100.10` (Server'ın IP'si)
        - **Öğrenilen Bilgi 💡:** İstemci makinenin domain'e katılabilmesi için DNS sunucusu olarak Domain Controller'ın IP adresini bilmesi zorunludur. Aksi takdirde, "contoso.local" gibi bir domain isminin hangi IP adresine karşılık geldiğini çözemez.

#### Karşılaşılan Sorun ve Çözüm: "AD DC Could Not Be Connected" 🤯
Her şey hazır gibiydi. Windows 10 makinesini `CLIENT01` olarak yeniden adlandırdım ve domain'e dahil etmeye çalıştığımda o meşhur hatayı aldım: **"An Active Directory Domain Controller for the domain could not be contacted."**

Ping testinde Windows 10'dan sunucuya ping gidebiliyorken, sunucudan Windows 10'a ping gitmemesi ilk ipucuydu. Kısa bir araştırma ve yapay zekaya danışma sonucunda suçlunun **Windows Güvenlik Duvarı (Firewall)** 🔥 olduğunu anladım.

**Çözüm (Geçici) ✅:** Sorunu hızlıca aşmak için Windows Server üzerindeki güvenlik duvarını geçici olarak tamamen kapattım. Ve BINGO! 🎉 Windows 10 makinesi sorunsuz bir şekilde domain'e katıldı.

**Profesyonel İpucu ve Gelecek Notu 📝:** Gerçek bir ortamda güvenlik duvarını tamamen kapatmak **asla** yapılmaması gereken bir şeydir. Doğru yöntem, domain'e katılım için gerekli olan spesifik portlara (DNS, RPC, SMB vb.) güvenlik duvarı üzerinden izin vermektir. Bu konuyu ilerleyen günlerde detaylıca araştırıp doğru kural setini oluşturacağım.

#### Günün Sonucu ve Sonraki Adımlar 🏁
Laboratuvarım artık hazır! Bu temel kurulum, yol haritamdaki pratik uygulamalar için sağlam bir zemin oluşturdu. Artık gönül rahatlığıyla **[Microsoft Learn Windows Server 2019 Koleksiyonu](https://learn.microsoft.com/tr-tr/collections/5x1du7p537reex?WT.mc_id=modinfra-13564-socuff)**'na başlayabilirim!

---