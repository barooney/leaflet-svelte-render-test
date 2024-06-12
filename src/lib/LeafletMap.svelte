<script lang="ts">
	import { onMount } from 'svelte';
	import L from 'leaflet';
	import 'leaflet/dist/leaflet.css';

	const id = 'map-' + Math.random().toString(36).substring(2, 9);

	onMount(() => {
		const map = L.map(id).setView([52.0207768, 8.5324237], 21);
		L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
			attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a>'
		}).addTo(map);
	});
</script>

<pre>LeafletMap START with id {id}</pre>
<div {id} style="width: 500px; height: 350px; border: 1px solid #0f0" />
<pre>LeafletMap END with id {id}</pre>
