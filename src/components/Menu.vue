<template>
  <div id="menu">
    <h1>Accessible Drop Down Menu</h1>
    <nav role="navigation">
        <ul class="access-menu">
            <li>
                <a href="#" v-shortkey.focus="[1]">Womens</a>
                <ul class="access-submenu">
                    <li><a href="#">Featured</a></li>
                    <li><a href="#">Shoes</a></li>
                    <li><a href="#">Clothing</a></li>
                    <li><a href="#">Accessories</a></li>
                    <li><a href="#">Sports</a></li>
                    <li><a href="#">Sale</a></li>
                </ul>
            </li>
            <li>
                <a href="#" v-shortkey.focus="[2]">Mens</a>
                <ul class="access-submenu">
                    <li><a href="#">Featured</a></li>
                    <li><a href="#">Shoes</a></li>
                    <li><a href="#">Clothing</a></li>
                    <li><a href="#">Accessories</a></li>
                    <li><a href="#">Sports</a></li>
                    <li><a href="#">Sale</a></li>
                </ul>
            </li>
            <li>
                <a href="#" v-shortkey.focus="[3]">Kids</a>
                <ul class="access-submenu">
                    <li><a href="#">Featured</a></li>
                    <li><a href="#">Boys</a></li>
                    <li><a href="#">Girls</a></li>
                    <li><a href="#">Infant</a></li>
                    <li><a href="#">Sale</a></li>
                </ul>
            </li>
            <li>
                <a href="#" v-shortkey.focus="[4]">Sale</a>
                <ul class="access-submenu">
                    <li><a href="#">Men's Sale</a></li>
                    <li><a href="#">Women's Sale</a></li>
                    <li><a href="#">Plus Sale</a></li>
                    <li><a href="#">Kids' Sale</a></li>
                </ul>
            </li>
        </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Menu'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
