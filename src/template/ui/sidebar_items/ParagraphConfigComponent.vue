<template>
    <div>
        <label>
            <textarea type="text" name="ref" v-model="control.paragraph" style="min-height: 20rem"> Paragraph </textarea>
        </label>
        <div class="form-group font-type">
            <label><input type="checkbox" v-model="control.labelBold"> Bold</label>
            <label><input type="checkbox" v-model="control.labelItalic"> Italic</label>
            <label><input type="checkbox" v-model="control.labelUnderline"> Underline</label>
        </div>
    </div>
</template>

<script>
    export default {
        name: "ParagraphConfigComponent",
        props: {
            control: {
                type: Object
            },
        },
    }
</script>

<style scoped>

</style>
