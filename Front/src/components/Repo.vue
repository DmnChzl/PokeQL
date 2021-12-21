<template>
  <div>
    <h4>Sources</h4>
    <Item
      title="GitHub"
      subTitle="DmnChzl/PokeQL"
      :handleClick="goToRepository"
      faIcon="archive"
      leftColor="#424242"
      rightColor="#424242">
      <div class="clearfix">
        <i class="fa fa-angle-right" />
      </div>
    </Item>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Item from './Item.vue';

const GITHUB = 'https://github.com/dmnchzl/pokeql';

@Component({
  components: {
    Item,
  },
})
export default class Repo extends Vue {
  private goToRepository() {
    window.location.href = GITHUB;
  }
}
</script>
