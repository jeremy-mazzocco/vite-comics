<script>
export default {
  name: "AppHeader",
  methods: {
    getImageURL: function (imgPath) {
      return new URL(imgPath, import.meta.url).href;
    },
  },
  data() {
    return {
      links: [
        {
          text: "CHARACTERS",
          url: "#",
          current: false,
        },
        {
          text: "COMICS",
          url: "#",
          current: true,
        },
        {
          text: "MOVIES",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "GAMES",
          url: "#",
          current: false,
        },
        {
          text: "COLLECTIBLES",
          url: "#",
          current: false,
        },
        {
          text: "VIDEO",
          url: "#",
          current: false,
        },
        {
          text: "FANS",
          url: "#",
          current: false,
        },
        {
          text: "NEWS",
          url: "#",
          current: false,
        },
        {
          text: "SHOP",
          url: "#",
          current: false,
        }
      ]
    }
  }
}

</script>


<template>
  <div class="container">
    <nav>
      <a href="#">
        <img :src="getImageURL(`../assets/img/dc-logo.png`)" alt="#" />
      </a>
      <ul>
        <li v-for="link in links">
          <a :class="link.current ? 'active' : ''" :href="link.url">{{ link.text }}</a>
        </li>
      </ul>
    </nav>
  </div>
</template>


<style lang="scss" scoped>
@use '../styles/partiarls/mixins.scss' as *;
@use '../styles/partiarls/colors.scss' as *;

nav {
  @include my-dislay-flex;
  height: 80px;

  img {
    width: 60px;
    height: 60px;
  }

  ul {
    @include my-dislay-flex;
    font-size: 12px;
    font-weight: bold;

    li {
      padding: 0 10px;
      height: 80px;
      line-height: 80px;

      &:hover {
        border-bottom: 2px solid $dcBlue;
      }

      a {
        color: rgb(86, 85, 85);
        text-decoration: none;

        &.active,
        &:hover {
          color: $dcBlue;
        }
      }
    }
  }
}
</style>
