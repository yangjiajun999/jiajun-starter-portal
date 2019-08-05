<template>
    <div>
        <a-breadcrumb style="margin: 16px 0">
            <a-breadcrumb-item>User</a-breadcrumb-item>
            <a-breadcrumb-item>Bill</a-breadcrumb-item>
        </a-breadcrumb>
        <div :style="{ padding: '24px', background: '#fff', minHeight: '360px' }">
            Bill is a cat.
        </div>
    </div>
</template>

<script>
export default {
    name: 'home',
    layout: 'admin'
};
</script>

<style scoped>

</style>
