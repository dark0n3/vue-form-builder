<template>
    <div>
        <label>
            <input type="text" name="ref" v-model="control.header"> Header
        </label>
        <div class="form-group font-type">
            <label><input type="checkbox" v-model="control.labelItalic"> Italic</label>
            <label><input type="checkbox" v-model="control.labelUnderline"> Underline</label>
        </div>
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
