<script>
export default {
    name: 'cards',
    props: {
        title: String,
        url: String,
    }
}
</script>
<template>
    <div class="card">
        <img :src="url" :alt="title">
        <h4>{{ title }}</h4>
    </div>
</template>
<script lang="scss" scoped>
</script>
