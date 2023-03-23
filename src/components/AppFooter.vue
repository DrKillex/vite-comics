<script>
import AppFooterDisplay from './AppFooterDisplayer.vue';
import AppFooterNav from './AppFooterNav.vue';
import AppFooterContacts from './AppFooterContacts.vue';

export default {
    name: "AppFooter",
    components: {
        AppFooterDisplay,
        AppFooterNav,
        AppFooterContacts
    }
    }
</script>

<template>
    <footer>
        <AppFooterDisplay></AppFooterDisplay>
        <AppFooterNav></AppFooterNav>
        <AppFooterContacts></AppFooterContacts>
    </footer>
    
</template>