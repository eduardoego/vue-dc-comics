<template>
  <div>
      <div class="icons-width">
          <ul>
            <li v-for="(icon,i) in icons" :key="i">
                <div>
                    <img :src="'../assets/' + icon.image" :alt="icons.image">
                </div>

                <div>
                    {{ icon.text }}
                </div>
            </li>
        </ul>
      </div>
  </div>
</template>

<script>
export default {
  name: 'IconsComics',
  data() {
    return {
        icons: [
            {
                image: 'buy-comics-digital-comics.png',
                text: 'Digital Comics'
            },
            {
                image: 'buy-comics-merchandise.png',
                text: 'DC Merchandise'
            },
            {
                image: 'buy-comics-subscriptions.png',
                text: 'Subscription'
            },
            {
                image: 'buy-comics-shop-locator.png',
                text: 'Comic Shop Locator'
            },
            {
                image: 'buy-dc-power-visa.png',
                text: 'DC Power Visa'
            },
        ]
        }
    },
  props: {
    msg: String
  }
}
</script>

<style scoped lang="scss">
* {
    background-color: #0C7CEC;
    display: flex;
    justify-content: center;
    z-index: 1;


    .icons-width {
        width: calc((100% / 12) * 10);
        height: 110px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    ul {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 100%;
        height: 100%;

        li {
            color: white;
            text-transform: uppercase;
            display: flex;
            justify-content: space-around;

            img {
                width: 50%;
            }
        }
    }
}
</style>