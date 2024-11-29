<script lang="ts">
	import '../app.css';
	import * as Accordion from "$lib/components/ui/accordion/index.js";

	let { children } = $props();
</script>

<Accordion.Root type="single" class='flex justify-center w-full'>
  <Accordion.Item value="item-1" class='flex justify-center w-full flex-wrap'>
    <Accordion.Trigger class='w-full'>
		</Accordion.Trigger>
		<a href="/" class='w-full text-center'>
			<Accordion.Content>
				Home
			</Accordion.Content>
		</a>
		<a href="/portfolio" class='w-full text-center'>
			<Accordion.Content>
				Portfolio
			</Accordion.Content>
		</a>
		<a href="/contact" class='w-full text-center'>
			<Accordion.Content>
				Contact
			</Accordion.Content>
		</a>
  </Accordion.Item>
</Accordion.Root>
{@render children()}