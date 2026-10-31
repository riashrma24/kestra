<template>
    <div class="flow-warning-dialog">
        <AlertCircle class="icon" />
        <strong>{{ $t("warning") }}</strong>
    </div>

    <KsMarkdown :content="$t('trigger_check_warning')" />
</template>

<script setup lang="ts">
    import {KsMarkdown} from "@kestra-io/design-system"
    import AlertCircle from "vue-material-design-icons/AlertCircle.vue"
</script>

<style scoped>
.flow-warning-dialog {
    display: flex;
    align-items: center;
    padding: var(--ks-spacing-4) 0;
}

.flow-warning-dialog .icon {
    margin-inline-end: var(--ks-spacing-2);
    font-size: var(--ks-font-size-lg);
    color: var(--ks-status-warning);
}
</style>