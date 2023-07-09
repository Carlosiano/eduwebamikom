<script>
	import '../app.css';
	import '@fontsource/poppins';
	import Navbar from '../components/Navbar.svelte';
	import airbnb from '$lib/assets/airbnb.svg';
	import amazon from '$lib/assets/amazon.svg';
	import facebook from '$lib/assets/facebook.svg';
	import google from '$lib/assets/google.svg';
	import grab from '$lib/assets/grab.svg';
	import netflix from '$lib/assets/netflix.svg';
	import mentor from '$lib/assets/mentor.png'
	import pelajar from '$lib/assets/pelajar.png'

	import {
		Alert,
		Card,
		MenuButton,
		Dropdown,
		DropdownItem,
		Avatar,
		Button,
		Listgroup,
		Heading
	} from 'flowbite-svelte';

	let listBrand = [
		{ src: airbnb, alt: 'airbnb' },
		{ src: amazon, alt: 'amazon' },
		{ src: facebook, alt: 'facebook' },
		{ src: google, alt: 'google' },
		{ src: grab, alt: 'grab' },
		{ src: netflix, alt: 'netflix' }
	];
</script>

<main class="flex flex-col">
	<Navbar />
	<div class="flex m-auto container">
		<div class="flex flex-col">
			<div class="flex">
				<div class="flex m-auto gap-4">
					<Card padding="sm" class="h-fit border-none shadow-none">
						<div class="flex flex-col items-center pb-4">
							<h5 class="mb-1 text-5xl font-medium text-gray-900 dark:text-white">
								"Master the web from Anywhere, Anytime"
							</h5>
							<span class="text-sm text-gray-500 dark:text-gray-400"
								>Pelajari pengembangan web dengan cara yang inovatif dan interaktif melalui EduWeb,
								platform e-learning sejati.
							</span>
							<div class="flex mt-4 space-x-3 lg:mt-6">
								<Button>Ayo Gabung</Button>
								<Button color="light" class="dark:text-white">Lihat Cara Kerjanya</Button>
							</div>
						</div>
					</Card>

					<Card class="h-fit self-end">
						<div class="flex flex-col gap-3">
							<div class="flex items-center space-x-4">
								<Avatar src="" alt="avatar" class="flex-shrink-0" />
								<div class="flex-1 min-w-0">
									<p class="text-sm font-medium text-gray-900 truncate dark:text-white">
										User Experience Class
									</p>
									<p class="text-sm text-gray-500 truncate dark:text-gray-400">Today at 12.00 PM</p>
								</div>
							</div>
							<Button class="w-fit" color="red">Join Now</Button>
						</div>
					</Card>

					<Card class="h-fit self-center">
						<a class="flex flex-row" href="/">
							<svg
								width="50px"
								height="50px"
								viewBox="0 0 512 512"
								xmlns="http://www.w3.org/2000/svg"
								><g fill="none" fill-rule="evenodd"
									><path fill="#ffda3e" d="M56 402.667h400V109.333H56z" /><path
										fill="#fc0"
										d="M256 182.667l-200 220h400z"
									/><path
										d="M456 109.333L276.848 284.116c-11.675 11.4-30.02 11.4-41.696 0L56 109.333h400z"
										fill="#f33"
									/></g
								></svg
							>
							<div>
								<h5 class="mb-2 text-xl font-semibold tracking-tight text-gray-900 dark:text-white">
									Congratulation
								</h5>
								<p class="mb-3 font-normal text-gray-500 dark:text-gray-400">
									Your admission completed
								</p>
							</div>
						</a>
					</Card>
				</div>
			</div>
			<div class="flex flex-col justify-center mt-56 gap-2">
				<span class="m-auto">Trusted by 5,000+ Companies Worldwide</span>
				<Listgroup items={listBrand} let:item class="flex">
					<img src={item.src} alt={item.alt} />
				</Listgroup>
			</div>
			<div class="flex flex-col mt-44 gap-4">
				<Card class="m-auto shadow-none border-none" size="lg">
					<div class="text-center">
						<Heading tag="h4">All-In-One Cloud Software.</Heading>
						<span
							>Bergabung dengan EduWeb pasti akan memberikan manfaat bagi siswa yang tertarik dalam
							bidang pengembangan website.</span
						>
					</div>
				</Card>
				<div class="flex gap-5 justify-center">
					<Card padding="sm">
						<div class="flex flex-col items-center pb-4">
							<Avatar size="lg" src="/images/profile-picture-3.webp" />
							<h5 class="mb-1 text-xl font-medium text-gray-900 dark:text-white">Freedom</h5>
							<span class="text-sm text-gray-500 dark:text-gray-400"
								>EduWeb menawarkan beragam kursus yang dapat dipilih sesuai dengan tingkat keahlian
								dan minat siswa.</span
							>
						</div>
					</Card>
					<Card padding="sm">
						<div class="flex flex-col items-center pb-4">
							<Avatar size="lg" src="/images/profile-picture-3.webp" />
							<h5 class="mb-1 text-xl font-medium text-gray-900 dark:text-white">
								Fleksibilitas Pembelajaran
							</h5>
							<span class="text-sm text-gray-500 dark:text-gray-400"
								>EduWeb menawarkan fleksibilitas untuk belajar dan mengembangkan kursus secara
								online sesuai dengan jadwal mereka sendiri.</span
							>
						</div>
					</Card>
					<Card padding="sm">
						<div class="flex flex-col items-center pb-4">
							<Avatar size="lg" src="/images/profile-picture-3.webp" />
							<h5 class="mb-1 text-xl font-medium text-gray-900 dark:text-white">
								Bahan Kursus Online
							</h5>
							<span class="text-sm text-gray-500 dark:text-gray-400"
								>EduWeb menyimpan bahan kursus online dan memungkinkan siswa mengaksesnya dengan
								mudah dan belajar dengan fitur modern melalui platform EduWeb</span
							>
						</div>
					</Card>
				</div>
			</div>
			<div class="mt-44 m-auto">
				<div>
					<Card size="lg" class="shadow-none border-none">
						<div class="text-center">
							<Heading tag="h4">Gatau EduWeb?</Heading>
							<span
								>EduWeb adalah platform e-learning untuk belajar pengembangan website. Dengan kelas
								online, bahan kursus yang disimpan dan dikelola secara online, serta umpan balik dan
								pengajaran berkualitas tinggi dari para ahli industri, EduWeb memungkinkan siswa
								meningkatkan keterampilan pengembangan website mereka dengan fleksibilitas dan
								efisiensi. Bergabunglah sekarang</span
							>
						</div>
					</Card>
				</div>
				<div>
					<Card>
						<div class="bg-local bg-[url('/mentor.png')]"></div>
					</Card>
				</div>
			</div>
		</div>
	</div>
</main>
