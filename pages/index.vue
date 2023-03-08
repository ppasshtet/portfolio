<template>
  <div class="index">
    <Header />
    <Welcome />
    <ScrollDown />
    <Headline>
      <template #title>
        About me
      </template>
      <template #subtitle>
        My introducatio
      </template>
    </Headline>
    <About />
    <Headline>
      <template #title>
        Skills
      </template>
      <template #subtitle>
        My technical level
      </template>
    </Headline>
    <Knowledge />
    <Headline>
      <template #title>
        My way
      </template>
      <template #subtitle>
        My professional way in other project
      </template>
    </Headline>
    <Way />
    <Headline>
      <template #title>
        Portfolio
      </template>
      <template #subtitle>
        My portfolio works in other project
      </template>
    </Headline>
    <CarouselSlider />
    <Headline>
      <template #title>
        Resume
      </template>
      <template #subtitle>
        My resume on Linkedin and HeadHanter
      </template>
    </Headline>
    <Resume />
    <Headline>
      <template #title>
        Contact me
      </template>
      <template #subtitle>
        Get in touch
      </template>
    </Headline>
    <Contact />
    <Footer />
  </div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>

<style lang="scss">
  .index {
    padding: 20px 150px;
    background: $background;
  }
</style>
