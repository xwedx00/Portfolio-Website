<script>
	import Social from '../atoms/Social.svelte';
</script>

<div class="socials-container">
	<Social icon="github" tip="xwedx00" link="https://github.com/xwedx00" />
	<Social icon="discord" tip=xwedx00 link={`https://discord.com/users/asd`} />
	<Social icon="email" tip="xwedx00@protonmail.com" link="mailto:xwedx00@protonmail.com" />
</div>

<style>
	.socials-container {
		display: flex;
		gap: 0.75rem;
	}
</style>
