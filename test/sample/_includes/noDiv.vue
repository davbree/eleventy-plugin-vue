<!--DATA: {{ greeting }} URL method: {{ url("/test/") }}-->
<template>
<div class="parent">
	<child></child>
	<!-- <sibling></sibling> -->
</div>
</template>

<style>
.parent {
	font-weight: 400;
}
</style>

<style scoped>
.parent {
	font-weight: 700;
}
</style>

<script>
import childComponent from "./child.vue";
import siblingComponent from "./sibling.vue";

export default {
	data: function() {
		return {
			greeting: "Hello"
		};
	},
	created: function() {
		console.log( "noDiv is created", this.url, this.page );
	},
	components: {
		child: childComponent,
		sibling: siblingComponent
	}
};
</script>