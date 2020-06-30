<template>
    <div>
        <label>
            <input type="text" name="ref" v-model="control.header"> Header
        </label>
    </div>
</template>

<script>
    export default {
        name: "HeaderConfigComponent",
        props: {
            control: {
                type: Object
            },
        },
    }
</script>

<style scoped>

</style>
