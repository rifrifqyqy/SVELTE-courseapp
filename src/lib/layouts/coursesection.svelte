<script>
	import Button from '$lib/components/ui/button/button.svelte';
	const learnPath = [
		{
			id: 1,
			title: 'SVELTE',
			desc: 'Svelte adalah framework JavaScript modern untuk membangun antarmuka pengguna (UI). Berbeda dengan framework lain seperti React atau Vue yang melakukan banyak pekerjaan di browser menggunakan Virtual DOM, Svelte melakukan sebagian besar pekerjaan di waktu kompilasi. Ini berarti bahwa Svelte mengkompilasi komponen menjadi kode JavaScript yang sangat efisien yang secara langsung memanipulasi DOM saat dibutuhkan, mengurangi ukuran bundle dan meningkatkan kinerja aplikasi.',
			image: '/images/svelte.png'
		},
		{
			id: 2,
			title: 'CSS',
			desc: 'CSS adalah bahasa markup yang digunakan untuk membuat sebuah halaman website',
			image: '/images/css3.png'
		},
		{
			id: 3,
			title: 'Vue JS',
			desc: 'Javascript adalah bahasa markup yang digunakan untuk membuat sebuah halaman website',
			image: '/images/vue.png'
		}
	];
</script>

<section class="mx-32 mt-24 grid grid-cols-3 justify-items-center gap-8">
	<div class="col-span-3 flex justify-between rounded-xl bg-white px-12 shadow-lg">
		<div class="my-auto w-2/3">
			<h1 class="text-[32px] font-bold">Materi Pembelajaran</h1>
			<p class="text-[20px]">
				Jangan biarkan ketakutan atau ketidaktahuan menghalangi Anda. Mulailah belajar teknologi
				sekarang!
			</p>
			<Button class="bg-green1 hover:bg-green1/80 mt-4 px-7 text-lg">Daftar</Button>
		</div>
		<div class="h-fit w-fit bg-red-200">
			<img src="/images/teaching.png" alt="" class="h-[250px]" />
		</div>
	</div>
	{#each learnPath as path}
		<div class="card">
			<div class="aspect-video h-[200px] w-[300px] overflow-hidden rounded-md">
				<img src={path.image} alt={path.title} class="h-full w-full" />
			</div>
			<div class="px-1">
				<h1 class="text-2xl font-semibold">{path.title}</h1>
				<p class="line-clamp-2 text-zinc-500">{path.desc}</p>
			</div>

			<Button
				class="bg-green1 hover:bg-green1/80 mt-2 flex w-full items-center gap-4 rounded-md px-6 text-lg font-semibold text-white"
			>
				Lihat
			</Button>
		</div>
	{/each}
</section>

<style>
	.card {
		@apply flex max-w-min flex-col gap-2 rounded-xl bg-white p-3 text-zinc-800 shadow-md;
	}
</style>
