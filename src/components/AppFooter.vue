<script>
import ImportantLinks from './ImportantLinks.vue';

export default {
    name: 'AppFooter',
    components: {
        ImportantLinks,
    },
    data() {
        return {
            implinks: [
                'About me',
                'About us',
                'Language packs',
                'Become a coach',
                'Monthly events'
            ]
        }
    }
}
</script>

<template>
    <section>
        <div class="container">
            <div class="col">
                <h3>About</h3>
                <div class="line"></div>
                <p>We created Everlead to effectively become the stepping stone towards meeting all your goals & achieving business success.</p>
                <div class="icons">
                    <div class="icon">
                        <i class="fa-brands fa-linkedin-in"></i>
                    </div>
                    <div class="icon">
                        <i class="fa-brands fa-facebook-f"></i>
                    </div>
                    <div class="icon">
                        <i class="fa-brands fa-twitter"></i>
                    </div>
                </div>
            </div>
            <div class="col">
                <h3>Twitter</h3>
                <div class="line"></div>
                <div class="d-flex">
                    <i class="fa-brands fa-twitter"></i>
                    <p>
                        <a href="#">@aliasadadm</a> Hi <a href="#">@aliasadadm</a>, can you please submit a ticket at <a href="#">https://t.co/JLV61aXG7d</a> and one of our support agent... <a href="#">https://t.co/yk57k1S9bS</a>
                    </p>
                </div>
                <div class="d-flex">
                    <i class="fa-brands fa-twitter"></i>
                    <p>
                        <a href="#">@HenrySefaBoaky1</a> Check out our theme Gioia which has all necessary elements to build a multi vendor marketplace. <a href="#">https://t.co/c9BIYxZBIL</a>
                    </p>
                </div>
            </div>
            <div class="col">
                <h3>Important links</h3>
                <div class="line"></div>
                <ImportantLinks 
                v-for="implink in implinks"
                :footerlink="implink"
                />
            </div>
            <div class="col">
                <h3>Contact me</h3>
                <div class="line"></div>
                <div class="d-flex">
                    <i class="fa-solid fa-tag"></i>
                    <p>457 BigBlue Street, NY 10013</p>
                </div>
                <div id="pdt" class="d-flex">
                    <i class="fa-solid fa-phone"></i>
                    <p>(315) 5512-2579</p>
                </div>
                <div id="pdt" class="d-flex">
                    <i class="fa-solid fa-envelope"></i>
                    <p>everlead@mikado.com</p>
                </div>
                <div class="newsLetter">
                    <input class="sub" type="text" placeholder="Your Name">
                </div>
            </div>
        </div>
    </section>
    <section class="copyright">
        <p>Copyright Everlead&#169;MikadoThemes</p>
    </section>
</template>

<style lang="scss" scoped>
section {
    background-color: #181515;
    .container {
        max-width: 1400px;
        margin: auto;
        display: flex;
        justify-content: space-between;
        padding: 40px;
        .col {
            width: 25%;
            color: #d6d6d6;
            padding: 20px;
            .line {
                width: 35px;
                border-bottom: 1px solid #ff4c19;
                margin: 20px 0;
            }
            .icons {
                display: flex;
                .icon {
                    font-size: 15px;
                    background-color: #d6d6d6;
                    color: #181515;
                    width: 25px;
                    height: 25px;
                    border-radius: 50%;
                    line-height: 25px;
                    text-align: center;
                    margin-right: 10px;
                    margin-top: 20px;
                }
                .icon:hover {
                    background-color: #ff4c19;
                    color: #d6d6d6;
                }
            }
            .d-flex {
                display: flex;
                i {
                    color: #ff4c19;
                }
                p {
                    padding-left: 20px;
                }
                a {
                    color: #d6d6d6;
                }
            }
            .d-flex:last-child {
                padding-top: 20px;
            }
            .link {
                display: flex;
                flex-direction: column;
            }
            .link a {
                padding-bottom: 10px;
                cursor: pointer;
            }
            #pdt {
                padding-top: 20px;
            }
            .newsLetter {
                position: relative;
                .sub {
                    background-color: inherit;
                    border: none;
                    border-bottom: 1px solid #d6d6d6;
                    width: 100%;
                    padding: 10px;
                    margin-top: 50px;
                    
                }
                .sub::after {
                    content: attr(data-required);
                    position: absolute;
                    right: 0;
                    top: 50%;
                    font-size: 15px;
                    color: #ccc;
                }
            }
        }
    }
}
.copyright {
    background-color: #ff4c19;
    text-align: center;
    color: #d6d6d6;
    padding: 10px 0;
}
</style>