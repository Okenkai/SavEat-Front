<script>
export default {
    data() {
        return {

        }
    },
}
</script>

<template>
    <div class="container">
        <slot></slot>
    </div>
</template>

<style scoped>
    .container{
        max-width: 1200px;
        margin: auto;
    }
</style>