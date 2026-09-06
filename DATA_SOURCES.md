# Veri kaynakları ve kaynakça açıklaması

Bu not, 20 Haziran 2026 tarihli proje raporunun veri kaynaklarını dosya bazında açıklar. Raporun özgün 65 sayfalık PDF'si korunmuştur; aşağıdaki açıklama PDF ile birlikte okunmalıdır.

## 1. NAB kaynaklı zaman serileri

Aşağıdaki beş dosya, **Numenta Anomaly Benchmark (NAB)** koleksiyonunda yayımlanmıştır. NAB veri açıklaması, ilgili grupları AWS/CloudWatch kaynaklı sistem metrikleri olarak tanımlar.

| Projede kullanılan dosya | Özgün kaynak |
| --- | --- |
| `cpu_utilization_asg_misconfiguration.csv` | [NAB / realKnownCause](https://github.com/numenta/NAB/blob/master/data/realKnownCause/cpu_utilization_asg_misconfiguration.csv) |
| `ec2_request_latency_system_failure.csv` | [NAB / realKnownCause](https://github.com/numenta/NAB/blob/master/data/realKnownCause/ec2_request_latency_system_failure.csv) |
| `ec2_disk_write_bytes_1ef3de.csv` | [NAB / realAWSCloudwatch](https://github.com/numenta/NAB/blob/master/data/realAWSCloudwatch/ec2_disk_write_bytes_1ef3de.csv) |
| `ec2_network_in_257a54.csv` | [NAB / realAWSCloudwatch](https://github.com/numenta/NAB/blob/master/data/realAWSCloudwatch/ec2_network_in_257a54.csv) |
| `elb_request_count_8c0756.csv` | [NAB / realAWSCloudwatch](https://github.com/numenta/NAB/blob/master/data/realAWSCloudwatch/elb_request_count_8c0756.csv) |

[NAB veri açıklaması](https://github.com/numenta/NAB/blob/master/data/README.md) · [NAB deposu](https://github.com/numenta/NAB)

Bu eşleştirme, raporda belirtilen dosya adları ve NAB koleksiyonuyla yapılmıştır. Yerel işlenmiş dosyaların özgün dosyalarla birebir aynı olduğu veya kullanılan tarihsel sürümün hangi commit olduğu iddia edilmemektedir.

## 2. Raporun kaynakçasına açıklama

PDF'nin **50 numaralı sayfasında (dosyanın 58. sayfası)** bulunan “Uzkal, Ö. F. (2026). Proje kapsamında kullanılan CSV veri dosyaları [Veri seti]” kaydı, proje içinde kullanılan dosyaların bir envanteri olarak değerlendirilmelidir. Bu kayıt, yukarıdaki NAB kaynaklı ham verilerin Ömer Faruk Uzkal tarafından üretildiği veya bunların telif haklarının ona ait olduğu anlamına gelmez.

**Kaynak ile proje katkısının ayrımı:**

- Özgün beş bulut zaman serisinin kaynağı: NAB koleksiyonu ve koleksiyonun belirttiği veri sağlayıcıları.
- Projede raporlanan katkı: veri hazırlama, modelleme, karşılaştırmalı analiz, görselleştirme ve uygulama geliştirme.
- RAM dosyası: aşağıdaki ayrı açıklamaya tabidir.

### Veri seti için kaynak gösterimi

Numenta. (2015). *Numenta Anomaly Benchmark (NAB)* [Veri seti]. GitHub. https://github.com/numenta/NAB

### NAB'ın önerdiği yayın atfı

Ahmad, S., Lavin, A., Purdy, S., & Agha, Z. (2017). Unsupervised real-time anomaly detection for streaming data. *Neurocomputing, 262*, 134–147. https://doi.org/10.1016/j.neucom.2017.04.070

Bu yayın, projenin mevcut PDF kaynakçasında da yer almaktadır.

## 3. RAM telemetrisi

Rapor, `ram_telemetry.csv` dosyasının proje analizine uyarlandığını, RAM used/available/free metrikleri için kullanıldığını ve sentetik zaman damgaları içerdiğini belirtir. **Sentetik zaman damgası kullanılması, ölçüm değerlerinin de sentetik olduğu anlamına gelmez.**

Mevcut rapor ve incelenen proje dosyaları, RAM ölçüm değerlerinin ilk kaynağını ve varsa üçüncü taraf lisansını kesinleştirmemektedir. Bu nedenle dosyaya NAB, MIT veya CC lisansı atfedilmemiştir. Ham RAM verisi bu depoda dağıtılmamaktadır. Bu dosyanın paylaşılması için özgün kaynak ve kullanım koşulları ayrıca belirlenmelidir.

## 4. Lisans kapsamı

NAB deposunun 6 Eylül 2026 tarihinde kontrol edilen güncel lisansı MIT'dir. Numenta telif ve izin bildirimi [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) dosyasında korunmuştur. Kullanılan eski bir sürümde farklı koşullar varsa, ilgili sürümün koşulları ayrıca değerlendirilmelidir.

Bu projenin CC BY-NC-ND 4.0 bildirimi, üçüncü taraf veri, yazılım, yayın ve logoların haklarını değiştirmez. Veriyi analiz etmek, üçüncü taraf kaynağı yeniden lisanslama yetkisi vermez.

## English

The five cloud time series listed above originate from the NAB corpus. The PDF bibliography entry under the author's name describes the project's file inventory, not original authorship of the NAB data. Preprocessing, analysis and application development are distinct from ownership of the underlying data.

The original provenance of the RAM measurement values has not been established from the reviewed materials. Synthetic timestamps alone do not establish synthetic values. No raw CSV data is distributed here. See [third-party notices](THIRD_PARTY_NOTICES.md) for the current NAB MIT notice.

