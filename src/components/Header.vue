<template>
    <nav class="navbar">
        <div class="container-special wrapper-nav">
            <div class="left-nav">
                <router-link to="/" class="icon-left-1"><svg width="44" height="38" viewBox="0 0 44 38" fill="none"
                        xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                        <rect width="44" height="38" fill="url(#pattern0)" />
                        <defs>
                            <pattern id="pattern0" patternContentUnits="objectBoundingBox" width="1" height="1">
                                <use xlink:href="#image0" transform="scale(0.0227273 0.0263158)" />
                            </pattern>
                            <image id="image0" width="44" height="38"
                                xlink:href="data:image/png;base64,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" />
                        </defs>
                    </svg></router-link>
                <router-link to='/catalog' class="icon-left-2"><svg width="27" height="28" viewBox="0 0 27 28" fill="none"
                        xmlns="http://www.w3.org/2000/svg">
                        <path
                            d="M19.0596 17.6259C20.6713 15.8658 21.6282 13.6048 21.7698 11.2225C21.9113 8.84018 21.2288 6.48173 19.8369 4.54318C18.445 2.60463 16.4285 1.20404 14.126 0.576619C11.8234 -0.0508009 9.3751 0.13316 7.19217 1.09761C5.00923 2.06205 3.22463 3.74825 2.13804 5.87302C1.05145 7.9978 0.729054 10.4318 1.225 12.7661C1.72094 15.1005 3.00501 17.1932 4.86158 18.6927C6.71814 20.1922 9.03413 21.0072 11.4206 21.0009C13.673 21.004 15.8645 20.27 17.6606 18.9109L25.4086 26.7179C25.4941 26.807 25.5965 26.8781 25.7099 26.927C25.8232 26.9759 25.9452 27.0017 26.0686 27.0029C26.1923 27.0033 26.3148 26.9782 26.4283 26.9292C26.5419 26.8801 26.6441 26.8082 26.7286 26.7179C26.9025 26.537 26.9997 26.2958 26.9997 26.0449C26.9997 25.794 26.9025 25.5528 26.7286 25.3719L19.0596 17.6259ZM2.88662 10.5009C2.89946 8.81563 3.41094 7.17187 4.35659 5.77685C5.30224 4.38183 6.63972 3.29801 8.20044 2.662C9.76115 2.02599 11.4752 1.86627 13.1266 2.20298C14.7779 2.53969 16.2926 3.35775 17.4797 4.55404C18.6668 5.75033 19.4732 7.27129 19.7972 8.92519C20.1212 10.5791 19.9483 12.2919 19.3002 13.8476C18.6522 15.4034 17.5581 16.7325 16.1559 17.6674C14.7536 18.6023 13.1059 19.1011 11.4206 19.1009C9.14916 19.0901 6.97482 18.1784 5.37484 16.566C3.77486 14.9537 2.87998 12.7724 2.88662 10.5009Z"
                            fill="#E8E8E8" />
                    </svg></router-link>
                    <input v-model="query" placeholder="временный поиск">
            </div>
            <div class="right-nav">
                <button class="icon-right"><svg width="32" height="23" viewBox="0 0 32 23" fill="none"
                        xmlns="http://www.w3.org/2000/svg">
                        <path d="M0 23V20.31H32V23H0ZM0 12.76V10.07H32V12.76H0ZM0 2.69V0H32V2.69H0Z" fill="#E8E8E8" />
                    </svg></button>
                <router-link to='/registration' class="icon-right-2">
                    <svg class="icon-right-2-svg" width="29" height="29"
                        viewBox="0 0 29 29" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path
                            d="M14.5 19.937C19 19.937 22.656 15.464 22.656 9.968C22.656 4.472 19 0 14.5 0C13.3631 0.0217413 12.2463 0.303398 11.2351 0.823397C10.2239 1.34339 9.34507 2.08794 8.66602 3C7.12663 4.99573 6.30819 7.45381 6.34399 9.974C6.34399 15.465 10 19.937 14.5 19.937ZM14.5 1.813C18 1.813 20.844 5.472 20.844 9.969C20.844 14.466 17.998 18.125 14.5 18.125C11.002 18.125 8.15603 14.465 8.15503 9.969C8.15403 5.473 11 1.813 14.5 1.813ZM20.844 18.125C20.6036 18.125 20.373 18.2205 20.203 18.3905C20.033 18.5605 19.9375 18.7911 19.9375 19.0315C19.9375 19.2719 20.033 19.5025 20.203 19.6725C20.373 19.8425 20.6036 19.938 20.844 19.938C22.526 19.9399 24.1386 20.6088 25.3279 21.7982C26.5172 22.9875 27.1861 24.6 27.188 26.282C27.1875 26.5221 27.0918 26.7523 26.922 26.9221C26.7522 27.0918 26.5221 27.1875 26.282 27.188H2.71997C2.47985 27.1875 2.24975 27.0918 2.07996 26.9221C1.91016 26.7523 1.81449 26.5221 1.81396 26.282C1.81608 24.6001 2.48517 22.9877 3.67444 21.7985C4.86371 20.6092 6.47608 19.9401 8.15796 19.938C8.39824 19.938 8.62868 19.8425 8.79858 19.6726C8.96849 19.5027 9.06396 19.2723 9.06396 19.032C9.06396 18.7917 8.96849 18.5613 8.79858 18.3914C8.62868 18.2215 8.39824 18.126 8.15796 18.126C5.99541 18.1279 3.92201 18.9875 2.39258 20.5164C0.863144 22.0453 0.00264777 24.1185 0 26.281C0.000794067 27.0019 0.287502 27.693 0.797241 28.2027C1.30698 28.7125 1.99811 28.9992 2.71899 29H26.282C27.0027 28.9989 27.6936 28.7121 28.2031 28.2024C28.7126 27.6927 28.9992 27.0017 29 26.281C28.9974 24.1187 28.1372 22.0457 26.6083 20.5168C25.0793 18.9878 23.0063 18.1276 20.844 18.125Z"
                            fill="#E8E8E8" />
                    </svg>
                </router-link>
                <router-link to='/cart' class="icon-right-3">
                    <span class="right-nav-counter" id="cartCounter">4</span>
                    <svg class="icon-right-3-svg" width="42" height="37" viewBox="0 0 42 37" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path
                            d="M26.2009 37C25.5532 36.9738 24.9415 36.6948 24.4972 36.2227C24.0529 35.7506 23.8114 35.1232 23.8245 34.475C23.8376 33.8269 24.1043 33.2097 24.5673 32.7559C25.0303 32.3022 25.6527 32.048 26.301 32.048C26.9493 32.048 27.5717 32.3022 28.0347 32.7559C28.4977 33.2097 28.7644 33.8269 28.7775 34.475C28.7906 35.1232 28.549 35.7506 28.1047 36.2227C27.6604 36.6948 27.0488 36.9738 26.401 37H26.2009ZM6.75293 34.32C6.75293 33.79 6.91011 33.2718 7.20459 32.8311C7.49907 32.3904 7.91764 32.0469 8.40735 31.844C8.89705 31.6412 9.43594 31.5881 9.95581 31.6915C10.4757 31.7949 10.9532 32.0502 11.328 32.425C11.7028 32.7998 11.9581 33.2773 12.0615 33.7972C12.1649 34.317 12.1118 34.8559 11.9089 35.3456C11.7061 35.8353 11.3626 36.2539 10.9219 36.5483C10.4812 36.8428 9.96304 37 9.43298 37C9.08087 37.0003 8.73212 36.9311 8.40674 36.7966C8.08136 36.662 7.78569 36.4646 7.53662 36.2158C7.28755 35.9669 7.09001 35.6713 6.9552 35.3461C6.82039 35.0208 6.75098 34.6721 6.75098 34.32H6.75293ZM10.553 28.686C10.2935 28.6868 10.0409 28.6024 9.83411 28.4457C9.62727 28.2891 9.47758 28.0689 9.40796 27.819L4.57495 10.364H1.18201C0.868521 10.364 0.567859 10.2395 0.346191 10.0178C0.124523 9.79614 0 9.49549 0 9.18201C0 8.86852 0.124523 8.56787 0.346191 8.3462C0.567859 8.12454 0.868521 8.00001 1.18201 8.00001H5.46301C5.7225 7.99919 5.97504 8.08372 6.18176 8.24057C6.38848 8.39742 6.53784 8.61788 6.60693 8.86801L11.4399 26.323H24.6179L29.001 16.275H14.401C14.2428 16.2796 14.0854 16.2524 13.9379 16.1951C13.7904 16.1377 13.6559 16.0513 13.5424 15.9411C13.4288 15.8308 13.3386 15.6989 13.277 15.5532C13.2154 15.4074 13.1836 15.2508 13.1836 15.0925C13.1836 14.9343 13.2154 14.7776 13.277 14.6319C13.3386 14.4861 13.4288 14.3542 13.5424 14.2439C13.6559 14.1337 13.7904 14.0473 13.9379 13.9899C14.0854 13.9326 14.2428 13.9054 14.401 13.91H30.814C31.0097 13.91 31.2022 13.9587 31.3744 14.0517C31.5465 14.1448 31.6928 14.2793 31.7999 14.443C31.9078 14.6073 31.9734 14.7957 31.9908 14.9914C32.0083 15.1872 31.9771 15.3842 31.9 15.565L26.495 27.977C26.4026 28.1876 26.251 28.3668 26.0585 28.4927C25.866 28.6186 25.641 28.6858 25.411 28.686H10.553Z"
                            fill="#E8E8E8"
                        />
                    </svg>
                </router-link>

                <nav class="right-nav-dropdown right-nav-dropdown-close">
                    <!-- right-nav-dropdown-open -->
                    <div class="right-nav-group">
                        <button class="right-nav-btn-close">X</button>
                        <p class="right-nav-title">MENU</p>
                        <ul class="right-nav-list">
                            <li class="right-nav-item"><a href="catalog.html" class="right-nav-link">MEN</a>
                                <ul class="right-nav-sublist">
                                    <li class="right-nav-sublist-item"><a href="product.html"
                                            class="right-nav-sublist-link">Accesories</a></li>
                                    <li class="right-nav-sublist-item"><a href="product.html"
                                            class="right-nav-sublist-link">Bags</a></li>
                                    <li class="right-nav-sublist-item"><a href="product.html"
                                            class="right-nav-sublist-link">Denim</a></li>
                                    <li class="right-nav-sublist-item"><a href="product.html"
                                            class="right-nav-sublist-link">T-shirt</a></li>
                                </ul>
                            </li>
                            <li class="right-nav-item"><a href="catalog.html" class="right-nav-link">WOMEN</a>
                                <ul class="right-nav-sublist">
                                    <li class="right-nav-sublist-item"><a href="product.html"
                                            class="right-nav-sublist-link">Accesories</a></li>
                                    <li class="right-nav-sublist-item"><a href="product.html"
                                            class="right-nav-sublist-link">Bags</a></li>
                                    <li class="right-nav-sublist-item"><a href="product.html"
                                            class="right-nav-sublist-link">Denim</a></li>
                                    <li class="right-nav-sublist-item"><a href="product.html"
                                            class="right-nav-sublist-link">T-shirt</a></li>
                                </ul>
                            </li>

                            <li class="right-nav-item"><a href="catalog.html" class="right-nav-link">KIDS</a>
                                <ul class="right-nav-sublist">
                                    <li class="right-nav-sublist-item"><a href="product.html"
                                            class="right-nav-sublist-link">Accesories</a></li>
                                    <li class="right-nav-sublist-item"><a href="product.html"
                                            class="right-nav-sublist-link">Bags</a></li>
                                    <li class="right-nav-sublist-item"><a href="product.html"
                                            class="right-nav-sublist-link">Denim</a></li>
                                    <li class="right-nav-sublist-item"><a href="product.html"
                                            class="right-nav-sublist-link">T-shirt</a></li>
                                </ul>
                            </li>

                        </ul>
                    </div>
                </nav>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
  name: "Header",

  computed: {

    query: {
      get() {
        return this.$store.getters.setQuery
      },

      set(value) {
        this.$store.commit('setQuery', value)
      }
    }
  },
}
</script>

<style>
    input {
        height: 25px;
        margin-left: 15px;
        border-radius: 5px;
    }
</style>