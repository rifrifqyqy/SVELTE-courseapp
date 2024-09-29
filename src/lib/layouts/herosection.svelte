<script>
	import Button from '$lib/components/ui/button/button.svelte';
</script>

<main class="relative grid h-[600px] grid-cols-2 items-center" id="about">
	<div class="mx-32 flex flex-col gap-4">
		<h1 class="text-4xl font-bold">Bharacode</h1>
		<p class="text-[16px] text-zinc-500">
			Lorem, ipsum dolor sit amet consectetur adipisicing elit. Deleniti rem explicabo quidem
			dignissimos voluptate corrupti perferendis dolorum, non natus odio nobis inventore et.
			Laboriosam commodi molestiae neque, odio aperiam sit?
		</p>
		<Button class="bg-green1 hover:bg-green1/80 h-11 w-fit px-7 text-lg">Daftar Sekarang</Button>
	</div>
	<div class="">
		<img src="/images/konten_1.png" alt="" />
		<div class="absolute right-0 top-0 -z-30 h-[600px] w-[700px] rounded-bl-xl bg-zinc-100"></div>
	</div>
</main>
