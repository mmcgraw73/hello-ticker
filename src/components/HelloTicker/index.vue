<template>
  <h2>{{ helloTxt || 'Hello' }}</h2>
</template>

<script>
const HELLOS = [
  'Hello',
  'Bonjour',
  'Hola',
  'Ciao',
  'Olá',
  'Kia',
  'G’day',
  'Geia',
  'Zdravo',
  'Zdravo',
  'Privet',
  'Nǐ',
  'Nǐ',
  'Namaste',
  'Kon’nichiwa',
  'Merhaba',
  'Anyeong',
  'Ahoj',
  'Guten',
  'Hallo',
  'Cześć',
  'S̄wạs̄dī',
  'Szia',
  'Ahoj',
  'Hyālō',
  'Assalam',
  'Salām',
  'Dobryj',
  'Hallå',
  'Hallo',
  'Bunâ',
  'Shalom',
  'Barev',
  'Marhabaan',
  'Sata',
  'Halo',
  'Selamat',
  'Xin',
  'Kaixo',
  'Servus',
  'Kamusta',
  'Jambo',
  'Salom',
  'Salam',
  'Slav',
  'Namaste',
  'Creole:',
  'Dobry',
  'Moni',
  'Bula',
  'Aloha',
  'Tālofa',
  'Mālō',
  'A',
  'S’mae',
  'Hei',
  'Sveiki',
  'Sveika',
  'Halló',
  'Gaelic:',
  'Dia',
  'Tere',
  'Zdravo',
  'Tashi',
  'Sabaidee',
  'Gamarjoba',
  'Dumela',
  'Saluton',
  'Bongu',
  'Hello',
  'Nde-ewo',
  'Moïen',
  'Ya’at’eeh',
  'German:',
  'Ia',
  'Përshëndetje',
  'Hola',
  'Ola',
  'Sain',
  'Salaam',
  'Vanakkam',
  'Salam',
  'Namaskāra',
  'Sannu',
  'Mingalaba',
  'Selam',
  'Demat',
  'Akkam',
  'Khurumjari',
  'Kumusta',
  'Salama',
  'Henda',
  'Choum',
  'Ayubowan',
  'Salam',
  'Hokkien:',
  'Dumela',
  'Allianchu ',
  'Molweni',
];
export default {
  name: 'HelloTicker',
  data() {
    return {
      helloTxt: 'Hello',
    };
  },
  mounted: function () {
    window.setInterval(() => {
      this.helloTxt = this.getHello();
    }, 5000);
  },
  methods: {
    getIndex() {
      return Math.floor(Math.random() * 99 + 1);
    },
    getHello() {
      return HELLOS[this.getIndex()];
    },
  },
};
</script>

<style>
html,
body {
  background: #363737;
}
h2 {
  color: hotpink;
  font-size: 66px;
}
</style>
