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

<Question
	number={2}
	answer1="15"
	answer2="17"
	answer3="16"
	answer4="old"
    answer="a"
>
	how old am I?
</Question>

<Question
	number={3}
	answer1="red"
	answer2="blue"
	answer3="pink"
	answer4="orange"
    answer="a"
>
	what is my favorite color?
</Question>

<Question
	number={4}
	answer1="red"
	answer2="blue"
	answer3="pink"
	answer4="orange"
    answer="a"
>
	what is my favorite color?
</Question>
