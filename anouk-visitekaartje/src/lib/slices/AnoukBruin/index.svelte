<script>
  /** @type {import("@prismicio/client").Content.AnoukBruinSlice} */
  export let slice;
</script>

<section
  data-slice-type={slice.slice_type}
  data-slice-variation={slice.variation}
>
  Placeholder component for {slice.slice_type} (variation: {slice.variation})
  Slices
  <p>{slice.primary.title}</p>
  
</section>

<pre>
	{JSON.stringify(slice, null, 2)}
</pre>