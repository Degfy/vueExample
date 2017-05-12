<template>
  <!-- 代码规范 参考 http://codeguide.bootcss.com/#html -->
  <div class="example-class">
    this is a example.
    <!-- has slot -->
    <ComponentX>
      <div>slot content</div>
    </ComponentX>
    <!-- no slot -->
    <ComponentX/>
  </div>
</template>
<script>
// 代码规范 参考 https://github.com/feross/standard/blob/master/docs/RULES-zhcn.md
import BaseExample from './base-example'
import mixin from './mixin'

import DirectiveX from './directive-x'
import FilterX from './filter-x'
import ComponentX from './component-x'

export default {
  name: 'example',
  extends: BaseExample,
  mixins: [mixin],

  directives: {
    DirectiveX,
  },
  filters: {
    FilterX,
  },
  components: {
    ComponentX,
  },

  props: {},
  computed: {},
  methods: {},
  watch: {},

  beforeCreate() {

  },
  created() {

  },

  data() {},

  beforeMount() {

  },
  mounted() {

  },

}
</script>
<style lang="scss">
// 代码规范 参考 http://codeguide.bootcss.com/#css
.example-class {
  position: absolute;
  top: 0;
  left: 0;
  margin: 10px 20px;
  border: 1px solid #cccccc;
  padding: 20px;
}
</style>
