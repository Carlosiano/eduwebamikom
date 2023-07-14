<script>
	import '@fontsource/poppins';
	import Navbar from '../components/Navbar.svelte';
	import Footer from '../components/Footer.svelte';
	import airbnb from '$lib/assets/airbnb.svg';
	import amazon from '$lib/assets/amazon.svg';
	import facebook from '$lib/assets/facebook.svg';
	import google from '$lib/assets/google.svg';
	import grab from '$lib/assets/grab.svg';
	import netflix from '$lib/assets/netflix.svg';
	import mentor from '$lib/assets/mentor.png';
	import pelajar from '$lib/assets/pelajar.png';
	import fiturkami from '$lib/assets/fiturkami.png';
	import fiturkamiiconlist1 from '$lib/assets/fiturkamiiconlist1.png';
	import fiturkamiiconlist2 from '$lib/assets/fiturkamiiconlist2.png';
	import fiturkamiiconlist3 from '$lib/assets/fiturkamiiconlist3.png';
	import toolsformentor from '$lib/assets/toolsformentor.png';
	import venice from '$lib/assets/venice.png';
	import gradebook from '$lib/assets/gradebook.png';
	import discussions from '$lib/assets/discussions.png';
	import dimanapun from '$lib/assets/dimanapun.png';
	import freedom from '$lib/assets/freedom.png';
	import flexibilitas from '$lib/assets/flexibilitas.png';
	import bahankursus from '$lib/assets/bahankursus.png';
	import cloudstorage from '$lib/assets/cloudstorage.png';
	import glassman from '$lib/assets/glassman.png';

	import {
		Alert,
		Card,
		MenuButton,
		Dropdown,
		DropdownItem,
		Avatar,
		Button,
		Listgroup,
		Heading,
		Rating,
		Badge
	} from 'flowbite-svelte';

	import { VideoSolid, AddressCardSolid, PlaySolid } from 'flowbite-svelte-icons';

	let fiturKamiIcons = [
		{ icon: fiturkamiiconlist1, name: 'Ruang mentor yang unik dan fleksibel.' },
		{ icon: fiturkamiiconlist2, name: 'Alat-alat yang menarik.' },
		{ icon: fiturkamiiconlist3, name: 'Mentor dengan mudah memantau pelajar.' }
	];

	let listBrand = [
		{ src: airbnb, alt: 'airbnb' },
		{ src: amazon, alt: 'amazon' },
		{ src: facebook, alt: 'facebook' },
		{ src: google, alt: 'google' },
		{ src: grab, alt: 'grab' },
		{ src: netflix, alt: 'netflix' }
	];
</script>

