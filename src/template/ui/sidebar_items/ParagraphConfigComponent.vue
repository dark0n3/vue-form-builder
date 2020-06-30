<template>
    <div>
        <label>
            <textarea type="text" name="ref" v-model="control.paragraph"> Paragraph </textarea>
        </label>
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
