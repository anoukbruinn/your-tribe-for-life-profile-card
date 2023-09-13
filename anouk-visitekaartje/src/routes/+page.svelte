
<script>
    import { SliceZone } from '@prismicio/svelte'
    import { components } from '$lib/slices' 
    
    export let data

    console.log(data)
</script>

<!-- <h1>{ data.slices }</h1> -->
<body> 
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

<hr> 

<div class="bericht">

    <h3>{data.bericht}</h3>

</div>

<div class="fotos">

    <img class="foto" src="{data.foto1.url}" alt="{data.foto1.alt}">
    <img class="foto" src="{data.foto2.url}" alt="{data.foto2.alt}">
    <img class="foto" src="{data.foto3.url}" alt="{data.foto3.alt}">
</div>

<div class="fotos2">

    <img class="foto" src="{data.foto4.url}" alt="{data.foto4.alt}">
    <img class="foto" src="{data.foto5.url}" alt="{data.foto5.alt}">
    <img class="foto" src="{data.foto6.url}" alt="{data.foto6.alt}">
</div>

<div class="fotos3">

    <img class="foto" src="{data.foto7.url}" alt="{data.foto7.alt}">
    <img class="foto" src="{data.foto8.url}" alt="{data.foto8.alt}">
    <img class="foto" src="{data.foto9.url}" alt="{data.foto9.alt}">
</div>
</body>
 
<!-- <SliceZone slices={data.slices} {components} /> -->

<style>

    body {
        background-color: rgb(247, 244, 244);
        
    }
    .social{
        margin-top: 15px;
        justify-content: center;
    }
    .socials {
        width: 60px;
        height: 60px;
        border-color: grey;
        margin-right: 5px;
        border-radius: 100%;
        
    }

    .intro img {
        width: 110px;
        height: 110px;
        border-radius: 100%;
        margin-left: 30px;
        border-color: orange;
    }

    h1 {  
        text-align: right;
        margin-top: 20px;
    }

    img.foto {
        width: 110px;
        height:110px; 
    }

    .fotos {
        justify-content: center;
    }
    /* Desktop */
@media only screen and (min-width: 560px) { 
    body {
        background-color: rgb(247, 244, 244);
        
    }
    .social{
        margin-top: 15px;
        justify-content: center;
    }
    .socials {
        width: 120px;
        height: 120px;
        border-color: grey;
        margin-right: 5px;
        border-radius: 100%;
        margin-left: 30px;
        
    }

    .intro img {
        width: 150px;
        height: 150px;
        border-radius: 100%;
        margin-left: 30px;
        border-color: orange;
    }

    h1 {  
        text-align: right;
        margin-top: 20px;
        
    }

    img.foto {
        width: 520px;
        height:520px; 
        justify-content: center;
    }

    .fotos {
        justify-content: center;
    }

    div.fotos {
        justify-content: center;
    }
}
</style>