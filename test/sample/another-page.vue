<template>
	<div>
		Current page url: <p v-html="page.url"></p>
		<div v-html="test"></div>
		<myHeader>
		</myHeader>
		<hi></hi>
	</div>
</template>

<script>
export default {
	data: () => {
		return {
			layout: "layout.njk",
			test: "HELLO"
		};
	}
};
</script>