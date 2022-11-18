<template>
	<div>
		<!-- {{ threads }} -->
		<h1>Hello World</h1>
		{{ threads[0].id }}
	</div>
</template>

<script>
import sourceData from "@/data.json";
export default {
	name: "HelloWorld",
	props: {
		msg: String
	},
	data() {
		return {
			threads: sourceData.threads
		};
	}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
	margin: 40px 0 0;
}
ul {
	list-style-type: none;
	padding: 0;
}
li {
	display: inline-block;
	margin: 0 10px;
}
a {
	color: #42b983;
}
</style>
