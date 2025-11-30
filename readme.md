# chickOS Helper - Yapılan İşlemler Detaylı Açıklama
## 📋 İçindekiler

1. [Sistem Tweaks](#sistem-tweaks)
2. [Bloatware Kaldırma](#bloatware-kaldırma)
3. [Bileşen Kaldırma](#bileşen-kaldırma)

---

## 🔧 Sistem Tweaks

### Registry Ayarları

#### Explorer ve Başlat Menüsü
| Ayar | Değer | Açıklama |
|------|-------|----------|
| Start_TrackProgs | 0 | Sık kullanılan program takibini devre dışı bırakır |
| Start_TrackDocs | 0 | Son açılan belge takibini devre dışı bırakır |
| Start_IrisRecommendations | 0 | Başlat menüsü önerilerini devre dışı bırakır |
| LaunchTo | 1 | Dosya Gezgini'ni "Bu Bilgisayar" olarak açar |
| HubMode | 1 | Hızlı erişimi devre dışı bırakır |

#### Görev Çubuğu
| Ayar | Değer | Açıklama |
|------|-------|----------|
| SearchboxTaskbarMode | 3 | Arama kutusunu simge olarak gösterir |
| TaskbarNotification | 0 | Görev çubuğu bildirimlerini devre dışı bırakır |

#### Telemetri ve Gizlilik
| Ayar | Değer | Açıklama |
|------|-------|----------|
| AllowTelemetry | 0 | Windows telemetrisini devre dışı bırakır |
| DoNotShowFeedbackNotifications | 1 | Geri bildirim bildirimlerini kapatır |
| BingSearchEnabled | 0 | Başlat menüsü Bing aramasını devre dışı bırakır |
| DisableWebSearch | 1 | Web aramasını devre dışı bırakır |
| TailoredExperiencesWithDiagnosticDataEnabled | 0 | Kişiselleştirilmiş deneyimleri devre dışı bırakır |
| AdvertisingInfo | 0 | Reklam kimliğini devre dışı bırakır |

#### Windows Spotlight ve İçerik Teslimi
| Ayar | Değer | Açıklama |
|------|-------|----------|
| SystemPaneSuggestionsEnabled | 0 | Sistem önerilerini devre dışı bırakır |
| SoftLandingEnabled | 0 | Uygulama önerilerini devre dışı bırakır |
| RotatingLockScreenEnabled | 0 | Dönen kilit ekranı resimlerini devre dışı bırakır |
| SubscribedContentEnabled | 0 | Abone olunan içeriği devre dışı bırakır |

#### Performans Ayarları
| Ayar | Değer | Açıklama |
|------|-------|----------|
| Win32PrioritySeparation | 0x26 | İşlemci zamanlamasını optimize eder |
| KeyboardDataQueueSize | 0x32 | Klavye arabellek boyutunu artırır |
| MouseDataQueueSize | 0x32 | Fare arabellek boyutunu artırır |
| SystemResponsiveness | 1 | Sistem yanıt hızını optimize eder |
| MenuShowDelay | 0 | Menü açılma gecikmesini kaldırır |

#### Oyun Optimizasyonları
| Ayar | Değer | Açıklama |
|------|-------|----------|
| AutoGameModeEnabled | 1 | Otomatik oyun modunu etkinleştirir |
| GPU Priority | 8 | Oyunlar için GPU önceliğini artırır |
| Scheduling Category | High | Oyunlar için yüksek zamanlama önceliği |
| SFIO Priority | High | Oyunlar için yüksek I/O önceliği |

#### Güç Yönetimi
| Ayar | Değer | Açıklama |
|------|-------|----------|
| HiberbootEnabled | 0 | Hızlı başlatmayı devre dışı bırakır (daha temiz başlangıç) |
| USB selective suspend | 0 | USB güç tasarrufunu devre dışı bırakır |
| PCI Express ASPM | 0 | PCIe güç tasarrufunu devre dışı bırakır |

### Devre Dışı Bırakılan Servisler

| Servis | Açıklama |
|--------|----------|
| WSearch | Windows Search - Dosya dizinleme servisi |
| SysMain | Superfetch - Önceden yükleme servisi |
| WerSvc | Windows Hata Raporlama |
| DiagTrack | Bağlı Kullanıcı Deneyimleri ve Telemetri |

### Devre Dışı Bırakılan Zamanlanmış Görevler

- Dil Senkronizasyonu
- Dil Bileşenleri Yükleyicisi
- Windows Aktivasyon Doğrulama
- WinSAT Performans Testi
- Konuşma Modeli İndirme

### Kaldırılan Windows Özellikleri

| Özellik | Açıklama |
|---------|----------|
| DirectoryServices-ADAM-Client | AD LDS istemcisi |
| OneCoreUAP-OneSync | OneSync senkronizasyon |
| Hello-Face | Windows Hello yüz tanıma |
| MathRecognizer | Matematik tanıyıcı |
| OpenSSH-Client | OpenSSH istemcisi |
| WindowsMediaPlayer | Windows Media Player |
| Microsoft-Windows-PowerShell-ISE | PowerShell ISE |
| WorkFolders-Client | Çalışma Klasörleri istemcisi |

### Güç Planı

- **Aktif Plan:** Yüksek Performans
- **Ekran Kapanma:** Devre dışı
- **Uyku:** Devre dışı
- **USB Selective Suspend:** Devre dışı
- **PCI Express ASPM:** Devre dışı

---

## 🗑️ Bloatware Kaldırma

### Kaldırılan Uygulamalar

#### Microsoft Uygulamaları
| Uygulama | Paket Adı |
|----------|-----------|
| Microsoft Edge | Edge (setup.exe ile) |
| OneDrive | OneDriveSetup /uninstall |
| Windows Copilot | MicrosoftWindows.Client.AIX |
| Microsoft Teams | MicrosoftTeams / MSTeams |
| Outlook (Yeni) | Microsoft.OutlookForWindows |
| Solitaire Collection | Microsoft.MicrosoftSolitaireCollection |
| Clipchamp | clipchamp.clipchamp |
| Feedback Hub | Microsoft.Windows.FeedbackHub |
| Microsoft Family | MicrosoftCorporationII.MicrosoftFamily |

#### Bing Uygulamaları
| Uygulama | Paket Adı |
|----------|-----------|
| Bing News | Microsoft.BingNews |
| Bing Weather | Microsoft.BingWeather |
| Bing Search | Microsoft.BingSearch |

#### Medya Uygulamaları
| Uygulama | Paket Adı |
|----------|-----------|
| Groove Music | Microsoft.ZuneMusic |
| Movies & TV | Microsoft.ZuneVideo |
| Camera | Microsoft.WindowsCamera |
| Photos | Microsoft.Windows.Photos |
| Voice Recorder | Microsoft.Windows.SoundRecorder |

#### Xbox Uygulamaları
| Uygulama | Paket Adı |
|----------|-----------|
| Xbox App | Microsoft.GamingApp |
| Xbox Game Bar | Microsoft.XboxGamingOverlay |
| Xbox TCUI | Microsoft.Xbox.TCUI |
| Xbox Console Companion | Microsoft.XboxApp |
| Xbox Identity | Microsoft.XboxIdentityProvider |
| Xbox Speech | Microsoft.XboxSpeechToTextOverlay |

#### Diğer Uygulamalar
| Uygulama | Paket Adı |
|----------|-----------|
| Microsoft To Do | Microsoft.Todos |
| Power Automate | Microsoft.PowerAutomateDesktop |
| Sticky Notes | Microsoft.MicrosoftStickyNotes |
| Get Help | Microsoft.GetHelp |
| Tips | Microsoft.Getstarted |
| Remote Desktop | Microsoft.RemoteDesktop |
| Alarms & Clock | Microsoft.WindowsAlarms |
| Windows Terminal | Microsoft.Windows.Terminal |
| Phone Link | Microsoft.YourPhone |
| Maps | Microsoft.WindowsMaps |
| People | Microsoft.People |
| Mail & Calendar | Microsoft.WindowsCommunicationsApps |
| Skype | Microsoft.SkypeApp |
| Mixed Reality Portal | Microsoft.MixedReality.Portal |
| Cortana | Microsoft.549981C3F5F10 |
| LinkedIn | Microsoft.LinkedIn |

### Temizlenen Kısayollar

- Masaüstü Edge kısayolları
- Başlat menüsü kısayolları
- Görev çubuğu pinleri
- Start Menu önbelleği

---

## ⚙️ Bileşen Kaldırma

### Windows Özellikleri (DISM)

| Özellik | Açıklama |
|---------|----------|
| Internet-Explorer-Optional-amd64 | Internet Explorer |
| WindowsMediaPlayer | Windows Media Player |
| Microsoft-Windows-PowerShell-ISE | PowerShell ISE |
| WorkFolders-Client | Çalışma Klasörleri istemcisi |
| TFTP-Client | TFTP İstemcisi |
| SMB-Direct | SMB Direct |

### Windows Yetenekleri

| Yetenek | Açıklama |
|---------|----------|
| MathRecognizer | Matematik tanıyıcı |
| Microsoft.Windows.WordPad | WordPad |

### Devre Dışı Bırakılan Servisler

| Servis | Görünen Ad | Açıklama |
|--------|-----------|----------|
| WSearch | Windows Search | Dosya dizinleme |
| WerSvc | Windows Error Reporting | Hata raporlama |
| DiagTrack | Connected User Experiences | Telemetri |
| RemoteRegistry | Remote Registry | Uzak kayıt defteri erişimi |
| WinRM | Windows Remote Management | Uzaktan yönetim |
| WbioSrvc | Windows Biometric Service | Biyometrik hizmet |
| PhoneSvc | Phone Service | Telefon servisi |
| WpnService | Windows Push Notifications | Anlık bildirimler |
| MapsBroker | Downloaded Maps Manager | Harita yöneticisi |
| lfsvc | Geolocation Service | Konum servisi |
| RetailDemo | Retail Demo Service | Mağaza demo modu |
| wisvc | Windows Insider Service | Insider programı |
| SharedAccess | Internet Connection Sharing | Bağlantı paylaşımı |
| dmwappushservice | Device Management WAP Push | Cihaz yönetimi |

### Kaldırılan/Devre Dışı Bırakılan Zamanlanmış Görevler

| Kategori | İşlem |
|----------|-------|
| Customer Experience Improvement | Kaldırıldı |
| Application Experience | Devre dışı |
| Feedback | Devre dışı |
| Maps | Devre dışı |
| Windows Error Reporting | Devre dışı |
| Edge Update | Kaldırıldı |
| Telemetry | Devre dışı |
| DiagTrack | Devre dışı |

### Registry Tweaks

| Kategori | Ayar |
|----------|------|
| Cortana | Devre dışı |
| Web Search | Devre dışı |
| Telemetry | 0 (Kapalı) |
| Windows Copilot | Devre dışı |
| Edge Updates | Devre dışı |
| Advertising ID | Devre dışı |
| Consumer Features | Devre dışı |
| Cloud Content | Devre dışı |

### Edge Update Servisi

- `edgeupdate` servisi durduruldu ve devre dışı bırakıldı
- `edgeupdatem` servisi durduruldu ve devre dışı bırakıldı
- EdgeUpdate klasörü kaldırıldı
- Edge Update zamanlanmış görevleri kaldırıldı

### Ek Appx Paketleri

| Paket | Açıklama |
|-------|----------|
| Video Extensions (AV1, HEVC, MPEG2, VP9) | Video codec'leri |
| Microsoft.BioEnrollment | Windows Hello kurulumu |
| Microsoft.ECApp | Göz kontrolü |
| Microsoft.Windows.ContentDeliveryManager | İçerik teslim yöneticisi |
| Microsoft.Windows.DevHome | Dev Home |
| Microsoft.Windows.ParentalControls | Ebeveyn denetimleri |
| Microsoft.Windows.PeopleExperienceHost | Kişiler deneyimi |
| MicrosoftWindows.CrossDevice | Cihazlar arası deneyim |
| Windows.CBSPreview | Barkod önizleme |
| Microsoft.Services.Store.Engagement | Store etkileşim |
| Microsoft.MicrosoftOfficeHub | Microsoft 365 hub |

---

## ⚠️ Önemli Notlar

1. **Geri Yükleme:** Kaldırılan uygulamalar Microsoft Store'dan tekrar yüklenebilir.
2. **Edge:** Microsoft Edge'i geri yüklemek için [microsoft.com/edge](https://microsoft.com/edge) adresini ziyaret edin.
3. **Yeniden Başlatma:** Tüm değişikliklerin etkili olması için bilgisayarınızı yeniden başlatmanız önerilir.
4. **Windows Update:** Bazı bileşenler Windows Update ile geri yüklenebilir.

