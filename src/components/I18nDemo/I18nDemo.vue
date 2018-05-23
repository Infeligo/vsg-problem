<template>
    <div class="wrapper">
        <Button>{{ $t('greeting') }}</Button>
    </div>
</template>
<script>
//const Vue = require('vue').default;
//const VueI18n = require('vue-i18n').default;
import Vue from 'vue';
import VueI18n from 'vue-i18n';

Vue.use(VueI18n);

const i18n = new VueI18n({
    messages: {
        en: {
            greeting: "Hello!"
        }
    },
    locale: 'en'
});

export default {
    name: 'i18n-demo',
    i18n
};
</script>
