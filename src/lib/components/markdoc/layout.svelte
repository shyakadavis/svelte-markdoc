<script lang="ts">
	import SvelteSeo from 'svelte-seo';
	export let title: string | null = null;
</script>

<SvelteSeo title={title ? title : ''} />

<article
	class="prose prose-zinc mx-auto max-w-none text-foreground prose-blockquote:text-muted-foreground"
>
	<slot />
</article>
