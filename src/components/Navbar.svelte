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
		DropdownDivider
	} from 'flowbite-svelte';
</script>

<Navbar let:hidden let:toggle>
	<NavBrand href="/">
		<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">
			EduWeb
		</span>
	</NavBrand>
	<div class="flex md:order-2">
		<Avatar id="avatar-menu" src="/images/profile-picture-3.webp" />
		<NavHamburger on:click={toggle} />
	</div>
	<Dropdown placement="bottom" triggeredBy="#avatar-menu">
		<DropdownHeader>
			<span class="block text-sm"> Bonnie Green </span>
			<span class="block truncate text-sm font-medium"> name@flowbite.com </span>
		</DropdownHeader>
		<DropdownItem>Login</DropdownItem>
		<DropdownDivider />
		<DropdownItem>Sign Up</DropdownItem>
	</Dropdown>
	<NavUl {hidden} class="order-1">
		<NavLi href="/" active={true}>Home</NavLi>
		<NavLi href="/">Courses</NavLi>
		<NavLi href="/">Blog</NavLi>
		<NavLi href="/">About Us</NavLi>
	</NavUl>
</Navbar>