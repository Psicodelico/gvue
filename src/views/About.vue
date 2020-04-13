<template>
    <div class="about">
        <h1>This is an {{about}} page</h1>
        <span v-bind:title="message">鼠标悬停</span>
    </div>
</template>

<script>
export default {
    data: () => ({
        message: "页面加载于 " + new Date().toLocaleString(),
        about: "about1"
    })
};
</script>
