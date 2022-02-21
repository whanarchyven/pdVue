<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import HelloWorld from './components/HelloWorld.vue';
import Navbar from "./components/Navbar.vue";
import CompanyTitle from "./components/CompanyTitle.vue";
import CompanyEmployeerCardDemo from "./components/CompanyEmployeerCardDemo.vue";
import CompanyEmployeersList from "./components/CompanyEmployeersList.vue";
import VacancyCard from "./components/VacancyCard.vue";
import VacancyList from "./components/VacancyList.vue";



const proba={
  full_name:"ООО МОСПОЛИТЕХ",
  name:"МОСПОЛИТЕХ",
  logo:"../assets/aue.jpg",
  desc:"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum",
  rating:4.123,
  comments_quantity:25,
}
const employers=[
  {
  name:"Евгений",
  surname:"Селин",
  photo:"some.png",
  job:"Senior Developer",
  short_desc:"Lorem ipsum",
  full_desc:"Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum",
  email:"evgeniy@gmail.com",
  phone:"+799999123",
  },
  {
    name:"Евгений",
    surname:"Селин",
    photo:"some.png",
    job:"Senior Developer",
    short_desc:"Lorem ipsum",
    full_desc:"Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum",
    email:"evgeniy@gmail.com",
    phone:"+799999123",
  },
  {
    name:"Евгений",
    surname:"Селин",
    photo:"some.png",
    job:"Senior Developer",
    short_desc:"Lorem ipsum",
    full_desc:"Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum",
    email:"evgeniy@gmail.com",
    phone:"+799999123",
  },
  {
    name:"Евгений",
    surname:"Селин",
    photo:"some.png",
    job:"Senior Developer",
    short_desc:"Lorem ipsum",
    full_desc:"Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum",
    email:"evgeniy@gmail.com",
    phone:"+799999123",
  },
  {
    name:"Евгений",
    surname:"Селин",
    photo:"some.png",
    job:"Senior Developer",
    short_desc:"Lorem ipsum",
    full_desc:"Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum",
    email:"evgeniy@gmail.com",
    phone:"+799999123",
  },
]
const vacancies=[
  {
  name:"Разработка логотипа",
  desc: 'Разработка логотипа описание разработка логотипа описание разработка логотипа описание разработка логотипа описание',
  payment:1000,
  updated_at:'22.02.2002',
  },
  {
    name:"Разработка логотипа",
    desc: 'Разработка логотипа описание разработка логотипа описание разработка логотипа описание разработка логотипа описание',
    payment:1000,
    updated_at:'22.02.2002',
  },
  {
    name:"Разработка логотипа",
    desc: 'Разработка логотипа описание разработка логотипа описание разработка логотипа описание разработка логотипа описание',
    payment:1000,
    updated_at:'22.02.2002',
  },
  {
    name:"Разработка логотипа",
    desc: 'Разработка логотипа описание разработка логотипа описание разработка логотипа описание разработка логотипа описание',
    payment:1000,
    updated_at:'22.02.2002',
  },
  {
    name:"Разработка логотипа",
    desc: 'Разработка логотипа описание разработка логотипа описание разработка логотипа описание разработка логотипа описание',
    payment:1000,
    updated_at:'22.02.2002',
  },
  {
    name:"Разработка логотипа",
    desc: 'Разработка логотипа описание разработка логотипа описание разработка логотипа описание разработка логотипа описание',
    payment:1000,
    updated_at:'22.02.2002',
  },
  {
    name:"Разработка логотипа",
    desc: 'Разработка логотипа описание разработка логотипа описание разработка логотипа описание разработка логотипа описание',
    payment:1000,
    updated_at:'22.02.2002',
  },
  {
    name:"Разработка логотипа",
    desc: 'Разработка логотипа описание разработка логотипа описание разработка логотипа описание разработка логотипа описание',
    payment:1000,
    updated_at:'22.02.2002',
  },
  {
    name:"Разработка логотипа",
    desc: 'Разработка логотипа описание разработка логотипа описание разработка логотипа описание разработка логотипа описание',
    payment:1000,
    updated_at:'22.02.2002',
  },
]
</script>

<template>
  <navbar msg="sadaf"></navbar>
  <company-title :company="proba"></company-title>
  <company-employeers-list :employers="employers"></company-employeers-list>
  <vacancy-list :vacancies="vacancies"></vacancy-list>
</template>

<style>
@import url(https://gist.githubusercontent.com/mfd/09b70eb47474836f25a21660282ce0fd/raw/2923dc0cccd912c217ef244f5c42d547deab5b60/Gilroy.css);
@import url(https://gist.githubusercontent.com/praveenscience/4063b6db4bb3774d21e2219eeb00ff03/raw/4790dc13c0bea5c22cabf7e5d50fee1e61d27a88/proxima-nova.css);
#app {
  font-family: Gilroy,Proxima Nova, Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
