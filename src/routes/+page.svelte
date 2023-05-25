<script>
    import "../app.css"
    import Navbar from "../components/Navbar.svelte";
</script>

<main>
  <Navbar/>
  <div class="content">
    <div class="main">
        <h1>Hello World!</h1>
        <ul>
            <li>Mario Sebastian Carlosiano 20.11.3439</li>
            <li>Siti Nadia Nurul Fatihah 20.11.3472</li>
            <li>Marssel Nasran Lingkubi 20.11.3443</li>
        </ul>
    </div>
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
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .coba {
    height: 100px;
  }
</style>
