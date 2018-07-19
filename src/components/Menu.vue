<template>
  <div id="menu">
    <h1>Accessible Drop Down Menu</h1>
    <nav role="navigation">
        <ul class="access-menu">
            <li v-for="(value, key) in menu" :key="key">
                <a href="#" v-shortkey.focus="[value.shortcut]">{{ key }}</a>
                <ul class="access-submenu">
                  <a v-for="item in value.items" :key="item" href="#"><li> {{item}} </li></a>
                </ul>
            </li>
        </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Menu',
  data () {
    return {
      menu: {
        Womens: {
          shortcut: '1',
          items: [
            'Featured',
            'Shoes',
            'Clothing',
            'Accessories',
            'Sports',
            'Sale'
          ]
        },
        Mens: {
          shortcut: '2',
          items: [
            'Featured',
            'Shoes',
            'Clothing',
            'Accessories',
            'Sports',
            'Sale'
          ]
        },
        Kids: {
          shortcut: '3',
          items: ['Featured', 'Boys', 'Girls', 'Infant', 'Sale']
        },
        Sale: {
          shortcut: '4',
          items: ["Men's Sale", "Women's Sale", 'Plus Sale', "Kids' Sale"]
        }
      }
    }
  }
}
</script>

<!-- Add 'scoped' attribute to limit CSS to this component only -->
<style scoped>
</style>
