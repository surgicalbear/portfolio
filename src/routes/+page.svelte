<svelte:head>
  <!-- Link to the Google Fonts stylesheet -->
  <link
    href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@500&family=Roboto+Serif:wght@500&family=Roboto+Slab:wght@500&family=Roboto:ital,wght@0,400;0,500;1,400&display=swap"
    rel="stylesheet"
  />
</svelte:head>
<main>
    <body>
        <div class="container">
            <div class="middle">
                <div class="content">
                    <h1>
                    <span class = "eryk"> &lt;eryk/&gt</span>
                    </h1>
                    <p>
                        Eryk Sadelski
                        <br>
                        Carleton University '26
                        <br>
                    </p>
                    <h2>about me</h2>
                    <p><span class ="First-Word">Hi!</span> I'm a second-year computer science student at Carleton University 
                        with an interest in software engineering,
                        AI, cryptography and other related fields in tech. Check out my projects
                        <a class="project-link" href="/projects">here</a>
                    </p>
                    <h2>technologies</h2>
                    <div style ="display:flex; flex-wrap:wrap;">
                        <p class="test">python</p>
                        <p class="test">java</p>
                        <p class="test">c</p>
                        <p class="test">javascript</p>
                        <p class="test">react</p>
                        <p class="test">nextjs</p>
                        <p class="test">html</p>
                        <p class="test">css</p>
                        <p class="test">git</p>
                    </div>
                    <h2 class="links-header-tag">links</h2>
                    <p class ="links">
                        <a href=" ">resume
                            <span class ="lambda">λ</span>
                        </a>
                        <br>
                        <a href="https://github.com/surgicalbear" target="_blank">github
                            <span class ="lambda">λ</span>
                        </a>
                        <br>
                        <a href="https://www.linkedin.com/in/eryksadelski/" target="_blank">linkedin
                            <span class ="lambda">λ</span>
                        </a>
                        <br>
                        <a href="mailto:sadelski.dev@gmail.com" target="_blank">contact me
                            <span class ="lambda">λ</span>
                        </a>
                        <br>
                    </p>
                </div>
            </div>
        </div>
    </body>
</main>

<style>

body{
    background-color: #111;
    color: white;
    font-family: 'IBM Plex Mono', monospace;
    font-size: 14px;
}

*{
    box-sizing: border-box;
}

.container{
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
.middle{
    display: table-cell;
    vertical-align: middle;
}
.content{
    max-width: 390px;
    margin-left: auto;
    margin-right: auto;
    width: 23%;
    min-width: 300px;
    background-color: #111;
    border-top: 2px solid #fff;
    border-top-color: rgb(255, 255, 255);
    border-top-style: solid;
    border-top-width: 2px;
    border-bottom: 2px solid #fff;
    border-bottom-color: rgb(255, 255, 255);
    border-bottom-style: solid;
    border-bottom-width: 2px;
}

h1{
    font-size: 30px;
    font-weight: 700;
    width: 100%;
    white-space: nowrap;
    overflow: hidden;
    animation: typing 3s;
}

@keyframes typing {
    from { width: 0}
    to {width: 100%}
}

h2{
    font-size: 20px;
    font-weight: 500;
}

.links-header-tag{
    max-width: 105px;
}
.links{
    max-width: 105px;
}
.eryk{
    color: #8cade6;
}

p span.First-Word {
  color: #8cade6;
  font-weight: 700;
}

a{
    color: #8cade6;
}
a:hover{
    color: white;
}
.test{
    border-left: solid #c9c9c9 .125em;
    border-right: solid #c9c9c9 .125em;
    border-top: solid #c9c9c9 .125em;
    border: solid #c9c9c9 .125em;
    padding-right: 3px;
    padding-left: 3px;
    margin-bottom: 5px;
    margin-left: 4px;
    text-decoration: none;
    text-decoration-line: none;
    text-decoration-style: solid;
    text-decoration-color: currentcolor;
    text-decoration-thickness: auto;
    margin:0.1rem;
    padding:1;
    color:#8cade6;
}
</style>
