<script>
import {
  VApp,
  VToolbar,
  VToolbarTitle,
  VSpacer,
  VBtn,
  VContent,
} from 'vuetify/lib'

import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'App',
  render() {
    return (
      <VApp>
        <VToolbar app>
          <VToolbarTitle class="headline text-uppercase">
            <span>Vuetify </span>
            <span class="font-weight-light">MATERIAL DESIGN</span>
          </VToolbarTitle>
          <VSpacer />
          <VBtn
            flat
            href="https://github.com/vuetifyjs/vuetify/releases/latest"
            target="_blank"
          >
            <span class="mr-2">Latest Release</span>
          </VBtn>
        </VToolbar>

        <VContent>
          <HelloWorld />
        </VContent>
      </VApp>
    )
  },
}
</script>
