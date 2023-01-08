<template>
  <div class="row">
    <div class="col-12">
      <PageTitle page_title="Starters"/>
        <div>
          <pre>
            {{ menu }}
          </pre>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  layout: 'homepage',
  name: 'starters',
  data() {
    return {
      menu: [],
    }
  },
  created() {
    this.getMenu();
  },
  methods: {
    async getMenu() {
      try {
        const results = await fetch('http://localhost:1337/api/menu-combos').then(res => res.json());
        this.menu = results;
      } catch(error) {
        console.error('something went wrong ', error);
      }
    }
  }
}
</script>
