<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-xs-12 wrap">
                    <ul class="socials-items">
                        <li class="item">
                            <a class="item-link" href="https://www.instagram.com/kriss_drummer/">
                                <span class="icon instagram"></span>
                            </a>
                        </li>
                        <li class="item">
                            <a class="item-link" href="https://www.youtube.com/channel/UCpHjRsNuiIfaJR1n_9I0EvQ">
                                <span class="icon youtube"></span>
                            </a>
                        </li>
                        <li class="item">
                            <a class="item-link" href="https://open.spotify.com/playlist/4WebOojLHfQGA4MSv2bkra">
                                <span class="icon spotify"></span>
                            </a>
                        </li>
                    </ul>
                    <div class="copyright">&copy; 2021 &ndash; copyright Kriss Drummer</div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>

    export default {
        
    }

</script>

<style lang="scss">

    footer {
        padding: 110px 0;
        margin-top: 150px;
        background-color: #212121;

        .wrap {
            width: 100%;
        }

        .socials-items {
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0;
            padding: 0;
            list-style: none;

            .item {
                margin-right: 42px;

                &:last-child {
                    margin-right: 0;
                }

                a {
                    display: block;

                    .icon {
                        display: block;
                        width: 64px;
                        height: 64px;
                        background-position: center;
                        background-repeat: no-repeat;
                        background-size: cover;

                        &.instagram {
                            background-image: url('/img/icons/instagram.svg');
                        }

                        &.youtube {
                            background-image: url('/img/icons/youtube.svg');
                        }

                        &.spotify {
                            background-image: url('/img/icons/spotify.svg');
                        }
                    }
                }
            }
        }

        .copyright {
            text-align: center;
            margin-top: 100px;
            color: #999;
            font-weight: 300;
        }
    }

</style>