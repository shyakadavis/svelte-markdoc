<script lang="ts">
	import * as Accordion from '$lib/components/ui/accordion';
</script>

<section class="z-10 mx-auto my-4 max-w-4xl overflow-hidden rounded-lg border bg-popover">
	<div class="grid place-items-center p-4 shadow-inner sm:p-8">
		<slot />
		<slot name="message" />
	</div>
	<Accordion.Root class="w-full">
		<Accordion.Item value="item-1" class="border-b-0">
			<Accordion.Trigger class="max-h-10 bg-muted px-2">
				<span class="ml-auto mr-2 text-sm font-light">Code</span>
			</Accordion.Trigger>
			<Accordion.Content>
				<slot name="code" />
				How can I get the code here?
			</Accordion.Content>
		</Accordion.Item>
	</Accordion.Root>
</section>
