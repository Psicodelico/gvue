<template>
    <div class="about">
        <h1>This is an {{about}} page</h1>
        <span v-bind:title="message">鼠标悬停</span>
        <ol>
            <li v-for="todo in todos" :key="todo.text">
                {{ todo.text }}
            </li>
        </ol>
    </div>
</template>

<script>
export default {
    data: () => ({
        message: "页面加载于 " + new Date().toLocaleString(),
        about: "about1",
        todos: [{ text: "js" }, { text: "ng" }, { text: "vue" }]
    })
};
</script>
