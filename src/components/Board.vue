<template>
  <div>
    <b-table striped hover :items="items" :fields="fields"></b-table>
  </div>
</template>

<script>
  import data from '@/data'
  export default {
    data() {
      return {
        fields: [
          {
            key: 'content_id',
            label: '번호',
            sortable: true
          },
          {
            key: 'title',
            label: '제목',
            sortable: true
          },
          {
            key: 'created_at',
            label: '작성일',
            sortable: true,
          }
        ],
        items: data.Content
      }
    }
  }
</script>