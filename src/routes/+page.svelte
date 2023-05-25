<script>
    import "../app.css"
    import Navbar from "../components/Navbar.svelte";
</script>

<main>
  <Navbar/>
  <div class="content">
    <div class="main"><h1>Hello World!</h1></div>
    <div class="coba"></div>
  </div>
</main>

<style>
  .main {
    background-color: #FFF2E1;
    height: 100vh;
    border-bottom-right-radius: 20%;
    border-bottom-left-radius: 20%;
    display: flex;
    justify-content: center;
  }
  .coba {
    height: 100px;
  }
</style>
