# Vue JS Learn Component sandbox

Halo semuanya, Vue JS component sandbox ini bisa menjadi salah satu alat kalian untuk belajar Single file component, Props, Emit, pada vue.js. Bundler yang akan kita digunakan adalah [parcel](https://parceljs.org/getting_started.html) silahkan lakukan installasi bundler tersebut terlebih dahulu.

## Instalasi & Project setup

1. git checkout "1.installation"
2. Lakukan project folder setup sesuai dengan [link berikut](https://wahyudiputra.com/blog/build-vue-app-with-parcel/)

## Creating Single File Component

1. git checkout "2.component-slicing"
2. Buatlah component dengan nama "DashboardPage" pada folder components, (silahkan ambil template htmlnya pada file template.html)
3. Buatlah component dengan nama "AboutPage" pada folder components, (silahkan ambil template htmlnya pada file template.html)
4. Daftarkan dan render kedua component diatas pada file App.vue. Untuk contoh pembuatan component dan pendaftarannya di App kalian bisa lihat [link berikut](https://vuejs.org/v2/guide/single-file-components.html#Example-Sandbox)
5. Tambahkan property data pada App.vue, tambahkan state "currentPage" pada property data di App.vue
6. Tambahkan conditional rendering mengggunakan [v-if](https://vuejs.org/v2/api/#v-if). jika currentPagenya berisi "dashboard" maka component "DasboardPage" yang akan dirender sedangkan jika currentPagenya berisi "about" maka component "AboutPage"

## Props (Passing data down to children component)

1. git checkout "3.props"
2. Lakukan fetching pada method fetchUsers yang terdapat di App.vue dan simpan valuenya ke state users ! kalian bisa lakukan request ke https://jsonplaceholder.typicode.com/users
3. Kirimkan data users menggunakan props ke component "DashboardPage"
4. Lakukan looping component "UserRow" di component "DashboardPage" sejumlah data users yang diterima di props dan kirimkan props "user" di setiap iterasinya ke component "UserRow". [v-for](https://vuejs.org/v2/api/#v-for)
5. Referensi: https://vuejs.org/v2/guide/components-props.html
6. Contoh pengiriman props bisa dilihat di component TodoList [sandbox berikut](https://codesandbox.io/s/o29j95wx9?file=/components/TodoList.vue)
7. Contoh menerima data props bisa dilihat di component TodoListItem [sandbox berikut](https://codesandbox.io/s/o29j95wx9?file=/components/TodoListItem.vue)

## Emit (Listening to Child Components Events)

1. git checkout "4.emit"
2. Lakukan emit pada method changePage di component Navbar dengan isi argumen emit pertama "listenChangePage" dan argumen emit kedua isi variable page (untuk memanggil emit pada method bisa menggunakan this.$emit)
3. Dengarkan event listenChangePage pada parent dari component Navbar yaitu "App.vue" dengan menggunakan v-on
4. Jalankan method changePage pada App.vue ketika terjadi event listenChangePage
5. referensi: https://vuejs.org/v2/api/#vm-emit

## Additional

1. Direkomendasikan untuk latihan lagi menggunakan [link berikut](https://dhimas-hary.medium.com/learn-vue-js-single-file-component-passing-and-receiving-data-between-components-7a04ce3e2d40) untuk memperdalam konsep komponen dan penggunaan emit & props.