
<script>
    import { SliceZone } from '@prismicio/svelte'
    import { components } from '$lib/slices' 
    
    export let data

    console.log(data)
</script>

<!-- <h1>{ data.slices }</h1> -->
<div class="intro"> 
 <h1>{ data.title }</h1>
 <img src="{data.image.url}" width="50" alt="{data.image.alt}"> 

</div>

<div class="social"> 
 <img class="socials" src="{data.github.url}" alt="{data.github.alt}">
 <img class="socials" src="{data.facebook.url}" alt="{data.facebook.alt}">
 <img class="socials" src="{data.instagram.url}" alt="{data.instagram.alt}">
 <img class="socials" src="{data.email.url}" alt="{data.email.alt}">

</div>


 
<!-- <SliceZone slices={data.slices} {components} /> -->

<style>

    .socials {
        width: 40px;
        height: 40px;
        border-color: grey;
    }

    .intro img {
        width: 100px;
        height: 100px;
        border-radius: 100%;
        margin-left: 30px;
        border-color: orange;
    }

    h1 {  
        text-align: right;
    }


    /* Desktop */
@media only screen and (min-width: 560px) { 

}
</style>