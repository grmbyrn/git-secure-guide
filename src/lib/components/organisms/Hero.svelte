<script>
	import FeaturesIcon from '$lib/icons/features.svelte';
	import GitHubIcon from '$lib/icons/socials/github.svelte';
	import Button from '$lib/components/atoms/Button.svelte';
	import Sparkles from '../atoms/Sparkles.svelte';
	import Image from '../atoms/Image.svelte';
</script>

<section id="hero">
	<div class="image">
		<Image src="/images/SGG-IndexHeader-1600x500.jpg" alt="Sample for the static template" />
		<h1 class="hello">Secure Git Guide</h1>
	</div>
	<div class="ctas">
		<Sparkles>
			<Button href="https://github.com/Nautilus-Cyberneering/secure-git-guide/tree/main">
				<GitHubIcon slot="icon" />
				Edit on GitHub
			</Button>
		</Sparkles>
		<Button color="primary" href="https://histoire-sveltekit-static-blog-template.vercel.app/">
			<FeaturesIcon slot="icon" />
			Components
		</Button>
	</div>
</section>

<style lang="scss">
	@import '$lib/scss/breakpoints.scss';

	#hero {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		gap: 15px;
		position: relative;
		padding: 80px 0;

		@include for-phone-only {
			padding: 40px 0 50px;
		}

		.hello {
			text-align: center;
		}
		.ctas {
			display: flex;
			flex-wrap: wrap;
			align-items: center;
			justify-content: center;
			gap: 10px;
			width: 100%;
		}
	}
</style>
