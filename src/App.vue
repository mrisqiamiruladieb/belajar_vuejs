<template>
  <div>
    <ul>
      <li v-for="item in items" :key="item.id">{{ item.name }}</li>
    </ul>
    <button @click="addItem">Tambah Item</button>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      items: [
        { id: 1, name: 'Buku'},
        { id: 2, name: 'Pensil'},
        { id: 3, name: 'Penghapus'}
        ]
    }
  },
  methods: {
    addItem() {
      const newItem = { id: this.items.length + 1, name: "Barang Baru"};
      this.items.push(newItem);
    }
  }
}
</script>