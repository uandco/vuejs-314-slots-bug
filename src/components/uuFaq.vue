<template>
	<div>
		<ol>
			<li v-for="(item, key) in slots" :key="key + '-olterm'">
				<a :href="'#uu-faq-' + key">{{ item()[0].props.question }}</a>
			</li>
		</ol>

		<hr>

		<div v-for="(item, key) in slots" :key="key + '-term'">
			<h3 :id="'uu-faq-' + key">{{ item()[0].props.question }}</h3>
			<div>
				<slot :name="key"></slot>
			</div>
		</div>
	</div>
</template>

<script setup>
import { useSlots } from 'vue';

const slots = useSlots();
</script>
