<template>
    <button @click="handler">
        Click me!
    </button>
    <H1 v-show="isShow">
        Hello?!
    </H1>
</template>

<script>
export default {
    data() {
        return {
            isShow: false,
            count: 0
        }
    },
    methods: {
        handler() {
            this.isShow = !this.isShow
            this.count += 1
        }
    }
}
</script>