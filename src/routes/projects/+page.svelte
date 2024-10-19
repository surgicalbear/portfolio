<script>
    import Card from "$lib/Card.svelte"
</script>

<svelte:head>
  <link
    href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@500&family=Roboto+Serif:wght@500&family=Roboto+Slab:wght@500&family=Roboto:ital,wght@0,400;0,500;1,400&display=swap"
    rel="stylesheet"
  />
</svelte:head>
<main>
    <body>
        <div class="container">
            <div class ="middle">
                <div class="content">
                    <p>
                        <a href="/">home</a>
                    </p>
                    <h1>eryks</h1>
                    <div class="word-container">
                        <div class="typed-out">projects</div>
                    </div> 
                    <Card 
                    title="LeetTracker" 
                    description="A web application that allows users to create custom sets of LeetCode problems and track their progression over time" 
                    gitLink="https://github.com/surgicalbear/LeetTracker" 
                    techStack="Go JavaScript React PostgreSQL GraphQL Redis Docker"
                    />
                    <Card 
                    title="MelodyMap" 
                    description="A web application that showcases a Spotify user's top tracks and artists while providing personalized recommendations to help users explore and better understand their music history" 
                    gitLink="https://github.com/surgicalbear/MelodyMap" 
                    techStack="Python TypeScript Next React FastAPI"
                    />
                    <Card 
                    title="Central RateMyProf" 
                    description="A chrome extension that integrates professor reviews into Carletons course registration page" 
                    gitLink="https://github.com/surgicalbear/Central-RateMyProf" 
                    techStack="JavaScript GraphQL"
                    />
                </div>
            </div>
        </div>
    </body>
</main>

<style>

body {
    font-family: ibm plex mono,monospace;
    color: #fff;
    background-color: #111;
    font-size: 14px;
    padding: 20px;
    overflow-y: scroll;
}

* {
    box-sizing: border-box;
}
.container {
    display: table;
    position: absolute;
    top: 0;
    left: 0;
    padding-top: 50px;
    padding-bottom: 50px;
    height: 100%;
    width: 100%;
    background-color: #111;
  }

.middle {
    display: table-cell;
    vertical-align: middle;
}
.content {
    max-width: 390px;
    margin-left: auto;
    margin-right: auto;
    width: 40%;
    min-width: 300px;
    background-color: #111;
    border-top: 2px solid #fff;
    border-bottom: 2px solid #fff;
    padding-bottom: 15px;
}

h1{
    margin: 0;
    font-size: 28px;
    font-weight: 700;
    display: inline-block;
    vertical-align: middle;
}

.word-container{
    display: inline-block;
    vertical-align: middle;
}
.typed-out{
    color:#8cade6;
    font-size: 28px;
    font-weight: 700;
    width:100%;
    overflow: hidden;
    white-space: nowrap;
    animation: typing 1.4s;
}

@keyframes typing {
    from { width: 0}
    to {width: 100%}
}

a{
    color: #8cade6;
}
a:hover{
    color: white;
}

</style>
