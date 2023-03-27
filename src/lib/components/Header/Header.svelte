<script lang="ts">
	let darkMode = false;
	const toggleDarkMode = () => {
		darkMode = !darkMode;
		darkMode
			? document.documentElement.classList.add('dark')
			: document.documentElement.classList.remove('dark');
	};
</script>

<div class="w-full h-20 shadow-xl flex justify-between dark:bg-firstColor bg-thirdColor">
	<h1>Capture the Ether</h1>
	<div>
		<a>Home</a>
		<a>Challenges</a>
	</div>
	<button on:click={toggleDarkMode}>Dark Mode</button>
</div>
