Basic button:

You can also use the Single File Component Format

```vue
<template>
    <div class="wrapper">
        <Button>{{ $t('greeting') }}</Button>
    </div>
</template>
<script>
const Vue = require('vue');
const VueI18n = require('vue-i18n');

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
    name: 'vue-i18n-demo',
    i18n
};
</script>
```
