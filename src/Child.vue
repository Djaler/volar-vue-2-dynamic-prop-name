<template>
    {{ foo }}/{{ bar }}
</template>

<script lang="ts">
    import { defineComponent } from '@vue/composition-api';

    export default defineComponent({
        name: 'Child',
        props: {
            foo: {
                type: String,
                default: null,
            },
            bar: {
                type: String,
                default: null,
            },
        },
    });
</script>
