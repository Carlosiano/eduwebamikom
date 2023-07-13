<script>
	import {
		Avatar,
		Navbar,
		NavBrand,
		NavLi,
		NavUl,
		NavHamburger,
		Button,
		Input,
		Dropdown,
		DropdownItem,
		DropdownHeader,
		DropdownDivider,
    DarkMode
	} from 'flowbite-svelte';
</script>

<Navbar let:hidden let:toggle>
	<NavBrand href="/">
		<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">
			EduWeb
		</span>
	</NavBrand>
	<div class="flex md:order-2">
    <DarkMode />
		<NavHamburger on:click={toggle} />
	</div>
	<NavUl {hidden} class="order-1">
		<NavLi href="/" active={true}>Home</NavLi>
		<NavLi href="/">Courses</NavLi>
		<NavLi href="/">Blog</NavLi>
		<NavLi href="/">About Us</NavLi>
		<NavLi href="/">Login</NavLi>
		<NavLi href="/">Sign Up</NavLi>
	</NavUl>
</Navbar>