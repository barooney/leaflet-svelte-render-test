<script lang="ts">
	import { browser } from '$app/environment';
	import { onMount } from 'svelte';
	import Map from '$lib/LeafletMap.svelte';
</script>

<pre>routes/+page.svelte START</pre>
<div>Here goes the map:</div>
<Map />
<div>Here went the map</div>
<pre>routes/+page.svelte END</pre>
