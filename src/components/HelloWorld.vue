<script>
import { VContainer, VLayout, VFlex, VImg } from 'vuetify/lib'

import logo from '@/assets/logo.svg'

export default {
  data: () => ({
    ecosystem: [
      {
        text: 'vuetify-loader',
        href: 'https://github.com/vuetifyjs/vuetify-loader',
      },
      {
        text: 'github',
        href: 'https://github.com/vuetifyjs/vuetify',
      },
      {
        text: 'awesome-vuetify',
        href: 'https://github.com/vuetifyjs/awesome-vuetify',
      },
    ],
    importantLinks: [
      {
        text: 'Documentation',
        href: 'https://vuetifyjs.com',
      },
      {
        text: 'Chat',
        href: 'https://community.vuetifyjs.com',
      },
      {
        text: 'Made with Vuetify',
        href: 'https://madewithvuetifyjs.com',
      },
      {
        text: 'Twitter',
        href: 'https://twitter.com/vuetifyjs',
      },
      {
        text: 'Articles',
        href: 'https://medium.com/vuetify',
      },
    ],
    whatsNext: [
      {
        text: 'Explore components',
        href: 'https://vuetifyjs.com/components/api-explorer',
      },
      {
        text: 'Select a layout',
        href: 'https://vuetifyjs.com/layout/pre-defined',
      },
      {
        text: 'Frequently Asked Questions',
        href:
          'https://vuetifyjs.com/getting-started/frequently-asked-questions',
      },
    ],
  }),
  render() {
    return (
      <VContainer>
        <VLayout text-xs-center wrap>
          <VFlex xs12>
            <VImg src={logo} class="my-3" contain height="200" />
          </VFlex>

          <VFlex mb-4>
            <h1 class="display-2 font-weight-bold mb-3">Welcome to Vuetify</h1>
            <p class="subheading font-weight-regular">
              For help and collaboration with other Vuetify developers,
              <br />
              please join our online{' '}
              <a
                href="https://community.vuetifyjs.com"
                target="_blank"
                rel="noopener noreferrer"
              >
                Discord Community
              </a>
            </p>
          </VFlex>

          <VFlex mb-5 xs12>
            <h2 class="headline font-weight-bold mb-3">What's next?</h2>
            <VLayout justify-center>
              {this.whatsNext.map((next, i) => (
                <a
                  key={i}
                  href={next.href}
                  class="subheading mx-3"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  {next.text}
                </a>
              ))}
            </VLayout>
          </VFlex>

          <VFlex mb-5 xs12>
            <h2 class="headline font-weight-bold mb-3">Important Links</h2>
            <VLayout justify-center>
              {this.importantLinks.map((links, i) => (
                <a
                  key={i}
                  href={links.href}
                  class="subheading mx-3"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  {links.text}
                </a>
              ))}
            </VLayout>
          </VFlex>

          <VFlex mb-5 xs12>
            <h2 class="headline font-weight-bold mb-3">Ecosystem</h2>
            <VLayout justify-center>
              {this.ecosystem.map((eco, i) => (
                <a
                  key={i}
                  href={eco.href}
                  class="subheading mx-3"
                  target="_blank"
                  rel="noopener noreferrer"
                >
                  {eco.text}
                </a>
              ))}
            </VLayout>
          </VFlex>
        </VLayout>
      </VContainer>
    )
  },
}
</script>

<style></style>
