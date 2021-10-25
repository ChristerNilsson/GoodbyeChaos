
<script>
	// https://www.youtube.com/watch?v=Pp40Ejkk2Wc&t=33s&ab_channel=edynurcahyo
	import { GoogleAuth } from '@beyonk/svelte-social-auth'
	let data
</script>

<GoogleAuth clientId="810501500016-fod41p7083pb94hkjsc8ls2tq21ftssd.apps.googleusercontent.com" on:auth-success={e => data = e.detail.user} />

<h1>{#if data}Welcome {data.nt.Yt} !{:else}Not logged in.{/if}</h1>
