<script>
	export let inputId;
	export let inputType;
	export let inputValue;
	export let inputDisabled;
	export let inputPlaceholder;
	export let inputIcon = false;

	function getInputValue(event) {
		inputValue = event.target.value;
	}
</script>

<input
	id={inputId}
	class="input"
	type={inputType}
	spellcheck="false"
	autocomplete="off"
	disabled={inputDisabled}
	on:input={getInputValue}
	class:icon-space={inputIcon}
	placeholder={inputPlaceholder}
/>

<style>
	.input {
		width: 100%;
		padding: 9px 12px;
		font-size: var(--text-16);
		transition: box-shadow 100ms;
		border: 1px solid var(--primary-900);
	}

	.input:disabled {
		background-color: var(--grey-100);
		border: 1px solid var(--primary-300);
	}

	.input:focus {
		outline-offset: -1px;
		outline: 2px solid var(--primary-900);
	}

	.input::placeholder {
		font-size: 15px;
		color: var(--grey-500);
	}

	.icon-space {
		padding-right: var(--space-48x);
	}
</style>
