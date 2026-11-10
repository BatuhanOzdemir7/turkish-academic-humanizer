# Turkish Academic Text Humanizer 🇹🇷✒️

Yapay zeka dil modelleri (LLM) tarafından üretilen Türkçe akademik metinlerdeki sentetik sözdizimini (perplexity) ve tekdüze ritmi (burstiness) optimize ederek metnin doğal dil akışını sağlayan ve akademik platformlardaki *false-positive* etiketlenme riskini en aza indiren, ileri düzey bir Sistem Komutu (System Instruction) mimarisidir.

## 🎯 Projenin Amacı

Günümüzdeki büyük dil modelleri Türkçe akademik metin üretirken sıklıkla İngilizce'den çeviri kokan kalıplar (calque) ve aşırı öngörülebilir bağlaç örüntüleri kullanmaktadır. Bu durum, özgün araştırma metinlerinin bile yapay zeka tespit algoritmaları tarafından hatalı şekilde yapay zeka olarak etiketlenmesine yol açabilmektedir. Bu proje; taslak metinleri veri kaybı yaşatmadan, akademik tonu ve nesnelliği koruyarak ve morfolojik varyans yaratarak optimize eder.

## ✨ Öne Çıkan Özellikler

* **Perplexity Kırıcılar:** Yapay zekanın aşırı sık kullandığı çerçeveleme kalıplarını ve şişirme ifadeleri temizler, alan-spesifik doğrudan anlatımı teşvik eder.
* **Burstiness (Ritim) Mimarisi:** Paragraf içindeki cümle uzunluklarında asimetri yaratarak monotonluğu kırar.
* **Mekanik Bağlaç Yasakları:** Robotik geçiş ifadeleri yerine önceki cümlenin nesnesini yeni cümlenin öznesi yapan anlamsal zincirleme (*semantic chaining*) tekniğini uygular.
* **Akademik Ton Koruması:** Metnin laubalileşmesini önler; yüksek etki faktörlü dergilerin nesnel, veriye dayalı ve ihtiyatlı (*hedging*) dil yapısını muhafaza eder.
* **Otomatik Raporlama:** Düzenlenen metnin yanı sıra, yapılan tüm dilbilimsel müdahaleleri gösteren 3 sütunlu bir değişiklik analizi tablosu üretir.

## 🚀 Nasıl Kullanılır?

1. `SYSTEM_INSTRUCTION.md` dosyasında yer alan master prompt metnini kopyalayın.
2. Kullandığınız yapay zeka modelinin (Gemini, ChatGPT, Claude vb.) *System Prompt* veya *Custom Instructions* alanına yapıştırın.
3. Düzenlenmesini istediğiniz Türkçe akademik taslak metni modele iletin.
