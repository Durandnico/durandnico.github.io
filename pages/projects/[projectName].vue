<template>
    <div>
        <p>project details for {{ projectName }}</p>
    </div>
</template>

<script setup lang="ts">
    const { projectName } = useRoute().params
</script>

<style scoped>

</style>