<main class="flex flex-col items-center">
	<Navbar />
	<div class="flex container justify-center">
		<div class="flex flex-col">
			<div class="flex">
				<div class="flex m-auto gap-4 flex-col sm:flex-row items-center">
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
								<Button color="light" class="dark:text-white"
									><PlaySolid class="text-blue-500" /> Lihat Cara Kerjanya</Button
								>
							</div>
						</div>
					</Card>
					<div class="flex flex-col gap-3 md:w-96 lg:w-[600px] lg:h-80 lg:flex-row items-center">
						<Card class="h-fit w-fit md:self-start lg:self-end">
							<div class="flex flex-col gap-3">
								<div class="flex items-center space-x-4">
									<Avatar src="" alt="avatar" class="flex-shrink-0" />
									<div class="flex-1 min-w-0">
										<p class="text-sm font-medium text-gray-900 truncate dark:text-white">
											User Experience Class
										</p>
										<p class="text-sm text-gray-500 truncate dark:text-gray-400">
											Today at 12.00 PM
										</p>
									</div>
								</div>
								<Button class="w-fit" color="red">Join Now</Button>
							</div>
						</Card>
						<Card class="h-fit md:self-end lg:self-center">
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
									<h5
										class="mb-2 text-sm font-semibold tracking-tight text-gray-900 dark:text-white"
									>
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
			</div>
			<div class="flex flex-col mt-56 gap-2 items-center text-gray-900 dark:text-white">
				<span>Trusted by 5,000+ Companies Worldwide</span>
				<Listgroup items={listBrand} let:item class="flex">
					<img src={item.src} alt={item.alt} />
				</Listgroup>
			</div>
			<!-- all in one -->
			<div class="flex flex-col mt-44 gap-4 items-center">
				<Card class="m-auto shadow-none border-none" size="lg">
					<div class="text-center">
						<Heading tag="h4">All-In-One Cloud Software.</Heading>
						<span
							>Bergabung dengan EduWeb pasti akan memberikan manfaat bagi siswa yang tertarik dalam
							bidang pengembangan website.</span
						>
					</div>
				</Card>
				<div class="flex gap-5 justify-center flex-col sm:flex-row">
					<Card padding="sm">
						<div class="flex flex-col items-center pb-4">
							<img src={freedom} alt="" class="w-36" />
							<h5 class="mb-1 text-xl font-medium text-gray-900 dark:text-white">Freedom</h5>
							<span class="text-sm text-gray-500 dark:text-gray-400"
								>EduWeb menawarkan beragam kursus yang dapat dipilih sesuai dengan tingkat keahlian
								dan minat siswa.</span
							>
						</div>
					</Card>
					<Card padding="sm">
						<div class="flex flex-col items-center pb-4">
							<img src={flexibilitas} alt="" class="w-36" />
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
							<img src={bahankursus} alt="" class="w-36" />
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
				<div class="flex flex-col sm:flex-row items-center gap-2 sm:gap-3">
					<Card class="w-[336px] h-56 sm:w-1/2 p-0 border-none shadow-none" padding="none">
						<div
							class="w-full h-full bg-local bg-contain bg-no-repeat bg-center flex flex-col justify-center items-center"
							style="background-image: url({mentor}); "
						>
							<span class="text-white">Mentor</span>
							<Button color="none" class="border-2 text-white">Mulai</Button>
						</div>
					</Card>
					<Card class="w-[336px] h-56 sm:w-1/2 p-0 border-none shadow-none" padding="none">
						<div
							class="w-full h-full bg-local bg-contain bg-no-repeat bg-center flex flex-col justify-center items-center"
							style="background-image: url({pelajar});"
						>
							<span class="text-white">Pelajar</span>
							<Button color="none" class="border-2 bg-sky-500 text-white">Masukan Code</Button>
						</div>
					</Card>
				</div>
			</div>
			<div class="flex justify-center w-full mt-44">
				<Card size="xl">
					<div class="flex flex-col items-center sm:flex-row">
						<div
							class="sm:order-2 w-full sm:w-[50%] h-60 bg-local bg-contain bg-no-repeat bg-center flex flex-col justify-center items-center"
							style="background-image: url({dimanapun});"
						>
							<Button pill={true} outline={false} class="!p-2" color="light" size="lg"
								><PlaySolid class="text-blue-500" /></Button
							>
						</div>
						<div class="sm:order-1 sm:w-full">
							<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
								Dimanapun kamu berada, Komunitas eduweb selalu ada!
							</h5>
							<p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">
								EduWeb menciptakan komunitas pembelajaran di mana siswa dapat berinteraksi dengan
								sesama pembelajar, dan kolaborasi dengan orang-orang yang memiliki minat yang sama.
								Komunitas ini dapat memperkaya pengalaman belajar siswa dan membantu mereka
								membangun jaringan profesional.
							</p>
							<a href="/" class="inline-flex items-center underline"> learn more </a>
						</div>
					</div>
				</Card>
			</div>
			<div class="flex flex-col items-center w-full mt-44">
				<Card class="m-auto shadow-none border-none" size="lg">
					<div class="flex flex-col items-center">
						<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
							Fitur Kami
						</h5>
						<p class="mb-3 font-normal text-gray-700 dark:text-gray-400 leading-tight">
							Fitur yang sangat luar biasa ini, bisa membuat kegiatan belajar menjadi lebih efisien
						</p>
					</div>
				</Card>
				<Card size="xl" class="flex flex-col sm:items-start shadow-none border-none sm:flex-row">
					<img src={fiturkami} alt="" class="sm:w-1/2" />
					<div class="flex flex-col items-center">
						<h5
							class="mb-2 text-2xl sm:text-lg font-bold tracking-tight text-gray-900 dark:text-white"
						>
							Antarmuka pengguna yang dirancang untuk ruang kelas
						</h5>
						<Listgroup active items={fiturKamiIcons} let:item class="w-full p-0">
							<img src={item.icon} alt="" class="w-14 h-14 sm:w-10 sm:h-10" />
							{item.name}
						</Listgroup>
					</div>
				</Card>
				<Card size="xl" class="shadow-none border-none flex flex-col sm:items-center sm:flex-row">
					<img src={toolsformentor} alt="" class="sm:w-1/3 sm:order-2" />
					<div class="sm:order-1">
						<h5
							class="mb-2 text-2xl sm:text-lg font-bold tracking-tight text-gray-900 dark:text-white"
						>
							Tools Untuk mentor dan pelajar
						</h5>
						<p>
							Kelas memiliki seperangkat alat pengajaran dinamis yang dibuat untuk diterapkan dan
							digunakan selama kelas berlangsung. Pengajar dapat membagikan tugas secara real-time
							untuk diselesaikan dan diserahkan oleh siswa.
						</p>
					</div>
				</Card>
				<Card size="xl" class="shadow-none border-none flex flex-col sm:items-start sm:flex-row">
					<img src={venice} alt="" class="sm:w-1/2" />
					<div class="sm:mt-6">
						<h5
							class="mb-2 text-2xl sm:text-lg font-bold tracking-tight text-gray-900 dark:text-white"
						>
							Assessments, Quizzes, Tests
						</h5>
						<p>
							Easily launch live assignments, quizzes, and tests. Student results are automatically
							entered in the online gradebook.
						</p>
					</div>
				</Card>
				<Card size="xl" class="shadow-none border-none flex flex-col sm:items-start sm:flex-row">
					<img src={gradebook} alt="" class="sm:w-1/2 sm:order-2" />
					<div class="sm:mt-6 sm:order-1">
						<h5
							class="mb-2 text-2xl sm:text-lg font-bold tracking-tight text-gray-900 dark:text-white"
						>
							Class Management Tools for Educators
						</h5>
						<p>
							Class provides tools to help run and manage the class such as Class Roster,
							Attendance, and more. With the Gradebook, teachers can review and grade tests and
							quizzes in real-time.
						</p>
					</div>
				</Card>
				<Card size="xl" class="shadow-none border-none flex flex-col sm:items-start sm:flex-row">
					<img src={discussions} alt="" class="sm:w-1/2" />
					<div class="">
						<h5
							class="mb-2 text-2xl sm:text-lg font-bold tracking-tight text-gray-900 dark:text-white"
						>
							One-on-One Discussions
						</h5>
						<p>
							Teachers and teacher assistants can talk with students privately without leaving the
							Zoom environment.
						</p>
					</div>
				</Card>
				<Button class="w-fit">See more features</Button>
			</div>

			<div class="flex flex-col items-center w-full">
				<Card
					size="xl"
					class="sm:gap-4 shadow-none border-none flex flex-col sm:items-start sm:flex-row"
				>
					<img src={cloudstorage} alt="" class="sm:w-1/3" />
					<div class="sm:mt-6">
						<p>-------- INTEGRATIONS</p>
						<h5
							class="mb-2 text-2xl sm:text-lg font-bold tracking-tight text-gray-900 dark:text-white"
						>
							200+ educational tools and platform integrations
						</h5>
						<p>
							Schoology has every tool your classroom needs and comes pre-integrated with more than
							200+ tools, student information systems (SIS), and education platforms.
						</p>
						<Button>See All Integrations</Button>
					</div>
				</Card>
				<Card size="xl" class="gap-6 shadow-none border-none flex flex-col sm:items-start sm:flex-row">
					<div class="sm:mt-6">
						<p>-------- TESTIMONIAL</p>
						<h5
							class="mb-2 text-2xl sm:text-lg font-bold tracking-tight text-gray-900 dark:text-white"
						>
							What They Say?
						</h5>
						<p>Skilline has got more than 100k positive ratings from our users around the world.</p>
						<br />
						<p>Some of the students and teachers were greatly helped by the Skilline.</p>
						<br />
						<p>Are you too? Please give your assessment</p>
						<br />
						<Button>Write your assessment</Button>
					</div>
					<Card padding="md">
						<div
							class="rounded-md p-1 bg-slate-500 w-full h-full bg-local bg-contain bg-no-repeat bg-center flex flex-col justify-center items-center"
							style="background-image: url({glassman}); "
						>
							<div class="pt-36">
								<p class="bg-white dark:bg-gray-800 rounded-md p-1">
									“Terima kasih EduWeb, ini yang saya butuhkan untuk meningkatkan keterampilan
									pengembangan website saya. Sangat membantu dan menghemat waktu. Mama Saya Bangga
									sama saya sekarang”.
								</p>
							</div>
						</div>
						<div class="flex justify-between items-center">
							<p>Henry Mubarok</p>
							<div>
								<Rating rating="5" size="25" class="" />
								<p>666 reviews at Yelp</p>
							</div>
						</div>
					</Card>
				</Card>
			</div>
		</div>
	</div>
	<Footer />
</main>
