<template>
  <div>
    <ul>
      <li v-for="item in items" :key="item.id">{{ item.name }}</li>
    </ul>
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
  }
}
</script>