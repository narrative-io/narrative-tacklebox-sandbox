<template>
  <div class="tacklebox-demo">
    <img
      class="logo"
      src="https://www.narrative.io/hs-fs/hubfs/narrative%20logo%20150.png?width=260&name=narrative%20logo%20150.png"
      size="large"
    ></img>
    <h1 class="nio-jumbo-3 text-primary-darker">Tacklebox</h1>
    <p class="nio-p-large text-primary-dark">A library for building apps on the Narrative Data Commerce Platform</p>
    <div class="tiles">
      <div class="tile"> 
        <NioIconFramer
          iconName="display-new"
        ></NioIconFramer>
        <h2 class="nio-h3 text-primary-darker">Consectetur adipiscing elit</h2>
        <p class="nio-p text-primary-dark">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. </p>
      </div>
      <div class="tile"> 
        <NioIconFramer
          iconName="display-new"
        ></NioIconFramer>
        <h2 class="nio-h3 text-primary-darker">Consectetur adipiscing elit</h2>
        <p class="nio-p text-primary-dark">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. </p>
      </div>
      <div class="tile"> 
        <NioIconFramer
          iconName="display-new"
        ></NioIconFramer>
        <h2 class="nio-h3 text-primary-darker">Consectetur adipiscing elit</h2>
        <p class="nio-p text-primary-dark">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. </p>
      </div>
    </div>
    
    <NioButton 
      @click="learnMore"
      jumbo-primary-append
      iconName="utility-arrow-right"
    >View the docs</NioButton>
  </div>
</template>

<script>


export default {
  name: "TackleboxDemo",
  props: {
    msg: String,
  },
  methods: {
    learnMore() {
      window.open('https://docs.narrative.dev/tacklebox/', '_blank')
    }
  },
};
</script>

<style scoped lang="sass">

.tacklebox-demo
  display: flex
  flex-direction: column
  align-items: center
  .logo
    margin-bottom: 96px
    width: 200px
  h1
    margin-bottom: 24px
  p
    text-align: center
  .tiles
    display: flex
    justify-content: space-between
    max-width: 800px
    margin: 96px auto
    @media (max-width: 725px)
      flex-direction: column
      align-items: center
    .tile
      width: 200px  
      display: flex
      flex-direction: column
      align-items: center     
      .nio-icon-framer
        margin-bottom: 24px
      h2, p 
        text-align: center
      h2
        margin-bottom: 16px
    & > .tile + .tile
      @media (min-width: 726px)
        margin-left: 20px
      @media (max-width: 725px)
        margin-top: 64px
</style>
