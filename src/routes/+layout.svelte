<nav>
    <div class="nav-container">
        <a href="/" class="nav-logo" title="Back to Homepage">Арина Федорова</a>
        <div class="nav-links">
            {#each nav as link}
				{#if link.isShow}
				<a href={link.href} class="link">{link.title}</a>
				{/if}
            {/each}
        </div>
    </div>
</nav>

<div class="container">
    <!-- Pages will be injected below -->
    <slot></slot>
</div>
<script>
    	const nav = [
		{
			title: ' я интересная',
			href: '/about',
			isShow: true
		},
		{
			title: 'я разнообразная',
			href: '/blog',
			isShow: true
		},
		{
			title: 'я умная',
			href: '/project',
			isShow: true
		},
		{
			title: 'Связь со мной',
			href: '/contact',
			isShow: true
		}
	]
</script>
<style>
    .container {
        max-width: 1400px;
        margin: 50px auto;
    }
	

</style>
