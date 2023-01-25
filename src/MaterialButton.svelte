<script >

    import {onMount} from "svelte"

    import {MDCRipple} from '@material/ripple';
    onMount(() => {
        // const buttonRipple =  new MDCRipple(document.querySelector(".mdc-button"));
        const buttonRipple =  new MDCRipple(document.getElementById(id));
    })

    export let id;
    export let text;
</script>

<button {id} class="mdc-button" on:click>
    <span class="mdc-button__ripple"></span>
    <span class="mdc-button__label">{text}</span>
</button>