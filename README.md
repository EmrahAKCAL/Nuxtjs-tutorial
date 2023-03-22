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

## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out the [documentation](https://nuxtjs.org).

## Special Directories

You can create the following extra directories, some of which have special behaviors. Only `pages` is required; you can delete them if you don't want to use their functionality.

### `assets`

The assets directory contains your uncompiled assets such as Stylus or Sass files, images, or fonts.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/assets).

### `components`

The components directory contains your Vue.js components. Components make up the different parts of your page and can be reused and imported into your pages, layouts and even other components.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/components).

### `layouts`

Layouts are a great help when you want to change the look and feel of your Nuxt app, whether you want to include a sidebar or have distinct layouts for mobile and desktop.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/layouts).


### `pages`

This directory contains your application views and routes. Nuxt will read all the `*.vue` files inside this directory and setup Vue Router automatically.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/get-started/routing).

### `plugins`

The plugins directory contains JavaScript plugins that you want to run before instantiating the root Vue.js Application. This is the place to add Vue plugins and to inject functions or constants. Every time you need to use `Vue.use()`, you should create a file in `plugins/` and add its path to plugins in `nuxt.config.js`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/plugins).

### `static`

This directory contains your static files. Each file inside this directory is mapped to `/`.

Example: `/static/robots.txt` is mapped as `/robots.txt`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/static).

### `store`

This directory contains your Vuex store files. Creating a file in this directory automatically activates Vuex.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/store).
