<script setup>
defineProps({
  content: {
    type: String,
    required: true,
  },
});
</script>
<template>
  <div class="dynamic-content" v-html="content"></div>
</template>
<style lang="scss">
div.dynamic-content {
  font-size: 18px;
  line-height: 1.6rem !important;
  font-weight: 400;
  // a {
  //   color: unset;
  //   text-decoration: none;
  //   background: linear-gradient(
  //       to top,
  //       transparent 0%,
  //       #1976d2 0%,
  //       #1976d2 100%,
  //       transparent 100%
  //     )
  // no-repeat left 0 bottom 0;
  // background-size: auto;
  // background-size: 100% 2px;
  // transition: background-size 250ms ease, color 250ms ease;
  // &:hover {
  //   text-decoration: none;
  //   color: white;
  //   background-size: 100% calc(1em + 6px);
  // }
  // }
  img {
    max-width: 100%;
    height: auto;
    border-radius: 10px;
  }

  figure {
    figcaption {
      margin: 0;
      margin-bottom: 10px;
      padding: 0;
      font-size: 0.8rem;
      line-height: 1.25rem;
      text-align: right;
      justify-content: flex-end;
    }

    a {
      background-color: transparent;
      background-size: 0px;

      &:hover {
        background-size: 0px;
      }
    }
  }

  video {
    width: 100%;
    height: auto;
  }

  p {
    margin-top: 0;
    margin-bottom: 30px;
  }

  ul,
  ol {
    margin-bottom: 1rem;
  }

  blockquote {
    position: relative;
    font-size: 20px;
    margin-bottom: 20px;
    border-right: 10px solid var(--v-primary-base);
    background-color: rgba(50, 50, 50, 0.4);

    // backdrop-filter: blur(20px);
    &::before {
      content: open-quote;
      position: absolute;
      top: 0;
      left: -10px;
      font-family: medium-content-serif-font, Georgia, Cambria,
        "Times New Roman", Times, serif;
      font-size: 50px;
      font-weight: 900;
    }

    // footer.blockquote-footer{}
  }

  pre {
    padding: 10px 10px;
    overflow: auto;
    margin-bottom: 10px;
    background-color: #2d2d2d;
    color: white;
  }

  h1 {
    font-size: 2.5rem !important;
    margin-bottom: 0.5rem;
    font-family: inherit;
    font-weight: 500;
    line-height: 1.2;
    color: inherit;
  }

  h2 {
    font-size: 2rem !important;
    margin-bottom: 0.5rem;
    font-family: inherit;
    font-weight: 500;
    line-height: 1.2;
    color: inherit;
  }

  h3 {
    font-size: 1.75rem !important;
    margin-bottom: 0.5rem;
    font-family: inherit;
    font-weight: 500;
    line-height: 1.2;
    color: inherit;
  }

  h4 {
    font-size: 1.5rem !important;
    margin-bottom: 0.5rem;
    font-family: inherit;
    font-weight: 500;
    line-height: 1.2;
    color: inherit;
  }

  h5 {
    font-size: 1.25rem !important;
    margin-bottom: 0.5rem;
    font-family: inherit;
    font-weight: 500;
    line-height: 1.2;
    color: inherit;
  }

  h6 {
    font-size: 1rem !important;
    margin-bottom: 0.5rem;
    font-family: inherit;
    font-weight: 500;
    line-height: 1.2;
    color: inherit;
  }
}
</style>