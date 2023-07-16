<script>
	import HeroImage from '../../components/atoms/HeroImage.svelte';
	import Button from '../atoms/Button.svelte';
	import Socials from '../molecules/Socials.svelte';

	function handleClick() {
		const el = document.querySelector('#work');
		if (!el) return;
		el.scrollIntoView(true);
	}
</script>

<section id="home" class="wrapper">
	<div>
		<h1>𝕩00</h1>
		<h5>
			"Bringing Linux to Life, One Byte at a Time through Tech Tinkering!"<br />Attempting to
			program.
		</h5>
		<div class="socials">
			<Socials />
		</div>
		<Button side on:click={handleClick} on:keypress={handleClick}>Discover my work ↓</Button>
	</div>
	<HeroImage />
</section>

<style lang="scss">
	@import '../../styles/mixins.scss';

	section {
		scroll-margin-top: 20rem;
		display: flex;
		justify-content: space-between;
		align-items: center;
		margin-bottom: 5.75rem;
		margin-top: 7rem;

		@media screen and (max-width: 868px) {
			margin-top: 4rem;
		}

		@media screen and (max-width: 768px) {
			margin-bottom: 2.75rem;
		}

		@media screen and (max-width: 500px) {
			display: block;
		}
	}

	.socials {
		margin-top: 1rem;
		margin-bottom: 1.7rem;
	}

	h1::before {
		@include outlineText($content: '⌥', $translateX: -125%,$translateY: -50%,
			$fontSize: 100px, $letterSpacing: -0.1em);
	}

	@media screen and (max-width: 1240px) {
		h1 {
			min-height: 0vw;
			font-size: clamp(4rem, 10vw, 6.25rem);
		}
	}
</style>
