<script>
	let count=0;
	function countup() {
		count +=1;
	}
	function countdown(){
		count -=1;
	}
</script>

{#if count == 1}
	<h1>
		I have {count} dollar.
	</h1>
{/if}
{#if count != 1}
	<h1>
		I have {count} dollars.
	</h1>
{/if}

<div>
	<button on:click={countup}>
		+1
	</button>
	<button on:click={countdown}>
		-1
	</button>
</div>