<template>
    <div>
        <div class="row" v-if="labelPosition === 'left'">
            <div class="col-md-4">
                <label :class="{'bold': control.labelBold, 'italic': control.labelItalic, 'underline': control.labelUnderline}">
                    {{control.label}}
                </label>
            </div>
            <div class="col-md-8">
                <a class="form-control"
                          :href="this.control.ref"
                          :readonly="this.control.readonly"
                          :name="control.fieldName">{{control.fieldName}}</a>
            </div>
        </div>
        <div v-else class="form-group">
                <a
                    :href="this.control.ref"
                    :readonly="this.control.readonly"
                    :name="control.fieldName">{{control.label}}
                </a>
        </div>
    </div>
</template>

<script>
    import {Hooks} from 'sethFormBuilder/gui/components/hook_lists';

    export default {
        name: "HyperlinkControl",
        props: ['control', 'labelPosition'],
    }
</script>

<style scoped>

</style>
