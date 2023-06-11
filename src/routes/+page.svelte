<script>
    import "../app.css"
    import Navbar from "../components/Navbar.svelte";
    import avatar from "$lib/assets/Ellipse.png"
</script>

<main>
  <Navbar/>
  <div class="content">
    <div class="main">
      <div style="display: flex; flex-direction: column; flex:1.5; align-self: start; height: 100%; padding-top: 5%; box-sizing: border-box;">
        <span style="font-size: 39px; font-weight: bold;"><span style="color: #F48C06;">"Master the web from</span><br> <span style="color: #2F327D;">Anywhere</span>, <span style="color: #65DAFF;">Anytime"</span></span>
        <p>Pelajari pengembangan web dengan cara yang inovatif dan interaktif melalui EduWeb, platform e-learning sejati.</p>
        <div><button class="ayo-gabung">Ayo Gabung</button> <button>Lihat Cara Kerjanya</button></div>
      </div>
      <div class="coba" style="flex: 1; height: 100%; padding-top: 14%; box-sizing: border-box; display: flex; justify-content: center;">
        <div style="background-color: white; border-radius: 10px; height: 350px;display: flex;flex-direction: column; align-items: center; width: 90%; padding-top: 5%;">
          <div style="display: flex; gap: 7px;">
            <img src="{avatar}" alt="avatar" height="40" width="40"/>
            <div style="display: flex; flex-direction: column;">
              <span style="font-weight: bold;">User Experience Class</span>
              <span style="font-size: small;">Today at 12.00 PM</span>
            </div>
          </div>
          <button class="join-now">Join Now</button>
          <div>
            <div class="jadwal-logo"></div>
            <span>250k</span>
            <p>Assisted Student</p>
          </div>
        </div>
      </div>
      <div class="coba2" style="flex: 1; background-color: violet;">
        <div class="card" style="background-color: white;">
          <div class="mail-logo"></div>
          <span>Congratulation</span>
          <p>Your admission completed</p>
        </div>
      </div>
    </div>
  </div>
</main>

<style>
  .content {
    display: flex;
    justify-content: center;
    background-color: #FFF2E1;
  }
  .main {
    height: 100vh;
    border-bottom-right-radius: 20%;
    border-bottom-left-radius: 20%;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 85%;
  }
  .ayo-gabung {
    background-color: #F48C06;
    padding-bottom: 10px;
    padding-top: 10px;
    width: 100px;
    text-align: center;
    border-radius: 20px;
    color: white;
  }
  .join-now {
    background-color: red;
    padding-bottom: 10px;
    padding-top: 10px;
    width: 100px;
    text-align: center;
    border-radius: 20px;
    color: white;
  }
</style>
