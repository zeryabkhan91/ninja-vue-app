<template>
  <div class="home">
    <List :list_items="menu_items" />
	</div>
</template>

<script>
import List from './List.vue';

export default {
  components: {
    List
  },
  data() {
    return {
      menu_items: [
        {
          title: "Ninja Gaming",
          link: "http://youtube.com/ninja?sub_confirmation=1",
          icon: ''
        },
        {
          title: "Ninja Vods",
          link: "https://www.youtube.com/channel/UCQU9XxfLNdix04S3hWRw8-Q",
          icon: ''
        },
        {
          title: "Ninja Shorts",
          link: "https://www.youtube.com/channel/UCmyweyoqldy5yPGeHigEyzA",
          icon: ''
        }
      ]
    }
  }
}
</script>
