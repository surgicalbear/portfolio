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
                    title="Statify" 
                    description="Statify is an application that displays a spotify users top tracks and artists over different timeframes, allowing users to get a better understanding of their music history" 
                    gitLink="https://github.com/surgicalbear/statify" 
                    techStack="Next.js React JavaScript TypeScript Shadcn"
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
