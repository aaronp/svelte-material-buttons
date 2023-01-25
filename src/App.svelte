<script>
	import MaterialButton from "./MaterialButton.svelte";

	const click = (event) => {
		//https://developer.mozilla.org/en-US/docs/Web/API/MouseEvent
		const src = event.target || event.srcElement

		alert(src.innerText);
	}
</script>

<MaterialButton id="one" text="first" on:click={click}/>
<MaterialButton id="two" text="second" on:click={click}/>

<style global lang="scss">
@use "@material/button/styles";
</style>