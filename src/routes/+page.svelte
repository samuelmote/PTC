<script>
	import Score from "../components/score.svelte";
	import Question from "../components/question.svelte";
	
</script>

<Score score={0} />

<Question
	number={1}
	answer1="First answer"
	answer2="Second answer"
	answer3="Third answer"
	answer4="Fourth answer"
	answer="c"
>
<Question number={1} answers={['Yes', 'No', 'Maybe, but not right now']} correctIndex={0}>
	This is my new question?
</Question>
</Question>


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
>what is my favorite color?
	<style> 
	.Question{
	color: #ffffff;
		font-weight: bold;
		text-decoration: underline;
	}
	</style>
</Question>


