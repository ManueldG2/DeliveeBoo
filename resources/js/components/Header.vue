<template>
    <header >
        <ul>
            <li>
                <a href="/">
                    <img src="../img/delive.png" alt="" />
                </a>
            </li>
        </ul>
        <ul>
            <li class="nav-dx">


                <router-link
                        :to="{
                            name: 'checkout',


                        }" ><i class="fas fa-shopping-basket"></i>
                        Cart</router-link>
            </li>
            <li class="nav-dx">
                <a href="/admin" target="_blank"><i class="fas fa-home"></i>Log In</a>
            </li>
        </ul>
    </header>
</template>

<script>
export default {
    name: "Header"
};
</script>

<style scoped lang="scss">
header {
    background: white;
    line-height: 3;
    display: flex;
    justify-content: space-between;
    border-bottom: 1px solid #ccc;

    ul {
        list-style: none;
        display: flex;

        li {
            padding-right: 15px;

            img {
                width: 150px;
            }
            a {
                text-decoration: none;
                color: #000;
            }
        }

        .nav-dx {
            border: 1px solid #ccc;
            border-radius: 5px;
            padding: 0 15px;
            margin-right: 10px;

            i {
                margin-right: 10px;
                color: #00a396;
            }
        }
    }
}
</style>
