<script>
	import Skills from "$lib/components/Skills.svelte";
	import Frameworks from "$lib/components/Frameworks.svelte";
</script>

<article class="main-container">
	<div class="welcome-container">
		<h1>Welcome to my Website!</h1>
		<h2>I am computer science student aspiring to become a web developer</h2>
	</div>
	<img src="/images/profile-picture.jpg" alt="zi wei profile pic" />
</article>

<Skills />
<Frameworks />

<style>
	.main-container {
		display: flex;
		justify-content: center;
		align-items: center;
		min-height: 100vh;
		gap: 1.5rem;
	}

	.main-container > img {
		width: 300px;
		height: 300px;
		border-radius: 50%;
		margin-right: 2rem;
		object-fit: cover;
	}

	.welcome-container {
		text-align: center;
		padding: 1rem;
	}

	h1 {
		font-size: 3rem;
		font-weight: 700;
		color: #000;
		text-align: center;
	}

	h2 {
		font-size: 1.5rem;
		font-weight: 400;
		color: #000;
		text-align: center;
	}

	@media only screen and (max-width: 768px) {
		.main-container {
			flex-direction: column;
			align-items: center;
			justify-content: center;
			min-height: auto;
			padding-bottom: 3rem;
		}

		.main-container h1 {
			font-size: 2rem;
		}

		.main-container h2 {
			font-size: 1rem;
		}

		.main-container > img {
			margin: auto;
			margin-top: 20px;
		}
	}
</style>
