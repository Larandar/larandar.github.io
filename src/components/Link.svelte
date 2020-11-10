<script>
    import Icon from "./Icon.svelte";

    export let href;
    export let icon = "fas fa-link";
</script>

<style>
    a,
    a:visited {
        display: block;
        color: hsl(345, 67%, 55%);
        background: hsla(165, 57%, 78%, 25%);
        border-radius: 1rem;
        padding: 0.5rem 0;
        margin: 0.5rem;
        text-decoration: none;
    }

    a:hover {
        background: hsla(165, 57%, 78%, 65%);
    }

    .icon {
        font-size: 1.5rem;
        line-height: 1rem;
        margin-left: 0.2rem;
    }
</style>

<a {href}>
    <span class="icon"><Icon {icon} /></span>

    <slot /></a>
