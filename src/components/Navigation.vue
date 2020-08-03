<template>
  <div>
    <nav>
      <router-link to="/"><img class="about" src="../assets/logo.png" /></router-link>
      <router-link to="/Home"><img class="home" src="../assets/home.png" /></router-link>
      <router-link to="/About"><img class="file" src="../assets/two-overlapping-square.png" /></router-link>

       <div class="search-wrapper">
       <div class="tick">✓</div>
          <input class="searchbar" type="text" placeholder="Build on Dploy completed by Guy Bosa"/>
        </div>

        <router-link to=""><img class="bell" src="../assets/bell-icon.png" /></router-link>
        <router-link to=""><img class="bolt" src="../assets/bolt.png" /></router-link>
        <div class="avatar-info"><h4>Guy Bosa</h4><p>guybosa0@gmail.com</p></div>
        <router-link to=""><img class="about" src="../assets/user.png" /></router-link>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Navigation',
  data () {
    return {
      links: [
        {
          id: 1,
          text: 'Home',
          page: '/Home'
        },
        {
          id: 2,
          text: 'About',
          page: '/About'
        },
        {
          id: 3,
          text: 'Contact',
          page: '/Contact'
        }
      ]
    }
  }
}
</script>

<style>
  .spacing {
    Margin-right: 10px;
  }
  nav {
    overflow: hidden;
    background-color: #171B26;
    position: fixed;
    height: 60px;
    top: 0;
    bottom: 0;
    width: 100%;
    display: flex;
    justify-content: space-evenly;
  }
  .tick {
  position: absolute;
    top: 12px;
    margin: 0 0 0 10px;
  }
  .searchbar {
  text-align: center;
  background-color: #11151E;
  color: white;
  flex: auto;
  width: 390px;
  border-radius: 11px;
  outline: none;
    border-color: transparent;
    margin-top: 10px;
  }
  .home {
  height: 43px;
  margin-top: 5px;
padding: 0 0 0 50px;
  }

  .about {
  margin-top: 5px;
  height: 33px;
  }

  .bell {
  margin-top: 5px;
  height: 33px;
  padding: 0 0 0 100px;
  }

  .bolt {
  padding: 0 50px 0 0;
  margin-top: 5px;
  height: 33px;
  }

  .file{
  padding: 0 100px 0 0;
  margin-top: 5px;
  height: 33px;

  }

  .avatar-info {
  text-align: right;
    line-height: 0;
    }

  .search-wrapper {
  color: white;
  }

</style>
