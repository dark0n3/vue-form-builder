<template>
    <div class="controlItemWrapper" :class="control.className" :data-control-name="control.name">
        <div class="controlItem row" :id="control.name" v-if="labelPosition === 'left'">
            <div class="col-md-8 input-group">
                <p
                    :value="demo_value"
                    :class="{'bold': control.labelBold, 'italic': control.labelItalic, 'underline': control.labelUnderline}"
                    >
                        {{control.paragraph}}
                    </p>
            </div>
        </div>
        <div class="controlItem row" :id="control.name" v-else>
            <div class="form-group col-md-12">
                <div class="input-group">
                    <p :value="demo_value"
                    :class="{'bold': control.labelBold, 'italic': control.labelItalic, 'underline': control.labelUnderline}"
                    >
                        {{control.paragraph}}
                    </p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Pragraph",
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
