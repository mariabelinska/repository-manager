<template>
  <v-container>
    <h1 class="mx-3">Bookmarks</h1>
    <RepositoryCard v-for="bookmark in bookmarks" :key="bookmark.id" :repository="bookmark" />
  </v-container>
</template>

<script>
import RepositoryCard from '@/components/RepositoryCard.vue';
import { mapState } from 'vuex';

export default {
  components: {
    RepositoryCard,
  },
  computed: mapState({
    bookmarks: state => state.bookmark.bookmarks,
  }),
};
</script>
