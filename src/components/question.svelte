<script>
    import Answer from "./answer.svelte";
	import QuestionOption from './question-option.svelte';
    export let number = 1;
    export let answer1 = "";
    export let answer2 = "";
    export let answer3 = "";
    export let answer4 = "";
	
    /** @type { "a" | "b" | "c" | "d" } */
    export let answer = "a";
	/** @type { [string, string] | [string, string, string] | [string, string, string, string] } */
	export let answers = ['', ''];
    /** @type { "a" | "b" | "c" | "d" } */
    let selected = "a";
	/** @type { 0 | 1 | 2 | 3 | null } */
	export let correctIndex = 0;
	/** @type { number } */
	let selected;
</script>

<div>
    <p>{number}. <slot /></p>

    <label for="q{number}a">
        <input
            type="radio"
            name="q{number}"
            id="q{number}a"
            value="a"
            bind:group={selected}
        />
        A: {answer1}
    </label>

    <label for="q{number}b">
        <input
            type="radio"
            name="q{number}"
            id="q{number}b"
            value="b"
            bind:group={selected}
        />
        B: {answer2}
    </label>

    <label for="q{number}c">
        <input
            type="radio"
            name="q{number}"
            id="q{number}c"
            value="c"
            bind:group={selected}
        />
        C: {answer3}
    </label>

    <label for="q{number}d">
        <input
            type="radio"
            name="q{number}"
            id="q{number}d"
            value="d"
            bind:group={selected}
        />
        D: {answer4}
    </label>
	<p style="font-size: 1.5rem; margin-top: 0;">{number}. <b><slot /></b></p>

	<div class="answer-group">
		{#each answers as answer, index}
			<QuestionOption
				letter={['a', 'b', 'c', 'd'][index]}
				text={answer}
				selected={selected == index}
				on:clicked={() => (selected = index)}
			/>
		{/each}
	</div>
</div>

<Answer answer={answer == selected} />
<Answer answer={correctIndex == selected} />

<style>
	.answer-group {
		display: grid;
		gap: 24px;
	}






</style>
<script>
	import Answers from "./answers.svelte"; 
	export let number = 1;

	export let answer1 = '';
	export let answer2 = '';
	export let answer3 = '';
	export let answer4 = '';

	/** @type { "a" | "b" | "c" | "d" } */
	export let answer = "a";
	/** @type { "a" | "b" | "c" | "d" } */
	let selected= "a";
</script>

<div>
	<p>{number} <slot /></p>

	<label for="q{number}a">
		<input type="radio" name="q{number}" id="q{number}a" value="a" 
		bind:group={selected}
		/>
		
		A. {answer1}
	</label>
	<label for="q{number}b">
		<input type="radio" name="q{number}" id="q{number}b" value="b" 
		bind:group={selected}
		/>
		
		B. {answer2}
	</label>
	<label for="q{number}c">
		<input type="radio" name="q{number}" id="q{number}c" value="c" 
		bind:group={selected}
		/>
		
		C. {answer3}
	</label>
	<label for="q{number}d">
		<input type="radio" name="q{number}" id="q{number}d" value="d" 
		bind:group={selected}
		/>
		
		D. {answer4}
	</label>
</div>

<Answers answer={answer == selected} />