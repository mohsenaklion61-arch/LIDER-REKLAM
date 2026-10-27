# Lider Reklam — Ücretsiz başlangıç kurulumu

Bu paket, Türkiye genelinde işletme ve hizmet ilanları için Türkçe/Farsça başlangıç sitesidir.

## Kurulum
1. https://supabase.com adresinde ücretsiz hesap ve proje oluşturun.
2. Supabase SQL Editor içinde `schema.sql` dosyasını çalıştırın.
3. Project Settings / API bölümünden Project URL ve public publishable/anon anahtarını alın.
4. `config.js` dosyasındaki yer tutucuları bu değerlerle değiştirin. `service_role` veya secret anahtarını asla tarayıcıya koymayın.
5. Siteyi Cloudflare Pages üzerinden ücretsiz yayınlayın: https://pages.cloudflare.com/
6. `index.html`, `style.css`, `app.js` ve `config.js` dosyalarını yükleyin. Ücretsiz `*.pages.dev` adresi alabilirsiniz.

## İlan onayı
Kullanıcı gönderileri `pending` durumunda kaydedilir. Supabase Dashboard > Table Editor > `listings` bölümünden ilanı kontrol edin. Uygun ilan için `status` değerini `approved`, reddetmek için `rejected` yapın. Ziyaretçiler yalnızca onaylanmış ilanları görür.

Bu başlangıç sürümünde site içi yönetici paneli ve fotoğraf yükleme yoktur; yönetim Supabase panelinden yapılır. Yayına almadan önce gizlilik/şartlar sayfası, spam önlemleri ve hukuki gereklilikler eklenmelidir.
