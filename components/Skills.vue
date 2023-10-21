<template>
  <div id="skills" class="skills">
    <Headline
      :title="'Skills'"
      :subtitle="'My technical level'"
    />
    <div class="skills-header">
      <div
        v-for="(headerIcon, headerIconId) in headerIcons"
        :key="headerIconId"
        class="block"
        :class="{'radius-top-left' : headerIcon.title === 'HTML 5', 'radius-top-right' : headerIcon.title === 'Node'}"
      >
        <div class="icon">
          <img :src="require(`../assets/images/${headerIcon.img}.svg`)" alt="">
        </div>
        <div class="title text text--14">
          {{ headerIcon.title }}
        </div>
        <div class="subtitle text text--12">
          {{ headerIcon.subtitle }}
        </div>
      </div>
    </div>
    <div class="skills-center">
      <div
        v-for="(centerIcon, centerIconId) in centerIcons"
        :key="centerIconId"
        class="block"
      >
        <div class="icon">
          <img :src="require(`../assets/images/${centerIcon.img}.svg`)" alt="">
        </div>
        <div class="title text text--14">
          {{ centerIcon.title }}
        </div>
        <div class="subtitle text text--12">
          {{ centerIcon.subtitle }}
        </div>
      </div>
    </div>
    <div class="skills-footer">
      <div
        v-for="(footerIcon, footerIconId) in footerIcons"
        :key="footerIconId"
        class="block"
        :class="{'radius-bottom-left' : footerIcon.title === 'NuxtJS', 'radius-bottom-right' : footerIcon.title === 'VSC'}"
      >
        <div class="icon">
          <img :src="require(`../assets/images/${footerIcon.img}.svg`)" alt="">
        </div>
        <div class="title text text--14">
          {{ footerIcon.title }}
        </div>
        <div class="subtitle text text--12">
          {{ footerIcon.subtitle }}
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  data () {
    return {
      headerIcons: [
        {
          img: 'html',
          title: 'HTML 5',
          subtitle: 'markup language for Web pages'
        },
        {
          img: 'css',
          title: 'CSS 3',
          subtitle: 'use to style an HTML document'
        },
        {
          img: 'javaScript',
          title: 'JavaScript',
          subtitle: 'programming language of the Web'
        },
        {
          img: 'node',
          title: 'Node',
          subtitle: 'engine ofJavaScript'
        }
      ],
      centerIcons: [
        {
          img: 'vueIcon',
          title: 'VueJS',
          subtitle: 'framework of JavaScript'
        },
        {
          img: 'typeScript',
          title: 'TypeScript',
          subtitle: 'language that builds on JS'
        },
        {
          img: 'npm',
          title: 'Npm',
          subtitle: 'library and registry for JS'
        },
        {
          img: 'gitIcon',
          title: 'Git',
          subtitle: 'version control system'
        },
        {
          img: 'webPack',
          title: 'Webpack',
          subtitle: 'is a module bundler'
        }
      ],
      footerIcons: [
        {
          img: 'nuxtJS',
          title: 'NuxtJS',
          subtitle: 'framework of Vue'
        },
        {
          img: 'sass',
          title: 'Sass',
          subtitle: 'superpowers of CSS'
        },
        {
          img: 'web3',
          title: 'Web3',
          subtitle: 'world wide web based on Blockchain'
        },
        {
          img: 'vsc',
          title: 'VSC',
          subtitle: 'best of the best code editor'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.skills {
  display: flex;
  flex-direction: column;
}
.skills-header {
  display: grid;
  grid-template-columns: repeat(4, 24%);
  justify-content: space-between;
  margin-top: 40px;
}
.skills-center {
  display: grid;
  grid-template-columns: repeat(5, 19%);
  justify-content: space-between;
  padding-top: 1%;
}
.skills-footer {
  display: grid;
  grid-template-columns: repeat(4, 24%);
  justify-content: space-between;
  padding-top: 1%;
}
.block {
  border: 0.5px solid $gray;
  height: 150px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.icon {
  >img {
      width: 50px;
      height: 60px;
  }
}
.title {
  color: $brand;
}
.subtitle {
  padding-top: 5px;
}
.radius-top-left {
  border-top-left-radius: 20px;
}
.radius-bottom-left {
  border-bottom-left-radius: 20px;
}
.radius-top-right {
  border-top-right-radius: 20px;
}
.radius-bottom-right {
  border-bottom-right-radius: 20px;
}
</style>
