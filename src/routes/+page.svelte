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
                    <h2>About me</h2>
                    <p><span class ="First-Word">Hi!</span> I'm a third-year computer science student at Carleton University 
                        with an interest in software engineering,
                        AI, cryptography and other related fields in tech. Check out my projects
                        <a class="project-link" href="/projects">here</a>
                    </p>
                    <h2>Experience</h2>
                    <div class="timeline">
                        <div class="timeline-item">
                            <div class="timeline-content">
                                <div class="timeline-description-container">
                                    <div class="timeline-description">BlackBerry QNX</div>
                                </div>
                                <div class="timeline-title">Software Engineering Intern</div>
                            </div>
                        </div>
                        <div class="timeline-item">
                            <div class="timeline-content">
                                <div class="timeline-description-container">
                                   <div class="timeline-description">Carleton University</div>
                                </div>
                                <div class="timeline-title">Teaching Assistant</div>
                            </div>
                        </div>
                    </div>
                    <h2 class="links-header-tag">Links</h2>
                    <p class ="links">
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
    margin-top: 4px;
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
    margin-top: 10px;
}
.links{
    max-width: 105px;
    margin-top: -10px;
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

.timeline {
  position: relative;
  max-width: 800px;
  margin: 0 auto;
  padding: 20px 20px;
}
.timeline::after {
  content: '';
  position: absolute;
  width: 2px;
  background-color: #fff;
  top: 0px;
  bottom: 10px;
  left: 5px; 
}
.timeline-item:nth-child(2) {
  margin-top:10px; 
}

.timeline-item {
  position: relative;
  margin-bottom: 0px;
  margin-top: 0px;
}

.timeline-item::after {
  content: '';
  position: absolute;
  width: 8px;
  height: 8px;
  background-color: #fff;
  border-radius: 50%;
  top: 7px;
  left: -18px; 
}

.timeline-content {
  position: relative;
  left: -5px; 
}

.timeline-description {
  margin-bottom: 2px;
  font-size: 16px;
}

.timeline-description-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 0px; 
}

.timeline-title {
  font-size: 14px; 
  color: #8cade6; 
}

.timeline-date {
  font-size: 13px;
  color: #bbb;
  margin-left: auto; 
}

</style>
