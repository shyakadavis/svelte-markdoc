<script>
	import '../app.postcss';
	import { ModeWatcher } from 'mode-watcher';
</script>

<main class="max-w-3xl mx-auto">
	<slot />
</main>

<ModeWatcher />
