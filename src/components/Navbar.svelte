<script>
  import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte'
</script>

<Navbar let:hidden let:toggle>
  <NavBrand href="/">
    <img
      src="/images/flowbite-svelte-icon-logo.svg"
      class="mr-3 h-6 sm:h-9"
      alt="Flowbite Logo"
    />
    <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">
      EduWeb
    </span>
  </NavBrand>
  <NavHamburger on:click={toggle} />
  <NavUl {hidden}>
    <NavLi href="/" active={true}>Home</NavLi>
    <NavLi href="/about">Courses</NavLi>
    <NavLi href="/services">Blog</NavLi>
    <NavLi href="/pricing">About Us</NavLi>
    <NavLi href="/login">Login</NavLi>
    <NavLi href="/signup">Sign Up</NavLi>
  </NavUl>
</Navbar>



<!-- <script>

</script>

<nav>
  <div class="logo">EduWeb</div>
  <ul> 
    <li>
      <a href="#">Home</a>
    </li>
    <li>
      <a href="#">Courses</a>
    </li>
    <li>
      <a href="#">Blog</a>
    </li>
    <li>
      <a href="#">About Us</a>
    </li>
    <li class="login">
      <a href="#">Login</a>
    </li>
    <li class="sign-up">
      <a href="#">Sign Up</a>
    </li>
  </ul>
</nav>

  <style>
  nav {
    background-color: #FFF2E1;
    display: flex;
    justify-content: space-between;
    padding-left: 100px;
    padding-right: 100px;
    height: 100px;
    align-items: center;
  }
  nav ul {
    list-style-type: none;
    display: flex;
    gap: 80px;
    align-items: center;
  }
  nav ul li a {
    text-decoration: none;
    color: #252641;
    font-size: 20px;
  }
  .login {
    background-color: white;
    padding-bottom: 10px;
    padding-top: 10px;
    width: 100px;
    text-align: center;
    border-radius: 20px;
  }
  .sign-up {
    background-color: #F48C06;
    padding-bottom: 10px;
    padding-top: 10px;
    width: 100px;
    text-align: center;
    border-radius: 20px;
  }
</style> -->
