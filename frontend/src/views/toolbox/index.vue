<template>
    <div>
        <RouterButton :buttons="buttons" />
        <LayoutContent>
            <router-view></router-view>
        </LayoutContent>
    </div>
</template>

<script lang="ts" setup>
import i18n from '@/lang';

const buttons = [
    {
        label: i18n.global.t('toolbox.device.toolbox'),
        path: '/toolbox/device',
    },
    {
        label: i18n.global.t('menu.supervisor'),
        path: '/toolbox/supervisor',
    },
    {
        label: 'Fail2Ban',
        path: '/toolbox/fail2ban',
    },
];
</script>
