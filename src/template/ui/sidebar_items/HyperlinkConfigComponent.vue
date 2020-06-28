<template>
    <div>
        <label>
            <input type="text" name="ref" v-model="control.ref"> Input link
            <input type="checkbox" name="isMultiLine" v-model="control.isMultiLine"> Multi-line?
        </label>
    </div>
</template>

<script>
    export default {
        name: "HyperlinkConfigComponent",
        props: {
            control: {
                type: Object
            },
        },
    }
</script>

<style scoped>

</style>
