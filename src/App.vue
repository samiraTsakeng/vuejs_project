<template>
  <div id="app">
  <NavComponent />
  <PictureHeader />
  <section class="featured" id="companies">
      <FeaturedHeader />
  </section>



  </div>
</template>

<script>
import NavComponent from './components/NavComponent.vue'
import PictureHeader from './components/PictureHeader.vue';
import FeaturedHeader from './components/FeaturedHeader.vue';
export default{
  name: 'App',
  components: {
  NavComponent,
  PictureHeader,
  FeaturedHeader
  }
}
</script>

<style>
:root{
    --primarycolor: #CD7F32;
    --whitecolor: #FFFFFF;
    --Blackcolor: #000000;
    --greycolor: #A9A9A9;
    --Pinkcolor: #E8ADAA;
    --Bluecolor: #2B65EC;   
}

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    outline: none;
    font-family: 'Nunito', sans-serif;
}

body{
    width: 100%;
    height: auto;
    
}

h1{
    line-height:1.5;
}

.navbar{
    width: 100%;
    height: 60px;
    display: flex;
    justify-content: space-around;
    position: fixed;
    top: 0;
    left: 0;
    padding: 1rem 2.5rem;
    z-index: 10;
    color: var(--greycolor);
    background: #CD7F32;
}

.navbar-logo > a {
    letter-spacing: 0;
    text-decoration: none;
    color: var(--Blackcolor);
}

.navbar-menu{
    width: 400px;
    display: flex;
    justify-content: space-between;

}

.navbar-menu > a{
    color: var(--Blackcolor);
    text-decoration:none;
    margin: 0px 0px 10px 10px;
    font-weight: bolder;
    
}

.navbar-menu > a:hover{
    background: #FFF;
    height: fit-content;
}

.dropbtn {
    background-color: transparent;
    color: black;
    padding: 2.5px;
    font-size: 15px;
    border: none;
    font-weight: bolder;
    
  }
  
  .dropdown {
    position: relative;
    display: inline-block;
  }
  
  .dropdown-content {
    display: none;
    position: absolute;
    background-color: #f1f1f1;
    min-width: 160px;
    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
    z-index: 1;
  }
  
  .dropdown-content a {
    color: black;
    padding: 12px 16px;
    text-decoration: none;
    display: block;
  }
  
  .dropdown-content a:hover {background-color: #cd770f;}
  
  .dropdown:hover .dropdown-content {display: block;}
  
  .dropdown:hover .dropbtn {background-color: #ffffff;}
.menu-toggle{
    display: none;
}

.menu-toggle .bar{
    width: 15px;
    height: 2px;
    margin: 3px auto;
    transition: all 0.3 ease-in-out;
    background-color: #000000;
    cursor: pointer;
}

header{
    width: 100%;
    height:80%;
    background-image: url("./assets/image5.jpg");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
}

.header-title {
    position: absolute;
    top: 7rem;
    left: 3rem;
    letter-spacing: 3;
    font-weight: bolder;
    font-size: 52px;
    color: var(--whitecolor);
    text-shadow: 4px 2px 0px rgba(0,0,0,0.2);
}

.header-title > span {
 color: var(--primarycolor)
}

.featured{
    width: 100%;
    height: auto;
    text-align: center;
    padding: 5rem 1rem;
    background-color: #FFFFFF;   
}

.section-title {
    margin-bottom: 0.5rem;
    letter-spacing: 1.5;
    font-size: 36px;
}

.featured-wrapper{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
    gap: 5rem;
    align-items: center;
    width: 90%;
    padding: 3% 10%;
}

.featured-card{
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 1rem;
    background-color: var(--whitecolor);
    box-shadow: rgba(0, 0, 0, 0.16) 0px 1px 4px;
}

.featured-card:hover{
box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}

.featured-image {
    height: 50px;
    margin-bottom: 0.2rem;
}

.featured-button{
    border: 1px solid var(--primarycolor);
    background-color: transparent;
    margin-top: 0.5rem;
    padding: 3px 10px;
    cursor: pointer;
    color: var(--primarycolor);
}

.featured-button:hover {
    background-color:var(--primarycolor);
    color: var(--whitecolor);
}
.join{
    width: 100%;
    height:350px;
    background-image: url(./assets/image5.jpg);
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    color:#000000;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 1rem 3rem;
    align-items:center;
    position: relative;
    padding-top: 0;
}

.join-detail > p {
    color:#FFFFFF;
}

.join::before {
    content:"";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: linear-gradient(180deg, rgba(0, 0, 0, 0.6) 0%, rgba(0, 122, 255, 0.5) 100%),
    linear-gradient(180deg, rgba(0, 0, 0, 0.65) 0%, transparent 100%);
    z-index: 1;
}

.join-detail{
    min-width: 280px;
    width: 50%;
    z-index: 2;
    margin-bottom: 1rem;
}

.join-detail{
    font-size: 36px;
    letter-spacing: 2;
}

.join-button{
    width: 200px;
    padding: 1rem;
    border: none;
    color: var(--Blackcolor);
    background-color: var(--primarycolor);
    box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
    z-index: 2;
    cursor: pointer;
}

.join-button:hover{
    background: transparent;
    border: 2px solid #551606;
    color: #551606;
}





</style>
