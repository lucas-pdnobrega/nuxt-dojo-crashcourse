<template>
    <div>
        <h2>About</h2>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestias aperiam animi, corporis fugiat nobis aspernatur porro excepturi totam deleniti omnis illum ab saepe labore odit minima natus veritatis laboriosam? Fugiat?</p>
    </div>
    <div>
        {{ data }}
    </div>
</template>

<script setup>
    const { data } = await useFetch('/api/ninja?name=mario', {
        method: 'post',
        body: { age: 30}
    });
</script>

<style scoped>
    h2 {
        margin-bottom: 20px;
        font-size: 36px;
    }
    p {
        margin: 20px 0;
    }
</style>