<template>
	<div class="faq">
		<h1>Frequently Asked Questions</h1>

		<uuFaqVue>
			<template #faq0>
				<div question="Question 1?">
					<p>Answer 1.</p>
				</div>
			</template>
			<template #faq1>
				<div question="Question 2?">
					<p>Answer 2.</p>
				</div>
			</template>
		</uuFaqVue>
	</div>
</template>

<script setup>
import uuFaqVue from '@/components/uuFaq.vue';
</script>
