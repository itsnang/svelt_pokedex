<script>
	export let pokeman;
</script>

<div class="h-full flex min-h-[12rem] flex-col bg-white rounded-2xl w-full">
	<a href="#">
		<img class="rounded-t-lg" src={pokeman.image} alt={pokeman.name} />
	</a>
	<div class="p-5">
		<h5 class="mb-2 text-2xl tracking-tight text-gray-900">
			{pokeman.name}
		</h5>
	</div>
</div>
