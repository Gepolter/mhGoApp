<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
    
    <div id="donate-button-container">
      <div id="donate-button"></div>
    </div>


  </nav>
  <GoogleAdSense adSlot="5373754521" :timeout="200" classNames="page-top"/>
  <router-view/>
</template>

<style lang="scss">
#app {
  font-family: "MonsterHunter", Arial, Helvetica, sans-serif;
  color: var(--mh-white);

  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  

  body {
    background-color: var(--mh-gray);
    //font-family: "monsterhunter", Avenir, sans-serif;
  }

  //vselect vars
  --vs-controls-color: var(--mh-yellow);
  --vs-border-color: var(--mh-dark-yellow);

  --vs-dropdown-bg: linear-gradient(var(--mh-yellow), var(--mh-dark-yellow));
  --vs-dropdown-color: black;
  --vs-dropdown-option-color: black;

  //--vs-selected-bg: green;
  --vs-selected-color: #eeeeee;

  --vs-search-input-color: #eeeeee;

  --vs-dropdown-option--active-bg: var(--mh-light-blue);
  --vs-dropdown-option--active-color: #eeeeee;
/*
  --vs-transition-timing-function: cubic-bezier(1,-0.115,0.975,0.855);
  --vs-transition-duration: 1500ms;
*/
  .vcp__header-icon{
    height: 0%;
    width: 0%;
    overflow: hidden;
  }
  .vcp__header-title{
    flex: 4;
  }
  .vcp__header{
    display: flex;
    justify-content: space-between;
    align-items:stretch;
    padding-bottom: 5px;
  }
  .vcp__body{
    max-height: fit-content;
  }

  button{
    background: radial-gradient(var(--mh-red), var(--mh-dark-red));
    color: var(--mh-white);
    border: 3px solid black;
    font-family: inherit;
  }
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
/* width */
::-webkit-scrollbar {
  width: 12px;
}

/* Track */
::-webkit-scrollbar-track {
  background: var(--mh-gray); 
  background: linear-gradient(var(--mh-dark-green), var(--mh-light-blue));
  border: 2px solid black;
  border-radius: 50%;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: linear-gradient(var(--mh-dark-red), var(--mh-red));
  border:2px solid var(--mh-orange);
  border-radius: 70%;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: linear-gradient(var(--mh-dark-green), var(--mh-light-blue));
}


</style>

<script>
  import GoogleAdSense from "../src/components/GoogleAdSense"
  export default {
  name: "App",
  components: {
    GoogleAdSense
  }
};
</script>