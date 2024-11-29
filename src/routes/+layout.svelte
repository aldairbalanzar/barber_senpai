<script lang="ts">
	import '../app.css';
	import * as Menubar from "$lib/components/ui/menubar"
	import * as Accordion from "$lib/components/ui/accordion/index.js";

	let { children } = $props();
</script>

{@render children()}
<Accordion.Root type="single" class='flex justify-center w-full'>
  <Accordion.Item value="item-1" class='flex justify-center w-full flex-wrap'>
    <Accordion.Trigger class='w-full'>Is it accessible?</Accordion.Trigger>
    <Accordion.Content class='w-full text-center'>
      Yes. It adheres to the WAI-ARIA design pattern.
    </Accordion.Content>
  </Accordion.Item>
</Accordion.Root>