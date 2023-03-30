<script>
	import Question from '../components/question.svelte';
	import Score from '../components/score.svelte';
</script>

<Score score={0} />

<Question
	number={1}
	answer1="first answer"
	answer2="second answer"
	answer3="third answer"
	answer4="fourth answer"
    answer="a"
>
	This is my Question?
</Question>
