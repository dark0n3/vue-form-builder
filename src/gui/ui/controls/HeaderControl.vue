<template>
    <div>
        <div class="row" v-if="labelPosition === 'left'">
            <div class="col-md-8">
                <h4 class="modal-title" :value="demo_value">{{control.label}}</h4>
            </div>
        </div>
        <div v-else class="form-group">
                <h4 class="modal-title" :value="demo_value">{{control.label}}</h4>
        </div>
    </div>
</template>

<script>
    import {Hooks} from 'sethFormBuilder/gui/components/hook_lists';

    export default {
        name: "HeaderControl",
        props: ['control', 'labelPosition'],
    }
</script>

<style scoped>

</style>
