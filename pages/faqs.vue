<template>
    <div class="m-24 p-12 bg-gray-300 rounded-xl shadow-xl">
      <h1>Nuxt faqs</h1>
      <ul>
        <li v-for="faq of faqs" :key="faq.id">{{ faq.judul }} <br> {{ faq.isi }}</li>
        
      </ul>
      <h1 class="font-bold text-pink-500">{{ msg }}</h1>
      <h1 class="font-bold text-pink-200">{{ sc }}</h1>
      <button @click="$fetch">Refresh</button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            faqs: null,
            msg: null,
            sc: null
        }
    },
    mounted() {
        this.faqq();
    },
    methods: {
        faqq() {
            const that = this;
            this.$axios.get('public/faq').then(({data}) => {
                this.faqs = data.data
                this.msg = data.message
                this.sc = data.success
            })
            .catch((err) => {
                console.log(err)
            })
        }
    }
}
</script>