<template>
    <Child :[propName]="propValue"/>
</template>

<script lang="ts">
    import { defineComponent, ref } from '@vue/composition-api';
    import Child from '@/Child.vue';

    export default defineComponent({
        name: 'App',
        components: { Child },
        setup() {
            const propName = 'foo';
            const propValue = 'value';

            return {
                propName,
                propValue,
            };
        },
    });
</script>
