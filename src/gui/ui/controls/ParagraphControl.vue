<template>
    <div>
        <div class="row" v-if="labelPosition === 'left'">
            <div class="col-md-8">
                <p
                    :value="demo_value"
                    :class="{'bold': control.labelBold, 'italic': control.labelItalic, 'underline': control.labelUnderline}"
                >
                    {{control.paragraph}}
                </p>
            </div>
        </div>
        <div v-else class="form-group">
            <p class="modal-title"
                :value="demo_value"
                :class="{'bold': control.labelBold, 'italic': control.labelItalic, 'underline': control.labelUnderline}"
            >
                {{control.paragraph}}
            </p>
        </div>
    </div>
</template>

<script>
    import {Hooks} from 'sethFormBuilder/gui/components/hook_lists';

    export default {
        name: "ParagraphControl",
        props: ['control', 'labelPosition'],
    }
</script>

<style scoped>

</style>
