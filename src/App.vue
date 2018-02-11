<template>

  <div id="app">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css"
     integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">
    <div class="container">
      <b-navbar toggleable="md">

         <b-navbar-brand id="home">
            <h1>Sérgio Carneiro</h1>
        </b-navbar-brand>

        <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>       
       
        <b-collapse is-nav id="nav_collapse">
            <b-navbar-nav>
                <b-nav-item to="/" exact>Profile</b-nav-item>
                <b-nav-item to="/skills">Skills</b-nav-item>
                <b-nav-item to="/technical">Technical</b-nav-item>
            </b-navbar-nav>
        </b-collapse>
        
      </b-navbar>
    </div>
    <hr/>
    
    <router-view/>
  </div>
</template>

<script>
export default {
  name: "App"
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 20p;
}

#home {
  font-family: Britannica Bold;
}

hr {
    display: block;
    height: 1px;
    border: 0;
    border-top: 1px solid #ccc;
    margin-top: 2px;
    padding: 0;
}

</style>
