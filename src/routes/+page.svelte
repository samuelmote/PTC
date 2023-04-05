<script>
	import Question from '../components/question.svelte';
	import Score from '../components/score.svelte';
</script>

<Score score={0} />

<Question
	number={1}
	answer1="red"
	answer2="blue"
	answer3="pink"
	answer4="orange"
    answer="a"
>
	what is my favorite color?
</Question>
