<script>
    export let title;
    export let description;
    export let gitLink;
    export let techStack;
    import DiGithubBadge from 'svelte-icons/di/DiGithubBadge.svelte';
</script>

<main>
    <div class="container">
        <div class="info">
            <h2> {title}</h2>
                <div class="gitIcon">
                    <a class="link" href={gitLink} target="_blank"><DiGithubBadge /></a>
                </div>
            <p>{description}</p>
            <div class="techWrapper">
                <p class="tech">{techStack}</p>
            </div>
            
        </div>
    </div>
</main>

<style>
    .info{
    display: flex;
    flex-wrap: wrap;
    padding-right: 3px;
    padding-left: 3px;
    margin-bottom: 5px;
    color:#8cade6;
    margin-top: 5px;
    margin-left: 15px; 
    
}
p{
    color: white;
    margin: 0;
    padding-bottom: 10px;
    font-size: 15px;
}
h2{
    margin-top: 5px;
    margin-bottom: 15px;
}
.container {
    max-width: 390px;
    margin-left: auto;
    margin-right: auto;
    min-width: 300px;
    background-color:#111;
    margin-left: 0px;
    margin-top: 25px;
    margin-bottom: 10px;
    border-radius: 20px;
    box-shadow: 0px 0px 10px 10px #0d0d0d88;
    border-color: #bbb;
    border-width: 0.1px; 
    border-style: solid;
}
.gitIcon{
    height: 27px;
    width: 27px;
    margin-left: auto;
    margin-right: 17px;
    margin-top: 6px;
    margin-bottom: 0;
}
.link{
    color: #8cade6;
}
.gitIcon:hover {
    filter: brightness(120%);
    transition: filter 0.3s ease; 
}
.tech{
    font-size: 12px;
    color: #bbb;
}
.techWrapper{
    padding-top: 10px;
}

</style>