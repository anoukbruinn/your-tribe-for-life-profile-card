
<script>
    import { SliceZone } from '@prismicio/svelte'
    import { components } from '$lib/slices' 
    
    export let data

    console.log(data)
</script>

<!-- <h1>{ data.slices }</h1> -->
 <h1>{ data.title }</h1>
 <img src="{data.image.url}" width="50" alt="{data.image.alt}"> 

<!-- <SliceZone slices={data.slices} {components} /> -->

<style>

    img {
        width: 100px;
        height: 100px;
        border-radius: 100%;
        margin-left: 30px;
        border-color: orange;
    }

    h1 { 
        text-align: right;
    }
</style>