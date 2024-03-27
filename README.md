# Main
All My Main Scripts
# yarn
yarn add @meforma/vue-copy-to-clipboard

# npm
npm install @meforma/vue-copy-to-clipboard
// In you main.js
// ... considering that your app creation is here
import copyText from "@meforma/vue-copy-to-clipboard";

createApp(App).use(copyText).mount("#app");
