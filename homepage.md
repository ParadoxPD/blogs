# Blogs

---

<style>
    body {
    --headings: #74c0fc;
    --links: #91A7FF;
    --highlight: #41C7C7;
    --bg: #1f242A;
    --bg-secondary: #323945;
    --text: #adb5bd;
    --text-secondary: #9CA3AF;
    --code-text: #91A7FF;
    --share-text: #C4C4C4
}

ul.horizontal-list {
    display: flex;
    margin-top: 0em;
    margin-left: -40px;
    flex-wrap: wrap
}
ul.horizontal-list li {
    display: inline;
    margin-right: 1em
}
ul.horizontal-list li a {
    text-decoration: none;
    font-weight: normal
}
.card {
    padding: 1em;
    border: 1px var(--text) solid;
    width: 15em;
    height: auto;
    text-align: center;
    font-size: 1em;
    align-items: center;
    background-color: var(--bg-secondary);
    margin-bottom: 0.8em;
    border-radius: 0.5em
}
.card .header {
    color: var(--links)
}
.card .body {
    font-size: 0.8em
}
.card hr {
    margin: 0.5em 0
}

@media screen and (max-width: 600px) {
    ul.horizontal-list li.card {
        width:100%;
        display: block;
        margin-bottom: 1em;
        margin-left: 1em
    }

    ul.horizontal-list li.card a,ul.horizontal-list li.card .header {
        font-size: 1em
    }
}

</style>
<div>
<ul class="horizontal-list">
    <li class="card">
      <a href="overview-post">
        <span class="header">
          Project 1
        </span>
        <hr>
        <p class="body">
          This is an example project, configured in _data/home.yml
        </p>
      </a>
    </li>
    <li class="card">
      <a href="overview-post">
        <span class="header">
          Project 2 
        </span>
        <hr> 
        <p class="body">
          Projects are shown in card layout
        </p>
      </a>
    </li>
    <li class="card">
      <a href="overview-post">
        <span class="header">
          Project 3   
        </span>
        <hr>
        <p class="body">
          You can control visibility from _config.yml file
        </p>
      </a>
    </li>
</ul>
</div>