<template>
    <div class="container">
        <select2-ajax v-model="selected" :list="'/api/mon-hoc/select2'"></select2-ajax>
        {{ selected }}
    </div>
</template>

<script>
    export default {
        mounted() {
            console.log('Component mounted.')
        },
        data() {
            return {
                selected: 4
            };
        }
    }
</script>
