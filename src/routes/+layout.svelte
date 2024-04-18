<script>
    import '$lib/styles/style.scss'
    import Header from "$lib/components/Header.svelte";
</script>

<Header />
<header>Hi, I'm a header</header>

<main>
    <slot />
</main>

<footer>Hello, I'm the footer.</footer>