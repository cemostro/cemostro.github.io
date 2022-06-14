<script>
    import { page } from '$app/stores';
    let current = $page.url.pathname;
</script>

<nav>
<ul>
    <li class:selected="{current === '/'}">
        <a href="/">about me</a>
    </li>
    <li class:selected="{current === '/contact'}">
        <a href="/">contact</a>
    </li>
    <li class:selected="{current === '/updates'}">
        <a href="/">updates</a>
    </li>
    <li class:selected="{current === '/blog'}">
        <a href="/">blog</a>
    </li>
</ul>
</nav>


<style>
    nav {
        border-bottom: 1px solid lightgray;
        font-weight: 400;
        padding: 0 1em;
        display: flex;
        margin: 0 auto;
        justify-content: center;
        background-color: #fffefc;
    }

    ul {
        display: flex;
        justify-content: center;
        list-style-type: none;
        margin: 0;
        padding: 0;
    }

    li {
        padding: 0.3rem 0;
        margin: 0 0.5rem;
    }

    a {
        text-decoration: none;
    }

    .selected {
        border-bottom: 2px solid #b8794c;
    }

</style>