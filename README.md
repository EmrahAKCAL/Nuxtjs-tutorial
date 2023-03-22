<h3>Nuxt.js Nedir?</h3>
<p>Nuxt.js, Vue.js, Node.js, Webpack ve Babel.js tabanlı ücretsiz ve açık kaynaklı bir JavaScript kitaplığıdır. Nuxt, React.js'yi temel alan benzer amaçlı bir çerçeve olan Next.js'den ilham almıştır.</p>
<ul>
<li>Modern javascript framework ü olan(SPA-Single Page Application) Vue.js üzerinden derlenir.</li>
<li>Dosya ve klasör yapılarını kullanarak konfigürasyon yapar.</li>
<li>Universal Vue Application(SSR-Server Side Rendering) üretmemize imkan sağlar.</li>
</ul>

<h3>Proje Dosyalarının Oluşturulması</h3>
<ul>
<li>Kullandığımız paket yönetim sisteme göre aşağıdaki kodu bilgisayarımızın terminalinde(cmd) çalıştırılır.
<ul>
<li>yarn için ==> <strong>yarn create nuxt-app PROJE_ISMI</strong></li>
<li>npx için ==> <strong>npx create-nuxt-app PROJE_ISMI</strong></li>
<li>npm için ==> <strong>npm init nuxt-app PROJE_ISMI</strong></li>
</ul>
</li>
<li>Birinci işlem yaptıktan sonra terminalimize gelen aşağıdakilere benzer sorulara yanıt verilerek proje oluşturulur.
<ul>
<li><strong> Project name</strong>: Projeye bir isim verilir ya da varsayılan olarak oluşturmuş olduğumuz klasör ismi onaylayabiliriz.</li>
<li><strong> Programming language</strong>: Projemizi hangi dilde(javascript ya da typescript) yazacağımızı seçeriz.</li>
<li><strong> Package manager</strong>: Hangi paket tönetimini kullanacağımızı seçeriz.</li>
<li><strong> UI framework</strong>: Gelen liste içerisinde hangi kullanıcı arayüz framework kullanacağımızı seçeriz veya <strong>None</strong> seçip devam edebiliriz.</li>
<li><strong> Template engine</strong>: Kullanmak istediğimiz template(HTML ya da Pug) seçilir.</li>
<li><strong> Nuxt.js modules</strong>: Gelen liste içerisindeki modüllerden biri seçilir.
<ul>
<li><strong>Axios - Promise based HTTP client</strong></li>
<li><strong>Progressive Web App (PWA)</strong></li>
<li><strong>Content - Git-based headless CMS</strong></li>
</ul>
</li>
<li><strong>Linting tools</strong>: Gelen liste içerisinde kullanmak istediğimiz araçlardan biri seçilir.
<ul>
<li><strong>ESLint</strong></li>
<li><strong>Prettier</strong></li>
<li><strong>Lint staged files</strong></li>
<li><strong>StyleLint</strong></li>
<li><strong>Commitlint</strong></li>
</ul>
</li>
<li><strong> Testing framework</strong>: Kullanmak istediğimiz bir test framework varsa seçilir.</li>
<li><strong> Rendering mode</strong>: Kullanmak istediğimiz render modu(Universal (SSR / SSG), Single Page App) seçilir. Nuxt.js nin özelliklerden yararlanmak için burada Server Side Rendering(SSR) seçilmeli. </li>
<li><strong> Deployment target</strong>: Deploymen hedefi(Server (Node.js hosting), Static (Static/Jamstack hosting)) seçilir.</li>
<li><strong> Development tools</strong>: Kullanmak istediğimiz geliştirme araçlarından biri seçilir.</li>
<li><strong> Version control system</strong>: Varsa kullanmak isteğimiz kontrol sistemi(git vb.) seçilir.</li>
</ul>
</li>
</ul>
<p>Proje oluşturulduktan sonra proje dizinine giderek <strong>npm run dev</strong> ile proje çalıştırılır.</p>

<h3> Yapının Kurulumu</h3>

```bash
# Bağımlılıkların kurulumu
$ npm install

# Projeyi çalışmak
$ npm run dev

# Prod için derleme ve sunucu başlatma
$ npm run build
$ npm run start

# Statik proje oluştur
$ npm run generate
```

<p> Daha ayrıntılı açıklamalar için <a href="https://nuxtjs.org">nuxtjs.org</a> sayfasına göz atabilirsiniz.</p>

<h3>Proje Dosyaları</h3>
<p>
Bazıları özel davranışlara sahip olan aşağıdaki ekstra dizinleri oluşturabilirsiniz. Yalnızca <strong>pages</strong> gereklidir; işlevlerini kullanmak istemiyorsanız onları silebilirsiniz.</p>
<ul>
  <li><strong>assets</strong>: Stil(Stylus veya Sass) dosyaları, resimler veya yazı tipleri gibi derlenmemiş varlıklarınızı içerir. <a href="https://nuxtjs.org/docs/2.x/directory-structure/assets">Daha fazla bilgi</a></li>
  <li><strong>components</strong>: Vue.js conponentlerini içerir. Componentler, sayfanızın farklı bölümlerini oluşturur. <a href="https://nuxtjs.org/docs/2.x/directory-structure/components">Daha fazla bilgi</a></li>
  <li>
    <strong>layouts</strong>: İster sidebar eklemek, ister mobil ve masaüstü için farklı düzenlere sahip olmak isteyin, Nuxt uygulamanızın görünümünü ve verdiği hissi değiştirmek istediğinizde düzenler çok yardımcı olur.
    <a href="https://nuxtjs.org/docs/2.x/directory-structure/layouts">Daha fazla bilgi</a>
  </li>
  <li><strong>pages</strong>: Bu dizin, uygulama görünümlerinizi ve rotalarınızı içerir. Nuxt, bu dizindeki tüm `*.vue` dosyalarını okuyacak ve Vue Router'ı otomatik olarak kuracaktır.
    <a href="https://nuxtjs.org/docs/2.x/get-started/routing">Daha fazla bilgi</a></li>
  <li><strong>plugins</strong>: Plugins dizini, root Vue.js Uygulamasını başlatmadan önce çalıştırmak istediğiniz JavaScript eklentilerini içerir.
    Burası, Vue eklentileri eklemek ve işlevleri veya sabitleri enjekte etmek için kullanılan yerdir. 
    'Vue.use()'yi her kullanmanız gerektiğinde, 'plugins/' içinde bir dosya oluşturmalı ve yolunu 'nuxt.config.js' içindeki eklentilere eklemelisiniz.
    <a href="https://nuxtjs.org/docs/2.x/directory-structure/plugins">Daha fazla bilgi</a></li>
  <li><strong>static</strong>: Bu dizin statik dosyalarınızı içerir. Bu dizindeki her dosya `/` ile eşlenir.<br> <strong>Örnek: </strong>  '/static/robots.txt', '/robots.txt' olarak eşlenir.
    <a href="https://nuxtjs.org/docs/2.x/directory-structure/static">Daha fazla bilgi</a></li>
  <li><strong>store</strong>:Bu dizin, Vuex mağaza dosyalarınızı içerir. Bu dizinde bir dosya oluşturmak, Vuex'i otomatik olarak etkinleştirir. 
    <a href="https://nuxtjs.org/docs/2.x/directory-structure/store">Daha fazla bilgi</a></li>
</ul>
