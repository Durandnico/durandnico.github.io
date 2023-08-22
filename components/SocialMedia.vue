<template>
    <div class="watermark">
        <a href="https://github.com/Durandnico"><Icon name="grommet-icons:github" class="link" size="32px"></Icon></a>
        <a href="https://fr.linkedin.com/in/nicolas-durand-7b8288263"><Icon name="grommet-icons:linkedin" class="link" size="32px"></Icon></a>
    </div>
</template>

<script setup lang="ts">

</script>

<style scoped>

.watermark {
    z-index: 99;
    display: flex;
    flex-direction: row;
    gap: 12px;
}

a, a:visited {
    color:#f4dbd6;
}

</style>