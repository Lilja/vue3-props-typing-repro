<template>
  <div class="hello"> {{props}} </div>
</template>

<script lang="ts">
import { defineComponent, PropType } from 'vue';

const ComponentProps = {
    msg: {
        type: String as PropType<string>,
        required: true
    }
}
export default defineComponent({
  props: ComponentProps,
  setup(props) {
    const msg: string = props.msg
  }
});
</script>
