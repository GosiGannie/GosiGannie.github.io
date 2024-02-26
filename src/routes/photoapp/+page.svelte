<title> Photo App </title> 

<h1>Photo App</h1>

<div class = "photos">
    {#each images as img}
        <div class = 'image-wrapper'>
            <img src = {img} alt = 'flexbox rules'>
        </div>
        {/each}
</div>

<style>
    .photos{
        display:flex;
        max-width: 90vw;
    }

    .photos img {
        max-width: 90%;
        align-items: center;
        justify-content: space-around;
    }
</style>

<script>
    let image = 'https://picsum.photos/id/70/367/267'
    let photo = 'https://picsum.photos/id/88/367/267'
    let picture = 'https://picsum.photos/id/93/367/267'
    let images = [image, photo, picture, image, photo, picture]
</script>