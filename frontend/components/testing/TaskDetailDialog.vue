<template>
	<div class="modal">
		<div class="modal-content">
			<h2>Task Detail: {{ task }}</h2>
			<!-- Display task details here -->
			<button @click="close">Close</button>
		</div>
	</div>
</template>

<script>
export default {
	props: {
		task: {
			type: Object,
			required: true
		}
	},
	methods: {
		close() {
			this.$emit('close');
		}
	}
};
</script>

<style scoped>
/* Add your modal styling here */
.modal {
	/* ... */
}
.modal-content {
	/* ... */
}
</style>
