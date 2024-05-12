# IdentityGoogleAuth

Bu proje, ASP.NET Core Identity kullanarak Google ile kimlik doğrulamasını göstermektedir.

## Kurulum

1. Depoyu klonlayın (`git clone https://github.com/kullaniciadi/IdentityGoogleAuth.git`)
2. Visual Studio Code gibi bir IDE'de projeyi açın
3. `appsettings.json` dosyasını açın ve `DefaultConnection` bağlantı dizesini kendi SQLite veritabanı yolunuza güncelleyin
4. Google OAuth kimlik doğrulama bilgilerinizi alın ve `appsettings.json` dosyasındaki `Auth:Google` ve `Auth:Google:Secret` değerlerini güncelleyin (https://cloud.google.com/docs/authentication?_gl=1*bpwshy*_ga*ODQ0NTgyODM3LjE3MTU1MzI3MjI.*_ga_WH2QY8WWF5*MTcxNTUzMjcyMS4xLjEuMTcxNTUzNDQzMy4wLjAuMA..&_ga=2.67283608.-844582837.1715532722)
5. Projeyi derleyin ve çalıştırın

## Kullanım

1. Uygulamayı başlatın
2. Tarayıcınızda `https://localhost:5123` adresine gidin
3. Google ile giriş yapmak için "Login" bağlantısına tıklayın ve Google hesabınızla giriş yapın

## Katkıda Bulunma

Projede asıl odaklanmamız gereken nokta google ile nasıl kayıt olma ve giriş yapma süreçlerini yönetebileceğimiz kısımdır.

`dotnet new mvc -au Individual -n IdentityGoogleAuth` komutu ile mvc template'i kullanarak projemizi oluşturuyoruz.

.csproj dosyasında paketleri direkt aktarabilirsiniz. 

` dotnet aspnet-codegenerator identity -dc ApplicationDbContext` kodu ile template'İmizin geri kalanını yüklüyoruz. (https://learn.microsoft.com/tr-tr/aspnet/core/fundamentals/tools/dotnet-aspnet-codegenerator?view=aspnetcore-8.0)

Google cloud tarafında api kullanımı için client bilgilerini de aldıktan sonra projeyi kullanbilir hale getirebilirsiniz. İyi Çalışmalar.

## Lisans

Bu proje [MIT Lisansı](LICENSE) altında lisanslanmıştır.

