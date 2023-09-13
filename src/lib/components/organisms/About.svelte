<script>
	import SparklingHighlight from '$lib/components/molecules/SparklingHighlight.svelte';
	import Socials from '$lib/components/molecules/Socials.svelte';
</script>

<section id="about">
	<div class="info">
		<h2>Secure Git Guide</h2>
		<p>
			Here we attempt to help any developer to use GIT and GitHub more securely. Any challenges that
			we are facing in terms of security will be registered here. You will find information on how
			to use GIT securely in developement work. This guide is the result of our team actively
			developing a pure GIT / GitHub infrastructure for repository optimisation and automation
			during which we encountered security challenges.
		</p>
		<div class="socials">
			<span>Socials:</span>
			<Socials />
		</div>
	</div>
	<div>
		<h2>Topics that are covered among others:</h2>
		<ul class="list">
			<li>GPG and how we use it for projects.</li>
			<li>GPG basic and more advanced uses in relation to GIT and GitHub.</li>
			<li>GitHub secrets, tokens, etc.</li>
			<li>GIT vs GitHub differences.</li>
			<li>etc.</li>
		</ul>
	</div>
</section>

<style lang="scss">
	@import '$lib/scss/breakpoints.scss';

	#about {
		position: relative;
		display: grid;
		grid-template-columns: 500px 500px;
		align-items: center;
		justify-content: space-between;
		padding-bottom: 50px;

		@include for-phone-only {
			grid-template-columns: 1fr;
			justify-items: center;
			gap: 20px;
		}

		.info {
			display: flex;
			flex-direction: column;
			gap: 10px;
			h2 {
				@include for-phone-only {
					text-align: center;
				}
			}

			p {
				@include for-phone-only {
					text-align: justify;
				}
			}

			@include for-phone-only {
				gap: 20px;
			}
		}

		.socials {
			display: flex;
			align-items: center;
			gap: 15px;

			@include for-phone-only {
				justify-content: center;
				margin-bottom: 10px;
				span {
					display: none;
				}
			}
		}
	}
</style>
