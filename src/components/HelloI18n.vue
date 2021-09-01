<template>
  <div>
  <div class="locale-changer">
    <select v-model="$i18n.locale">
      <option v-for="(lang, i) in langs" :key="`Lang${i}`" :value="lang">{{ lang }}</option>
    </select>
  </div>

  <p>{{ $t('message') }}</p>
    </div>
</template>

<script>
export default {
  name: 'HelloI18n',
  data () {
    return { langs: ['en', 'uk'] }
  }
}
</script>

