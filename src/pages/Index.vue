<template>
  <Layout :sidebar="false">
    <div class="content">
      <div class="title-block">
        <h1 class>
          Do it yourself
          <span class="primary">CS</span>
        </h1>
        <h1 class="tagline">
          A structured path for learning
          <span class="primary">computer science</span> in a way that suits you
        </h1>
      </div>

      <nav>
        <!-- To use other icons here, you need to import them in the Shortcut component -->
        <Shortcut link="/getting-started" text="Introduction" icon="play-icon"/>
        <Shortcut link="/theme-configuration" text="Configuration" icon="sliders-icon"/>
        <Shortcut link="/theme-configuration#changing-colors" text="Change colors" icon="eye-icon"/>
      </nav>
    </div>
  </Layout>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
import Shortcut from "~/components/Shortcut.vue";

export default {
  components: {
    Shortcut
  },
  data() {
    return {
      description:
        "A structured path for learning computer science in a way that suits you"
    };
  },
  metaInfo() {
    return {
      title: this.description,
      meta: [
        {
          key: "description",
          name: "description",
          content:
            "A theme for static site documentation based on Gridsome, ready to deploy to Netlify in one click."
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.content {
  display: flex;
  flex-direction: column;
}

div.title-block {
  text-align: center;
  max-width: 600px;
  margin: 1.5em auto 1.5em;

  .primary {
    color: $brandPrimary;
  }

  .tagline {
    font-size: 1.8em;
  }

  @include respond-above(md) {
    max-width: 1000px;
  }
}

h2 {
  font-size: 1.4rem;
  margin: 0;
}

nav {
  display: flex;
  justify-content: space-between;
  flex-direction: column;

  @include respond-above(sm) {
    flex-direction: row;
  }
}

.git {
  margin: 3em 0 0;
  align-self: center;

  @include respond-above(md) {
    margin: 5em 0 0;
  }
}
</style>
