<script>
    import {link} from "svelte-spa-router"
</script>

<header>
    <div>logo</div>
    <nav>
        <ul>
            <li><a href="/" use:link>Accueil</a></li>
            <li><a href="/portfolio" use:link>Portfolio</a></li>
            <li><a href="/contact" use:link>Contact</a></li>
        </ul>
    </nav>
</header>



