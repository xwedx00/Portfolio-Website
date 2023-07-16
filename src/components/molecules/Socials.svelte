<script>
	import Social from '../atoms/Social.svelte';
</script>

<div class="socials-container">
	<Social icon="github" tip="xwedx00" link="https://github.com/xwedx00" />
	<Social icon="discord" tip=xwedx00 link={`https://discord.com/users/asd`} />
	<Social icon="email" tip="hey@afn.im" link="mailto:hey@afn.im" />
	<Social icon="kofi" tip="affan" link="https://ko-fi.com/affan" />
</div>

<style>
	.socials-container {
		display: flex;
		gap: 0.75rem;
	}
</style>
