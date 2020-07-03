<template>
    <div class="row mt-2">
        <div class="col-md-12">
            <label>
                <input type="checkbox" name="isRequired" v-model="control.required"> Required?
            </label>
            <label>
                <input type="checkbox" name="isReadonly" v-model="control.readonly"> Readonly?
            </label>
        </div>
    </div>
</template>

<script>
export default {
    name: "BaseConfigInputGroup"
}
</script>

<style scoped>

</style>
