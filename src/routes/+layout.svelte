<script lang="ts">
	import LeafletMap from '$lib/LeafletMap.svelte';
</script>

<pre>routes/+layout.svelte HEADER</pre>
<div style="border: 1px solid #f00">
	<div>Here is the routes/+layout.svelte map:</div>
	<LeafletMap />
	<div>Here was the routes/+layout.svelte map</div>

	<div>Here is the routes/+layout.svelte &lt;slot&gt; map:</div>
	<slot />
	<div>Here was the routes/+layout.svelte &lt;slot&gt; map</div>
</div>
<pre>routes/+layout.svelte FOOTER</pre>
