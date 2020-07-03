<template>
    <div class="controlItemWrapper" :class="control.className" :data-control-name="control.name">
        <div class="controlItem row" :id="control.name" v-if="labelPosition === 'left'">
            <div class="col-md-8 input-group">
                <h4 class="modal-title" :value="demo_value">{{control.header}}</h4>
            </div>
        </div>
        <div class="controlItem row" :id="control.name" v-else>
            <div class="form-group col-md-12">
                <div class="input-group">
                    <h4 class="modal-title" :value="demo_value">{{control.header}}</h4>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Header",
        props: ['control', 'labelPosition'],
        computed: {
            demo_value() {
                if (!_.isEmpty(this.control.defaultValue)) {
                    return this.control.defaultValue;
                }

                return "";
            }
        }
    }
</script>

<style scoped>

</style>
